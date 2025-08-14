# Implementation Blueprint: Closing AI Governance Circumvention Gaps

## Executive Summary

This document provides a concrete 18-month implementation pathway for ten solutions designed to prevent circumvention of AI moratorium frameworks. The approach transforms academic proposals into operational reality through strategic sequencing: voluntary market adoption → financial leverage → international coordination.

**Core Objectives:**
- Raise circumvention costs by ≥10× within 12 months
- Detect GPT-4-scale training with ≥90% recall and ≤5% false positives
- Build momentum through market incentives rather than waiting for perfect consensus

**Key Insight:** Perfect enforcement is neither necessary nor possible. We need only make legitimate pathways more attractive than evasion, buying time for AI safety research while building institutional capacity.

**Resource Requirements:** ~$300-400M coalition investment in Year 1 (less than the cost of one frontier training run)

## Governance Structure

### International AI Safety Commission (IASC)
- New treaty body or G7+EU+key fabs coalition
- Owns: rulebook, thresholds, sanctions coordination, global telemetry hub
- Quarterly threshold adjustments based on efficiency improvements

### National Compute Auditors (NCAs)
- Joint task force: energy regulator + telecom authority + finance ministry
- Owns: licensing, enforcement, domestic monitoring
- Operates fusion watchfloor for real-time detection

### Industry Working Groups
- GPU vendors, cloud providers, ISPs/IXPs, power utilities
- Provide telemetry, implement hardware changes, run pilots
- Coordinate through Compute-ISAC for threat sharing

## Phased Implementation Timeline

### Phase 1: Emergency Response (Days 0-90)
**Objective:** Stand up minimal viable controls using existing infrastructure

#### Immediate Actions
1. **Model Run Notice (MRN) Requirement**
   - Any training >10^24 FLOP must file 14 days before start
   - Strict liability: $250M or 2% global turnover penalties
   - Owner: NCAs implement via emergency order

2. **Software Compute Passports (Gen 1)**
   - Driver-level attestation using TPM/TEE
   - Mandatory for datacenters, optional for on-premise
   - Logs device IDs, kernels, FLOP counts, power to Merkle tree
   - Owner: GPU vendors push signed drivers

3. **Fusion Watchfloor (V0)**
   - Correlates MRNs, cloud logs, NetFlow, power telemetry
   - Basic anomaly detection for undeclared training
   - Owner: NCAs stand up national cells

4. **Whistleblower Framework**
   - $50M bounty authorization using existing financial frameworks
   - 10-30% of collected fines, immunity for incidental participation
   - Owner: Finance/Justice ministries

### Phase 2: Market-Led Adoption (Months 3-6)
**Objective:** Create voluntary adoption through competitive advantage

#### Hardware Security & Insurance
5. **Performance Bonds**
   - $250M minimum for frontier runs
   - Lloyd's/Munich Re offer as new product line
   - Creates market pressure for compliance

6. **Hardware Compute Passports (Gen 2)**
   - Firmware-anchored attestation binding GPU serials
   - NVIDIA/AMD implement as "verified compute" premium feature
   - Transparency logs mirrored to IASC

7. **HSM Weight Protection (V1)**
   - Frontier checkpoints in certified HSMs
   - Publish salted hashes within 24h to IASC registry
   - Cloud providers offer as premium tier

#### Detection Enhancement
8. **Whole-Network Detection (V1)**
   - Correlate telemetry with ISP flow patterns
   - Deploy ML models for distributed training signatures
   - Feature store for: synchronized bursts, power anomalies, residential swarms

9. **Dynamic Thresholds**
   - First quarterly adjustment based on observed efficiency
   - Account for algorithmic improvements (16-month doubling)
   - Prevents gaming through efficiency gains

### Phase 3: Financial Leverage (Months 6-12)
**Objective:** Use economic pressure to force compliance

10. **Extraterritorial Enforcement**
    - Tie foundry access, export licenses to passport compliance
    - SWIFT/dollar-clearing contingent on verification
    - Secondary sanctions for facilitators

11. **International Inspectorate**
    - "Anywhere, anytime" teams with boot-level verification authority
    - Begin with voluntary peer review (UK/Canada/Japan)
    - Expand to surprise audits by Month 9

