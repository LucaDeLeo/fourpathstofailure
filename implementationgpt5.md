## Implementation Blueprint (12–18 months)

**Objective:** Stand up a minimally viable but globally leverageable regime that (1) raises the cost of moratorium evasion by ≥10× within 12 months and (2) detects GPT‑4‑scale training attempts with ≥90% recall and ≤5% false positives across participating jurisdictions.

### Program governance (who runs this)

* **International AI Safety Commission (IASC)** – new treaty body or interim coalition secretariat (G7+EU+key fabs). Owns rulebook, thresholds, sanctions coordination, and the global telemetry hub.
* **National Compute Auditors (NCAs)** – one per member state (e.g., energy regulator + telecom regulator + finance ministry joint task force). Own licensing and enforcement on national soil.
* **Industry Working Groups** – GPU vendors, cloud providers, ISPs/IXPs, and power utilities. Provide telemetry, implement hardware/driver changes, and run pilots.
* **Compute-ISAC** – an information‑sharing community for real‑time alerts (modelled on sectoral ISACs).

---

## Roadmap at a Glance

### First 90 days (MVP control)

1. **Emergency Order + Model Run Notice (MRN v0.1):** Any training run **projected** to exceed 10^24 FLOP must file an MRN 14 days before start. (Owner: NCAs)
2. **Software‑attested “Compute Passport – Gen1” (driver level):** Mandatory for data centers and clouds; optional for on‑prem. Uses host TPM/TEE + signed driver to log device IDs, kernel digests, FLOP counters, and power draw to a Merkle log. (Owners: GPU vendors + clouds)
3. **Fusion Watchfloor (V0):** A national cell that ingests (a) MRNs, (b) cloud logs, (c) backbone NetFlow summaries from IXPs, (d) bulk power telemetry from utilities. (Owner: NCAs)
4. **\$50M whistleblower bounty rulemaking (draft):** Align with existing financial whistleblower frameworks to allow rapid adoption. (Owner: Finance/Justice ministries)
5. **Performance Bonds (pilot):** Require bonds for declared frontier runs in regulated clouds (\$250M floor). (Owner: NCAs; bonding capacity via reinsurers)

### 3–6 months (from MVP to verifiable regime)

6. **Hardware‑anchored “Compute Passport – Gen2”:** Vendor firmware update that binds GPU serials to signed runtime metrics; logs anchored to vendor transparency service and mirrored to IASC. (Owners: GPU vendors)
7. **Whole‑of‑Network Detection (V1):** Correlate Gen1/Gen2 logs with ISP/IXP flow anomalies and substation‑level power spikes; deploy feature store and anomaly models. (Owners: IASC + NCAs)
8. **Dynamic Thresholds (quarterly):** IASC publishes updated risk thresholds and evaluation gates informed by observed scaling efficiency. (Owner: IASC)
9. **Extraterritorial Levers:** Treasury/Trade issue rules tying foundry access, export licenses, and dollar clearing to passport compliance. (Owners: member states)

### 6–12 months (closing the hard gaps)

10. **International Inspectorate (“anywhere, anytime”)**: Teams trained to perform boot‑level verification, on‑site log validation, and surprise power/network audits. (Owner: IASC)
11. **HSM Weight Custody (V1):** Frontier checkpoints must live inside certified HSMs; each checkpoint publishes a salted hash within 24h to IASC registry. (Owners: model developers + HSM vendors)
12. **Sanctions & Listings Playbook:** Designation pipeline for haven clouds, shell resellers, and state proxies; secondary sanctions procedures. (Owners: IASC + member treasuries)

### 12–18 months (hardening + scale)

13. **Compute Passport – Gen3 (on‑die):** Next silicon tape‑out with embedded secure element, signed kernel‑class summaries, random challenge‑response, and power‑signal attestation. (Owners: GPU vendors/foundries)
14. **Infrastructure Aid with Compliance:** Development bank facility for pre‑certified datacenter blueprints with built‑in telemetry. (Owners: MDBs + IASC)
15. **Sunset & Iteration Clause:** Every 30 months, automatic re‑authorization with published impact assessment. (Owner: IASC)