12. **Sanctions Playbook**
    - Designation pipeline for haven clouds, shell resellers
    - Public "non-compliant venue" list
    - Coordinated through IASC

### Phase 4: Infrastructure Hardening (Months 12-18)
**Objective:** Embed verification in hardware and aid systems

13. **On-Die Compute Passports (Gen 3)**
    - Next silicon tapeout with embedded secure elements
    - Random challenge-response, power-signal attestation
    - Makes circumvention require semiconductor manufacturing

14. **Conditional Infrastructure Aid**
    - World Bank facility for pre-certified datacenters
    - Built-in telemetry as condition for loans
    - Target: Kenya, Philippines, Chile pilots

15. **Sunset & Iteration**
    - 30-month automatic reauthorization requirement
    - Published impact assessments
    - Forces continuous adaptation

## Workstream Mapping

| WS | Deliverable | Owner | Timeline | Dependencies | Success Metric |
|----|------------|--------|----------|--------------|----------------|
| WS1 | Compute Passports (Gen 1→3) | GPU vendors, clouds | D90/M6/M18 | Legal safe harbor | 95% datacenter coverage by M12 |
| WS2 | Dynamic Thresholds | IASC | Quarterly | MRN data | First adjustment by M4 |
| WS3 | Secondary Sanctions | Treasuries | M6 | G7 alignment | 2+ designated entities by M9 |
| WS4 | Network Detection | IASC + NCAs | M4 MVP/M7 V1 | Telemetry MOUs | <24h detection latency |
| WS5 | Inspectorate | IASC | M9 | Treaty/MOU | First inspection by M10 |
| WS6 | HSM Weights | Labs + vendors | M8 | Legal mandate | 100% frontier runs by M12 |
| WS7 | Performance Bonds | NCAs + insurers | D60 pilot | Authority | 3+ labs purchase by M6 |
| WS8 | Whistleblower | Finance/Justice | D60 | Appropriation | First payout by M9 |
| WS9 | Infrastructure Aid | MDBs | M10 | Vendor specs | 3 countries by M18 |
| WS10 | Sunset Clause | IASC | M15 | Metrics | First review complete |

## Technical Specifications

### Compute Passport Data Schema (Gen 1)
```json
{
  "timestamp": "RFC3339",
  "gpu_serial": "string",
  "host_id": "TPM_EK_fingerprint",
  "driver_version": "semver",
  "kernel_digest": "SHA256(program + params)",
  "kernel_class": "enum{matmul, attention, conv, allreduce, other}",
  "accumulated_flops": "uint64",
  "instantaneous_power_w": "uint16",
  "memory_bandwidth_gbps": "uint16",
  "nonce": "uint128",
  "signature": "Ed25519(host_TEE_key)"
}
```

### Detection Pipeline
```
for each gpu in fleet:
  verify(signature, host_TEE_key)
  assert(timestamp monotonic && nonce fresh)
  append_to_merkle(gpu_log)
  if power_signature != model(power, mem_bw, kernel_class): 
    flag_anomaly
    
aggregate fleet:
  compare ∑accumulated_flops vs facility power & cooling
  cross_check with ISP flow patterns
  if projected_run > threshold && no MRN: 
    alert → NCA
```

### Training Fingerprint Features
- Synchronized all-reduce bursts with 10-60s cadence
- Sustained 5-15% above P95 power during nights/weekends  
- Repeating high-entropy kernel mix (matmul/attention patterns)
- Residential CGN clusters with periodic 64-128KB bursts

## Legal Framework Examples

### Model Run Notice (Statutory Text)
> Any person or entity initiating training whose projected compute exceeds 10^24 floating-point operations shall file a Model Run Notice 14 days prior. The Notice shall include: (a) model family and parameters; (b) compute budget; (c) facility identifiers; (d) hardware inventory; (e) attestation modality. Failure constitutes strict-liability offense with penalties up to 2% global turnover or $250M, whichever greater.