---

## Workstreams (mapped to your 10 recommendations)

| WS   | Workstream                        | What ships                                          | Owner                    | When                 | Dependencies                       |
| ---- | --------------------------------- | --------------------------------------------------- | ------------------------ | -------------------- | ---------------------------------- |
| WS1  | **Compute Passports (Gen1→Gen3)** | Signed device metrics → vendor firmware → on‑die SE | GPU vendors, clouds      | D90 / M6 / M18       | Legal safe harbor; export controls |
| WS2  | **Dynamic Thresholds**            | Quarterly risk thresholds + test suite              | IASC                     | Q+90 ongoing         | MRN data; observed runs            |
| WS3  | **Secondary Sanctions**           | Listings, KYC rules, dollar‑clearing conditions     | Treasuries               | M6                   | Diplomatic alignment               |
| WS4  | **Whole‑Network Detection**       | Fusion platform, feature store, ML alerts           | IASC + NCAs              | M4 MVP / M7 V1       | Telemetry MOUs (WS1, WS7)          |
| WS5  | **Inspectorate**                  | SOPs, kits, legal mandate                           | IASC                     | M9                   | Treaty/coalition MoU               |
| WS6  | **HSM Weight Protection**         | Certified HSM profile + hash registry               | Model labs + HSM vendors | M8                   | Legal mandate for hashes           |
| WS7  | **Performance Bonds**             | Bonding rule + triggers                             | NCAs + reinsurers        | D60 pilot / M6 scale | Statutory authority                |
| WS8  | **Whistleblower Bounties**        | Rulebook + secure portal + payouts                  | Finance/Justice          | D60                  | Fund appropriation                 |
| WS9  | **Infra Aid + Templates**         | Pre‑cert DC blueprint + telemetry                   | MDBs + utilities         | M10                  | Vendor specs                       |
| WS10 | **Sunset & Iteration**            | Review process + auto‑sunset                        | IASC                     | M15                  | Metrics + audits                   |

---

## Technical Reference (drop‑in appendix)

### A. Compute Passport (Gen1) – minimal viable spec

**Goal:** No new silicon; use signed drivers + host TPM/TEE.

**Data elements per GPU (every 5s rolling window):**

```json
{
  "ts": "RFC3339",
  "gpu_serial": "string",
  "host_id": "TPM_EK_fingerprint",
  "driver_version": "semver",
  "kernel_digest": "SHA256(program text + launch params)",
  "kernel_class": "enum{matmul, attention, conv, allreduce, other}",
  "accumulated_flops": "uint64",
  "instantaneous_power_w": "uint16",
  "mem_bw_gbps": "uint16",
  "nonce": "uint128",
  "sig": "Ed25519(host_TEE_key)"
}
```

* **Integrity:** Append to a local Merkle tree; publish tree heads (every minute) to vendor and IASC mirrors.
* **Privacy:** No user data; only runtime metadata. Allow labs to **zero‑knowledge attest** “≤ X FLOP today” without revealing kernels (proof circuit later; not required for Gen1).
* **Tamper checks:** Random challenge packets from vendor relay must trigger synthetic micro‑kernels with known power/latency signatures.

**Verification pipeline (high‑level pseudocode):**

```
for each gpu in fleet:
  verify(sig, host_TEE_key)
  assert(ts monotonic && nonce fresh)
  append_to_merkle(gpu_log)
  if power_signature != model(power, mem_bw, kernel_class): flag_anomaly
aggregate fleet:
  compare ∑accumulated_flops vs. facility power draw & cooling envelope
  cross-check with ISP flow features (see B)
  if projected run > threshold && no MRN: issue alert → NCA
```

### B. Whole‑of‑Network Detection (V1)

**Signals fused:**

* **Telemetry:** Passport logs (WS1).
* **Backbone flows:** IXPs/ISPs provide 5‑tuple flow summaries + byte counts at 1‑min intervals for known DC ASNs and residential CGNs. No payloads.
* **Power:** Substation‑level MW draw and variance (1‑min).
* **Cloud scheduler:** Large block reservations, abnormal inter‑region traffic.

**Feature examples (training-time fingerprints):**

* Diurnal spread of synchronized, wide‑fanout all‑reduce bursts
* Repeating high‑entropy kernel mix with matmul/attention cadence
* Sustained 5–15% above historical P95 power draw at cool nights/weekends
* Residential CGN clusters with periodic 64–128 kB bursts at 10–60 s cadence (decentralized swarms)

**Actioning:** Alerts graded A/B/C. A‑alerts (≥0.85 posterior) generate immediate on‑site inspection authority and bond escalations.

### C. HSM Weight Custody (V1)

* **Requirement:** All checkpoints for runs >IASC‑threshold reside in **certified HSMs** (PCIe card or cloud KMS with attestation).
* **Public artifact:** `checkpoint_hash(timestamp, model_id, salt)` posted to IASC within 24h.
* **Forensics:** If leaked weights surface, the public hash window narrows breach time; bond forfeiture triggers.

---

## Legal & Policy Pack (copy‑paste grade)

### 1) Model Run Notice (MRN) – statutory text (excerpt)

> Any person or entity intending to initiate a training run whose **projected compute budget** exceeds **10^24 floating‑point operations** shall file a **Model Run Notice** no later than **14 days** prior to initiation. The Notice shall include: (a) model family and parameter target; (b) projected compute budget; (c) compute facility identifiers; (d) hardware inventory with serials; (e) attestation modality (Gen1/Gen2/Gen3). Failure to file constitutes a **strict‑liability offense** with penalties up to **2% of global turnover** or **\$250M**, whichever is greater.

### 2) Compute Passport Mandate (driver‑based, transitional)

> It shall be unlawful to operate accelerators exceeding **10^13 FLOP·s⁻¹** without **passport telemetry enabled**. Vendors shall provide signed drivers that collect runtime metadata and anchor Merkle heads to a transparency log operated by the vendor and mirrored to the Commission. Operators shall retain raw logs for **5 years**. Good‑faith operators receive **safe harbor** from incidental disclosure liability for telemetry.

### 3) Bonding & Kill‑Switch Clause

> Applicants for licenses to conduct runs exceeding threshold shall post a **performance bond** of not less than **\$250,000,000**. Bonds are subject to immediate partial forfeiture upon: (a) failure to publish checkpoint hashes within 24h, (b) inspectorate obstruction, (c) detection of undeclared compute >10% of projected budget. Full forfeiture and injunctive relief upon confirmed unauthorized deployment.

### 4) Whistleblower Bounties

> The first individual(s) providing **original information** leading to successful enforcement actions related to unauthorized training shall receive **10–30%** of collected monetary sanctions, capped at **\$50,000,000**, with non‑prosecution assurances for incidental participation disclosures.

### 5) Secondary Sanctions Trigger

> The Commission shall designate foreign persons that **knowingly facilitate** unlicensed threshold‑exceeding compute, including by providing data center capacity, hardware, financing, or network transit. Designation triggers: (a) prohibition on dollar clearing, (b) export license denial (semiconductors/fabs), (c) correspondent account restrictions.

---

## Targeted Playbooks for the Four Circumvention Pathways

### A) **Regulatory Havens**

* **Detection:** Corporate registry scraping + AS/ASN monitoring + cloud SKU catalogs; look for “AI Innovation Zone” anomalies (sudden GPU imports, unusual power permits).
* **Disruption:** Secondary sanctions on haven clouds; seize/deny spare parts; block firmware updates (vendors cut keys for non‑compliant serials).
* **Deterrence:** Public “non‑compliant venue” list; customers procuring from listed venues lose eligibility for research grants and export licenses.

### B) **Distributed GPU Swarms**