### Compute Passport Mandate
> Operation of accelerators exceeding 10^13 FLOP/s without passport telemetry is unlawful. Vendors shall provide signed drivers collecting runtime metadata anchored to transparency logs. Operators retain raw logs for 5 years. Good-faith compliance provides safe harbor from incidental disclosure liability.

### Performance Bond Requirement
> Licenses for threshold-exceeding runs require $250,000,000 performance bond. Partial forfeiture upon: (a) missing checkpoint hashes; (b) inspectorate obstruction; (c) >10% undeclared compute. Full forfeiture for unauthorized deployment.

## Targeted Countermeasures by Circumvention Path

### Regulatory Havens
**Detection:** 
- Corporate registry monitoring for "AI Innovation Zones"
- Unusual GPU import patterns and power permits
- AS/ASN registration anomalies

**Disruption:**
- Secondary sanctions on haven clouds
- Block firmware updates for non-compliant serials
- Deny spare parts and maintenance

**Deterrence:**
- Public non-compliant venue list
- Loss of research grants for customers
- Reputational costs for participants

### Distributed GPU Swarms
**Detection:**
- Residential CGN flow fingerprints
- CDN telemetry for model-shard distribution
- App store scanning for training clients

**Disruption:**
- ISP terms of service enforcement
- Rate-limit suspicious all-reduce patterns
- Require notarized drivers for high-TDP consumer GPUs

**Deterrence:**
- Focus bounties on builders not participants
- Voluntary amnesty windows
- Civil liability funded by bonds

### Covert State Supercomputers
**Detection:**
- Satellite thermal/power anomalies
- Absent firmware ping responses
- Job mix audits via inspectorate

**Disruption:**
- Export controls on maintenance
- Bar foundry access without compliance
- Research collaboration isolation

**Deterrence:**
- Quiet diplomatic demarches
- Conditional scientific access
- Peer pressure through allies

### Offshore Proxy Datacenters
**Detection:**
- Aid flow tracing (loans → DC builds)
- Containerized modular DC shipments
- Atypical GPU densities in "edge" nodes

**Disruption:**
- Port-state control for GPU containers
- Revoke ASN allocations for shells
- Customs holds without certificates

**Deterrence:**
- Attractive pre-certified alternatives
- Preferential power tariffs for compliant facilities
- Development aid contingent on telemetry

## Critical Open Questions

### Technical Uncertainties
- **Retrofit feasibility:** Can 10M+ existing GPUs be upgraded with secure elements?
- **Cryptographic overhead:** Can attestation stay below 0.1% performance impact?
- **Detection accuracy:** What false positive rate is acceptable?
- **Evasion resistance:** Will determined actors always find workarounds?
- **Distributed training:** How to enable while maintaining HSM custody?

### Policy Uncertainties
- **Legal definitions:** Where's the line between training, fine-tuning, and inference?
- **Minimum coalition:** Is G7 sufficient or is China participation essential?
- **WTO compatibility:** Do compute controls violate trade commitments?
- **Privacy balance:** How to detect without mass surveillance?
- **Governance structure:** UN agency, treaty organization, or industry body?

### Economic Uncertainties
- **Compliance costs:** Full economic impact across supply chain?
- **Innovation effects:** Will regulations entrench incumbents?
- **Insurance pricing:** How to price unprecedented AI risks?
- **Sanctions effectiveness:** Can financial pressure overcome sovereignty?

## Research Priorities

### Immediate (0-3 months)
1. **Performance study:** Cryptographic attestation impact on training workloads
2. **Traffic analysis:** Distributed training signatures despite encryption
3. **Legal review:** Extraterritorial enforcement under international law
4. **Economic modeling:** Compliance vs circumvention cost curves

### Near-term (3-6 months)
1. **Historical analysis:** Lessons from nuclear/chemical/bio control regimes
2. **Game theory:** First-mover advantages and defection incentives
3. **Technical standards:** NIST/ISO specifications for compute attestation
4. **Efficiency tracking:** Objective metrics for algorithmic improvements

### Long-term (6-12 months)
1. **Governance design:** Structures resistant to regulatory capture
2. **Attribution systems:** Forensic capabilities for model provenance
3. **Market analysis:** Impact on competition and innovation
4. **International framework:** Minimal viable coalition analysis

## Key Performance Indicators

### 6-Month Targets
- 80% of member-state accelerators emitting telemetry
- 3+ frontier labs adopt voluntary measures
- First threshold adjustment implemented
- $100M in performance bonds purchased

### 12-Month Targets
- 95% telemetry coverage in participating jurisdictions
- Detection recall ≥90%, false positives ≤5%
- First successful whistleblower payout
- 5+ countries join inspection framework

### 18-Month Targets
- No undetected frontier training for 6+ months
- Distributed training costs 5x premium vs compliant
- 40+ signatories to international framework
- Haven state problem substantially mitigated

## Resource Requirements (Year 1)

| Component | Cost | Description |
|-----------|------|-------------|
| IASC Secretariat | $35M | Staff, infrastructure, analytics platform |
| Vendor Engineering | $60M | Driver/firmware development (co-funded) |
| National NCAs | $8-12M/country | Telemetry, inspectors, legal |
| Inspectorate Setup | $25M | Equipment, training, operations |
| Bounty Fund | $100M | Initial seed (replenished by fines) |
| Infrastructure Aid | $50M | Pilot datacenter projects |
| **Total Coalition** | **$300-400M** | Less than one frontier training run |

## Immediate Next Steps by Stakeholder

### AI Companies (Within 30 days)
- Implement internal compute accounting for all runs
- Establish risk officer with board reporting
- Pilot HSM weight protection on one model
- Join voluntary safety commitments

### Governments (Within 30 days)
- Map domestic compute >10^17 FLOPS
- Establish interagency AI task force
- Draft MRN emergency order
- Begin bilateral standards discussions

### Researchers (Within 30 days)
- Document compute for all experiments
- Prototype detection using public data
- Publish technical standards proposals
- Study historical control precedents

### Civil Society (Within 30 days)
- Build cross-sector coalition
- Document distributed training capabilities
- Educate policymakers on realities
- Propose equity-focused guidelines

## Risk Mitigation & Contingencies

### If China doesn't participate
- Focus on supply chain controls (TSMC, ASML)
- Strengthen allied coordination
- Prepare for bifurcated ecosystem

### If industry resists
- Start with government/academic facilities
- Use procurement power for leverage
- Consider regulatory mandates earlier

### If detection fails
- Increase bounty amounts
- Expand inspector authorities
- Lower intervention thresholds

### If costs exceed estimates
- Prioritize highest-impact measures
- Seek private sector co-funding
- Phase implementation more gradually

## Evaluation & Adaptation

### Quarterly Reviews
- Detection accuracy metrics
- Compliance rates by sector
- Cost-benefit analysis updates
- Threat landscape evolution

### Annual Assessment
- Full program evaluation
- Stakeholder feedback integration
- Threshold recalibration
- International expansion planning

### 30-Month Sunset
- Comprehensive impact assessment
- Public comment period
- Legislative reauthorization
- Next-generation requirements

## Conclusion

This blueprint transforms theoretical governance proposals into operational reality within 18 months. By sequencing implementation through market incentives, financial leverage, and gradual formalization, we can build momentum without waiting for perfect consensus.

The window for effective action is narrowing as capabilities advance and national strategies diverge. Beginning with voluntary adoption in the next 90 days could catalyze comprehensive governance within 18 months. The alternative—waiting for unanimous agreement—guarantees circumvention pathways will be exploited.

Success requires accepting imperfection while maintaining adaptability. The goal is not absolute control but sufficient friction to make compliance more attractive than evasion, buying crucial time for AI safety research and institutional development.

**Next step:** Convene working groups for each solution with industry, government, academic, and civil society representation to transform these proposals into detailed technical specifications and model legislation.

## Appendices (Available on Request)

1. Model Run Notice template form
2. Compute Passport technical specification v1.0
3. Inspectorate Standard Operating Procedures
4. Sanctions designation criteria and process
5. Checkpoint Hash Registry API documentation
6. Whistleblower portal security requirements
7. Pre-certified datacenter blueprints
8. Red-team exercise scenarios
9. Historical case studies analysis
10. Economic impact modeling spreadsheets