* **Detection:** Residential CGN flow fingerprints + CDN telemetry (frequent small payload model‑shards) + app‑store scanning for “training clients.”
* **Disruption:** ISP terms of service updates; rate‑limit suspicious all‑reduce patterns; notarized driver requirement for high‑TDP GPUs on consumer OSes.
* **Deterrence:** Bounty focus—pay the builders; voluntary amnesty window for participants; civil liability for payout fund seeded by bonds.

### C) **Covert State Supercomputers**

* **Detection:** Satellite + grid telemetry (nighttime heat/power anomalies); facility job mix audits via inspectorate; vendor firmware ping responses (absent = red flag).
* **Disruption:** Export controls on maintenance parts; bar foundry access for national labs lacking passport compliance; allied research isolation.
* **Deterrence:** Quiet demarches + conditional access to scientific collaborations contingent on inspectorate access.

### D) **Offshore Proxy Datacenters**

* **Detection:** Aid‑flow tracing (MDB loans → DC builds), containerized modular DC shipments, 5G “edge” nodes with atypical GPU densities.
* **Disruption:** Port‑state control analogues (customs holds for GPU containers without compliance certificates); revocation of ASN allocations for shell operators.
* **Deterrence:** Infrastructure‑aid alternative with pre‑cert templates; preferential electricity tariffs only for attested facilities.

---

## KPIs & Milestones

* **Coverage:** ≥80% of accelerators in member states emitting Gen1/Gen2 telemetry by Month 6; ≥95% by Month 12.
* **Detection:** A‑alert recall ≥90% on red‑team training runs; false positive rate ≤5%.
* **Compliance:** 100% of declared frontier runs publishing checkpoint hashes within 24h.
* **Deterrence:** ≥3 successful bounty cases and ≥2 sanctioned entities by Month 9.
* **Latency:** Median time from anomaly to NCA action ≤24 hours (M7).

---

## Resourcing & ROM Budget (Year 1)

* **IASC Secretariat & Watchfloor:** \~\$35M (people, secure infra, analytics)
* **Vendor Engineering (Gen1/Gen2 drivers & firmware):** \~\$60M (co‑funded by vendors + grants)
* **NCAs (per mid‑size country):** \$8–12M (telemetry ingestion, inspectors, legal)
* **Inspectorate setup:** \~\$25M (kits, ops, training)
* **Bounty Fund (seed):** \$100M (replenished by fines)
* **Bonding doesn’t cost the state** (market capacity via reinsurers)

*Total coalition order‑of‑magnitude:* **\$300–400M** in year one (small compared to one frontier run).

---

## Privacy, Security, and Operator Incentives

* **Data minimization:** No payload content; only runtime metadata.
* **Access controls:** Vendor ↔ IASC transparency logs are public for tree heads; raw logs accessible under subpoena or inspectorate warrants.
* **Safe harbor:** Good‑faith telemetry + prompt MRN = protection from minor paperwork defects.
* **Positive carrots:** Reduced insurance premia, fast‑track export licenses, and tax credits for attested facilities.

---

## Red‑Team & Drill Schedule

* **Quarterly “black‑box” drills:** Seed decoy swarms and covert runs; measure time‑to‑detect and adjudicate.
* **Annual haven state exercise:** Simulate sanctions playbook end‑to‑end with partners.
* **Leak‑response tabletop:** From checkpoint hash mismatch to bond forfeiture and public comms in <72h.

---

## Drop‑in Annexes (you can include as appendices)

1. **MRN template** (one‑page form)
2. **Passport telemetry MOU** (vendor ↔ regulator)
3. **Inspectorate SOP** (checklist for on‑site verification)
4. **Sanctions designation criteria** (clear thresholds; evidentiary standards)
5. **Checkpoint Hash Registry API** (POST `/hashes`, GET `/model/{id}`)

---

### What this buys you—even without perfection

* **Immediate friction** for would‑be violators (bonds, telemetry, and sanctions).
* **Early‑warning radar** through cross‑domain signals (compute + power + network).
* **Forensics hooks** (checkpoint hashes, Merkle logs) that make leaks and covert training **provably attributable**.
* **A living regime** via quarterly thresholds and the 30‑month sunset that forces iteration.
