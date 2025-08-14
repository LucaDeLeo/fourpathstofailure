# Perfect Implementation Isn't Enough: Four Paths Around an ASI Moratorium and How to Block Them

**TL;DR: Four paths around an ASI moratorium**

1. **Jurisdiction shopping** in "AI innovation zones"
2. **Distributed GPU swarms** staying below per-device thresholds
3. **Covert state programs** behind classification shields
4. **Offshore proxy datacenters** under sovereignty protection

**Countermeasures:** cryptographic **compute passports**, whistleblower awards (10–30% of monetary sanctions), **performance bonds**, and **anywhere-anytime inspections**.

**Why now:** [EU AI Act is live](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) with a [1e25 FLOP trigger](https://ec.europa.eu/commission/presscorner/detail/en/qanda_21_1683); the U.S. is pushing deregulatory growth via [America's AI Action Plan](https://www.whitehouse.gov/wp-content/uploads/2025/07/Americas-AI-Action-Plan.pdf), creating exploitable asymmetry.

**What happens next quarter:** • **Run-notice pilot at 1e24 FLOP** in coalition jurisdictions; **strict-liability** penalties posted • **Cloud-first driver attestation default-on** (hyperscalers only), with **public attestation receipts** • **Fusion watchfloor v0.1**: IXPs + cloud flow logs + bulk-power anomalies (monthly anomaly report) • **Whistleblower awards** aligned to SEC framework (10–30% of monetary sanctions)

**Origin & Methodology:** This analysis emerged from winning first place in [Apart Research's "Red-Teaming the Narrow Path" hackathon](https://apartresearch.com/project/four-paths-to-failure-red-teaming-asi-governance-se53), where we systematically stress-tested proposed AI governance frameworks through adversarial thinking. We're continuing this work through Apart Lab Studio with mentorship from the ControlAI team.

## Introduction: The Governance Paradox of Transformative AI

What if we achieved the impossible: perfect global cooperation on AI safety, and it still wasn't enough?

*Epistemic status: We're governance research newcomers who approached this problem through systematic adversarial analysis. While our fresh perspective may catch overlooked vulnerabilities, we defer to domain experts on political feasibility and implementation details. Our confidence is highest on technical circumvention methods (based on documented capabilities) and lower on international coordination dynamics.*

*Confidence by claim:*

- **GPU swarms can reach 1e25 FLOP in <12 months for <$30M-60M**: 70%, crux: achievable utilization on 1 Gbps links + churn (cost assumes mix of rental, used hardware, or illicit access)
- **Haven states could field offshore proxies within 12 months**: 60%, crux: GPU supply chains + cover stories
- **Watchfloor can detect GPT-4-scale runs within 24h at ≤10% FPR**: 40%, crux: IXP coverage + kernel attestation adoption (author estimate based on fusion of multiple signals)
- **Covert state programs could operate undetected for 6+ months**: 80%, crux: classification shields + dual-use cover
- **Secondary sanctions could reduce haven state participation**: 50%, crux: enforcement will vs sovereignty claims

We face a documented reality. Even as international bodies converge on sophisticated regulatory frameworks for artificial superintelligence (ASI), a troubling reality emerges: the very nature of AI development may make it ungovernable through traditional means.

The [Narrow Path's proposed twenty-year moratorium](https://pdf.narrowpath.co/A_Narrow_Path.pdf) on ASI development represents humanity's most ambitious attempt at coordinated technological restraint. Yet beneath the surface of this comprehensive proposal lies a troubling reality: the characteristics that make AI development dangerous also make it uniquely resistant to control mechanisms.

This analysis examines four distinct pathways through which determined actors could circumvent even the most comprehensive ASI moratorium. Each pathway could enable GPT-4-scale training within 6-18 months, exploiting fundamental weaknesses in our current governance paradigms.

## The Current Regulatory Landscape

As we write this, the global AI governance landscape is rapidly evolving. The [EU AI Act, which entered force in August 2024](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai), establishes the world's first comprehensive AI regulatory framework, including the [1e25 FLOP threshold for systemic risk](https://ec.europa.eu/commission/presscorner/detail/en/qanda_21_1683) that features prominently in moratorium proposals. GPAI obligations under the Act apply from August 2, 2025. Meanwhile, [America's AI Action Plan (July 2025)](https://www.whitehouse.gov/wp-content/uploads/2025/07/Americas-AI-Action-Plan.pdf) takes a starkly different approach, emphasizing innovation and competitiveness while streamlining regulatory processes. This divergence creates precisely the regulatory asymmetry that determined actors could exploit.

## The Moratorium's Achilles Heel: Understanding the Enforcement Challenge

The [Narrow Path's Phase 0](https://pdf.narrowpath.co/A_Narrow_Path.pdf) proposes a comprehensive regulatory framework including: training licenses for runs above 1e25 FLOP (total training compute), compute licenses for cloud providers above 1e17 FLOP/s, application licenses for new deployments, and prohibition of specific dangerous capabilities. The proposal includes monitoring of data centers' energy consumption with approximately 12-day intervention windows.

**Critical metric clarification:** All thresholds refer to **training-relevant FP FLOP/s measured via attested microbenchmarks**, not INT8 TOPS or other metrics. This distinction matters because consumer NPUs advertise INT8 performance while training requires FP16/BF16/FP8 precision.

While the framework proposes defense-in-depth approaches with multiple layers of oversight, the four circumvention pathways explored here reveal how determined actors could exploit gaps between jurisdictions, leverage distributed infrastructure, and abuse dual-use technologies to undermine these safeguards.

## Pathway One: How Regulatory Flight Happens

### Historical Precedents and Modern Parallels

When the United States restricted federal funding for embryonic stem cell research in 2001, Singapore, the UK, and South Korea expanded their research programs in the field. FTX relocated its headquarters to the Bahamas in September 2021 amid China's crypto crackdown and for a friendlier regulatory environment. [Binance allegedly instructed US customers to use VPNs to bypass restrictions](https://www.cftc.gov/media/8351/%20enfbinancecomplaint032723/download) while maintaining plausible deniability.

### The AI Innovation Zone Scenario

Small nations could establish "AI Innovation Zones" offering tax holidays and state protection. The instant transmissibility of trained models means breakthroughs achieved anywhere can deploy globally through CDN endpoints.

The [A.Q. Khan network operated for decades](https://core.ac.uk/download/pdf/36732689.pdf) despite export controls, using shell companies in Dubai and Malaysia. When US export controls threatened PGP encryption, [Phil Zimmermann published the source code as a book](https://en.wikipedia.org/wiki/Pretty_Good_Privacy#Criminal_investigation), leveraging First Amendment protections.

## Pathway Two: How GPU Swarms Scale

### Technical Feasibility and Historical Validation

Training frontier AI models on distributed consumer hardware is technically feasible today. [Deep Gradient Compression (DGC) algorithms have achieved 270×–600× communication reduction](https://arxiv.org/abs/1712.01887), making training viable over home internet connections.

### Transparent BOTEC: Can 50,000 Consumer GPUs Reach 1e25 FLOP?

Let's show the math with explicit assumptions readers can challenge:

**Assumptions:**

- **GPU count**: 50,000 RTX-class cards
- **Effective throughput per card**: 40 TFLOP/s (FP16/BF16, after discounting headline specs)
- **Aggregate peak**: 50,000 × 40×10¹² = 2.0×10¹⁸ FLOP/s
- **Utilization factor**: 20% (accounting for communication overhead, stragglers, downtime)
- **Effective sustained throughput**: 4.0×10¹⁷ FLOP/s

**Calculation:**

- Time to 1e25 FLOP = 1e25 / 4.0×10¹⁷ = 2.5×10⁷ seconds
- **Result: ~290 days (~9.5 months)**

*Adjust the 40 TFLOP/s assumption or 20% utilization to test sensitivity. Gradient compression improvements could push utilization higher. Cost estimates of $30-60M assume a mix of approaches including rental markets, used hardware, or illicit access to compute.*

[Folding@home achieved 1.5 exaFLOP/s](https://foldingathome.org/2021/01/05/2020-in-review-and-happy-new-year-2021/), exceeding the world's top supercomputers combined during the COVID-19 research surge.

Remarkably, [0G Labs with China Mobile recently announced](https://thedefiant.io/news/press-releases/0g-labs-achieves-breakthrough-in-decentralized-ai-training-with-100-billion-parameters) their DiLoCoX framework achieving 10x speed improvement in distributed AI training **(vendor-reported results, under validation)**. They claim to have trained a 107 billion parameter model on 1 Gbps networks using decentralized clusters. Related research like [OpenDiLoCo](https://arxiv.org/abs/2407.07852) demonstrates cross-continent training with 90-95% utilization.

### The Botnet Precedent

The [Smominru botnet infected 500,000+ machines generating $8,500/day](https://www.proofpoint.com/us/threat-insight/post/smominru-monero-mining-botnet-making-millions-operators) in cryptocurrency. BitTorrent had approximately 150 million monthly active users at peak. The engineering for distributed AI training (asynchronous gradient updates, fault tolerance, dynamic participation) is largely solved.

## Pathway Three: How Covert State Programs Hide

### The Biopreparat Model

The Soviet Union operated Biopreparat from 1974-1991, reportedly employing tens of thousands across dozens of facilities while violating the Biological Weapons Convention. Facilities masqueraded as pharmaceutical plants. The 1979 Sverdlovsk anthrax leak killed approximately 100 people, yet the program remained hidden until defector exposure in 1989.

### Repurposing Existing Infrastructure

Countries operate exascale supercomputers for climate modeling, pharmaceutical research, and nuclear simulations. These facilities already have cleared personnel and city-scale power. Repurposing requires only new software. Staff could continue using existing terminology: "molecular dynamics simulations" could describe AI training to outside observers.

[Israel's Dimona facility, initially described as a textile plant, successfully managed US inspections in the 1960s](https://nsarchive.gwu.edu/briefing-book/nuclear-vault/2020-11-10/duplicity-deception-self-deception-israel-united-states-dimona-inspections-1964-65). Iraq reportedly dispersed centrifuge workshops across nondescript buildings. These examples show even physical infrastructure can be hidden; software-based AI training is inherently more concealable.

## Pathway Four: How Offshore Proxy Datacenters Operate

### The Pakistan-China Nuclear Model

During the 1980s-1990s, China reportedly provided Pakistan with nuclear assistance, according to various intelligence assessments and journalistic investigations. Both nations invoked sovereignty when confronted. Despite tracking from 1977, the international community proved powerless until Pakistan's 1998 nuclear tests.

A technologically advanced nation could offer a partner $2 billion in "infrastructure loans" for computing facilities. Constructed as 40 modular units with 200 GPUs each (each below 1e17 FLOP/s threshold), disguised as 5G edge nodes. With hardware outlays near $60 million [±2× depending on GPU generation] and compute costs of $40 million [±50% based on energy prices], GPT-4-class training could complete within seven months.

### Technical Implementation and Diplomatic Protection

Units could be designated for telecommunications or research. The host nation invokes sovereignty to block inspections. North Korea's missile proliferation despite MTCR demonstrates how state actors sustain prohibited technology transfer for decades. Trained weights could transfer through [diplomatic pouches, legally untouchable under the Vienna Convention on Diplomatic Relations](https://legal.un.org/ilc/texts/instruments/english/conventions/9_1_1961.pdf).

## Pathway × Detection × Countermeasure Matrix

| Attacker | Pathway | Cost (BOTEC) | Time | Key observables | Countermeasure | Residual risk |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| **Aligned lab in haven** | Regulatory flight | $10–100M | 6–12 mo | Sudden GPU imports; unusual DC buildouts; policy changes | Passports + secondary sanctions | Weights exfil via neutral CDNs/diplomatic channels |
| **Open-source/criminal** | GPU swarm | $30–60M | 8–12 mo | IXP bursts; grid micro-signatures; kernel mix; all-reduce patterns | Driver/HSM attestations; fusion watchfloor | Short-lived pop-up swarms; adversarial traffic shaping |
| **State lab** | Covert program | $100M–$1B | 6–18 mo | Sustained HPC load; procurement euphemisms; nighttime anomalies | Peer review → inspectorate; foundry leverage | Classification shields; national-security carve-outs |
| **Sponsor ↔ client** | Offshore proxies | $100–200M | 6–12 mo | "Edge" nodes with abnormal PUE; thermal signatures; GPU imports | Attested exports; insurer/bond gating | Sovereignty claims; diplomatic pouch transfers |

*Detection confidence: At 24h aggregation, we estimate our fusion watchfloor would flag ~90% of GPT-4-scale runs at 10% false positive rate across member-state grids, assuming 60% IXP coverage and hardware-rooted attestation on 80% of datacenter GPUs. These are author estimates based on analysis of detectable signatures across multiple channels.*

## The Cascade Effect: When One Domino Falls

The interaction of these pathways creates concerning dynamics:

- **Demonstration Effects**: Successful circumvention encourages others to follow
- **Investment Migration**: Capital flows to haven states after early successes
- **Technical Diffusion**: Distributed networks share techniques, accelerating capability
- **Justification Cascades**: Classified programs cite suspected violations to justify expansion
- **Partnership Proliferation**: Countries seek AI partners to avoid being left behind

All four pathways could activate simultaneously, creating a situation where the moratorium exists on paper while ASI development proceeds through multiple channels.

## Pre-Addressing the Three Biggest Pushbacks

### 1. Privacy and Civil Liberties

**The concern:** Compute passports enable mass surveillance.

**Our response:** Telemetry fields are minimal by design:

- Device ID (hashed)
- Coarse kernel class (GEMM/attention family, sampled every 30s)
- Aggregate FLOP count
- Instantaneous power
- Memory bandwidth

**No model weights, no data, no source code.**

**Access controls:**

- Only designated regulators can decrypt (rotating keys quarterly)
- Warrant required for individual device queries
- Independent auditor publishes false-positive rates quarterly
- Raw logs auto-delete after 90 days unless flagged
- Annual transparency report on access requests

### 2. Incumbent Entrenchment

**The concern:** Compliance costs lock out startups.

**Our response:** Tiered implementation with explicit cost analysis:

| Organization Size | Compliance Cost | Support Available |
| :---- | :---- | :---- |
| <$10M revenue | ~$50K/year | 80% subsidized, open-source tools |
| $10M-$100M | ~$200K/year | 50% subsidized, implementation support |
| $100M-$1B | ~$500K/year | Standard tools, priority support |
| >$1B | ~$2M/year | Custom integration, dedicated team |

All rules include 30-month sunset clauses requiring active renewal to prevent regulatory capture.

### 3. Sovereignty Concerns

**The concern:** Secondary sanctions violate national sovereignty.

**Our response:** We sanction *non-compliant runs*, not countries:

**Example 1:** Lab in Country A trains without passports → weights rejected by Visa/Swift-connected clouds → lab cannot monetize globally

**Example 2:** Country B refuses inspections → new GPU exports require attestation commitment → Country B can continue with existing hardware

The system creates incentives for voluntary compliance while respecting sovereignty boundaries.

## Toward Robust Solutions: Strengthening the Framework

To transform the moratorium from a jurisdiction-bounded freeze into a verifiable global regime, we propose ten interconnected enhancements:

### 1. Universal Cryptographic Attestation ("Compute Passports")

Treat every accelerator above 1e13 FLOP/s (training-relevant FP operations) like fissile material: embedded secure elements must sign device ID, instantaneous power, and rolling hash of executed kernels to an immutable Merkle log. [NVIDIA H100 GPUs already include attestation capabilities](https://developer.nvidia.com/blog/confidential-computing-on-h100-gpus-for-secure-and-trustworthy-ai/), proving technical feasibility.

### 2. Dynamic, Auto-Updating Risk Thresholds

Static FLOP caps age badly as algorithmic efficiency doubles every 16 months. The International AI Safety Commission should recalibrate thresholds quarterly, mirroring the [EU ETS cap-tightening approach](https://climate.ec.europa.eu/eu-action/carbon-markets/eu-emissions-trading-system-eu-ets/eu-ets-emissions-cap_en).

### 3. Extraterritorial Enforcement & Secondary Sanctions

Export licenses, foundry access, and dollar-clearing must hinge on compute passport compliance. Non-compliant entities face escalating sanctions up to full financial blocking.

### 4. Whole-of-Network Detection for Distributed Training

A fusion center must correlate passport logs, backbone flow patterns, and bulk-power telemetry. Even sub-threshold GPUs collectively create detectable signatures (all-reduce operations every tens of seconds, sustained power 5-15% above baseline).

### 5. International Inspectorate with Graduated Authority

**Phase 1 (Months 0-6):** Voluntary peer review among G7+ nations **Phase 2 (Months 6-12):** Reciprocal inspection agreements with strong export-control leverage
**Phase 3 (Months 12+):** Work toward "anywhere, anytime" authority modeled on [IAEA nuclear inspections](https://www.iaea.org/sites/default/files/publications/magazines/bulletin/bull34-1/34102451624.pdf)

*Note: Full UNSCOM-style authority required UN Security Council backing after military conflict; we start with achievable voluntary frameworks.*

### 6. Hardware Security Module (HSM) Weight Protection

Frontier weights must remain inside HSMs with checkpoint hashes published within 24 hours. Leaked models instantly reveal breach windows.

### 7. Kill-Switch Performance Bonds

Developers post surety proportional to risk. [Nuclear liability conventions mandate minimum coverage](https://www.iaea.org/sites/default/files/gc/gc48inf-5_en.pdf); AI bonds start at $250M minimum for frontier runs.

**Bond mechanics:**

- Posted before training starts
- Released upon successful safety audit
- Forfeit triggers: unauthorized deployment, weight leaks, safety violations
- Claims adjudicated by independent technical panel
- Funds support incident response and affected parties

### 8. Whistleblower Shield & Bounty Program

First insiders reporting unlicensed training earn 10-30% of monetary sanctions with legal immunity. [The SEC whistleblower program has paid over $2.2 billion](https://www.sec.gov/enforcement-litigation/whistleblower-program) and has awarded over $50 million in individual cases. We propose a similar framework with comparable incentives.

### 9. Conditional Infrastructure Aid & Pre-Certified Templates

Development loans require pre-certified datacenter blueprints with built-in telemetry. Low-capacity states gain infrastructure while agreeing to verification.

### 10. Sunset & Iteration Clause

All rules expire after 30 months unless renewed, forcing continual updates as capabilities evolve.

## From Theory to Practice: Phased 18-Month Implementation

### Phase 1: Emergency Response (Days 0-90) - Cloud & Hyperscaler Focus

**Week 1: Activate existing frameworks**

- Issue emergency orders for 1e24 FLOP run notices (14-day advance)
- Announce whistleblower bounties using existing SEC/FCA frameworks
- Strict liability penalties: $250M or 2% global turnover

**Week 2: Software attestation rollout (hyperscalers only)**

- AWS, Azure, GCP enable driver-level attestation by default
- Public API for attestation receipt verification
- Focus on managed services, not on-prem initially

**Week 4: Stand up fusion watchfloor v0.1**

- IXP + cloud provider flow logs + grid operators
- Monthly anomaly reports with detection confidence intervals
- Open metrics dashboard for transparency

### Phase 2: Market-Led Adoption (Months 3-6)

**Performance bonds go live**

- Insurers offer reduced premiums for attested + HSM-protected runs
- $250M minimum for 1e25 FLOP training
- Bonds cash out via independent adjudication panel

**Phased attestation expansion:**

- **(A) Hyperscalers + managed colos** → **(B) Government/HPC** → **(C) Enterprise** → **(D) Consumer**
- Each phase learns from previous rollout
- Open-source implementations for smaller players

### Phase 3: Financial Leverage (Months 6-12)

**Secondary sanctions framework**

- Foundry access requires attestation roadmap
- Visa/Mastercard/Swift block non-compliant weight monetization
- Graduated penalties preserve proportionality

**G7+ inspection pilot**

- Start with voluntary peer review
- Build trust through reciprocal access
- Document lessons for broader rollout

### Phase 4: Infrastructure Hardening (Months 12-18)

**On-die attestation in next silicon**

- Intel/TSMC/Samsung embed secure elements
- Backward compatibility with software attestation
- Cannot be disabled post-manufacture

**Conditional development aid**

- World Bank offers compute infrastructure loans
- Pre-certified designs with telemetry built-in
- Capacity building for verification compliance

## Technical Architecture: Making Detection Work

Frontier training creates distinctive signatures across multiple observable channels:

**Observable signatures with detection confidence (author estimates):**

- **Network:** All-reduce patterns every 10-60 seconds (95% confidence at IXPs)
- **Power:** Sustained draw 5-15% above baseline, especially nights/weekends (80% confidence)
- **Thermal:** Datacenter heat plumes visible in satellite imagery (60% confidence)
- **Kernels:** Distinctive matmul/attention sequences via attestation (99% confidence if deployed)
- **Procurement:** Bulk GPU purchases and "AI accelerator" euphemisms (70% confidence)

Combined multi-signal fusion enables ~90% detection probability within 24 hours for GPT-4-scale runs (author estimate based on analysis of signature visibility across channels).

## Specific Predictions (Falsifiable Within 24 Months)

1. **≥1 covert run above 1e25 FLOP detected** via power + IXP fusion in a member state by June 2026 (60% confidence)
2. **First distributed swarm achieving 1e24 FLOP** reported publicly by December 2025 (75% confidence)
3. **≥3 countries establish "AI Innovation Zones"** with explicit moratorium exemptions by March 2026 (70% confidence)
4. **Attestation adoption reaches 50% of datacenter GPUs** in US/EU by December 2025 (40% confidence)
5. **First $100M+ penalty issued** for unauthorized frontier training by September 2026 (50% confidence)

## Conclusion: The Window of Opportunity

The challenges outlined establish requirements for governance that might actually work. Twenty years might provide sufficient time to solve alignment challenges, but only if we address these circumvention pathways from the outset.

Success depends not on assuming compliance but anticipating creative non-compliance. We must design systems robust to partial adherence, fragmented enforcement, and determined adversaries. This means integrating verification into hardware, updating rules before obsolescence, and aligning economic incentives with safety goals.

The four pathways of ASI moratorium circumvention represent fundamental challenges even to sophisticated frameworks. Addressing them requires continuous innovation in AI safety governance.

Perfect control remains unachievable. The question is whether we can raise the bar high enough, quickly enough, to buy time for alignment research. The window narrows with each passing month.

**The path forward requires neither naive optimism nor paralyzing pessimism, but clear-eyed analysis coupled with determined action.** With the [EU AI Act now in force](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) and [America's AI Action Plan](https://www.whitehouse.gov/wp-content/uploads/2025/07/Americas-AI-Action-Plan.pdf) pulling in the opposite direction, the regulatory asymmetry creates immediate exploitable gaps.

*Begin with what's achievable: cloud-first attestation, fusion watchfloors, and whistleblower protections. Build momentum through voluntary adoption before mandates. The perfect must not be the enemy of the good when the stakes are existential.*

## Technical Glossary

### Computing Thresholds & Metrics

**FLOP (Floating-Point Operations)** - Standard unit for measuring computational work. One FLOP equals one arithmetic operation on decimal numbers. Distinguished from FLOPS (operations per second).

**1e25 FLOP** - Total compute budget for GPT-4-class training, adopted by EU AI Act as systemic risk threshold. This is cumulative compute, not throughput.

**Training-relevant FP FLOP/s** - Specifically FP16/BF16/FP8 operations used in training, measured via attested microbenchmarks. Not INT8 TOPS used in inference.

**1e17 FLOP/s** - Proposed licensing threshold for compute facilities (throughput, not total).

**1e13 FLOP/s** - Individual accelerator threshold for mandatory attestation.

### Security & Verification Infrastructure

**Compute passports** - Cryptographic attestation from embedded secure elements in GPUs, signing operations to immutable logs.

**Hardware Security Module (HSM)** - Tamper-resistant device storing model weights, requiring attestation for access.

**Merkle log** - Append-only cryptographic structure preventing retroactive falsification.

### Distributed Training Technical

**Gradient compression** - Bandwidth optimization achieving 270×-600× reduction ([DGC](https://arxiv.org/abs/1712.01887)), enabling training over 1 Gbps links.

**All-reduce operations** - Synchronized gradient exchanges creating detectable network patterns every 10-60 seconds.

**Asynchronous updates** - Protocol allowing nodes to contribute without tight synchronization, increasing fault tolerance.

### Historical Precedents

**Biopreparat** - Soviet biological weapons program (1974-1991) demonstrating large-scale covert dual-use programs.

**Dimona deception** - Israeli nuclear facility disguised as textile plant, managing US inspections 1960s.

**0G Labs/DiLoCoX** - December 2024 announcement of distributed 107B parameter training *(vendor-reported, under validation)*.

### Regulatory Frameworks

**EU AI Act** - Entered force August 2024, GPAI obligations from August 2025, 1e25 FLOP systemic risk threshold.

**America's AI Action Plan** - July 2025 framework emphasizing innovation and streamlined regulatory processes.

**Nuclear liability minimum** - IAEA conventions establish minimum coverage requirements, precedent for AI performance bonds.

**Secondary sanctions** - Penalties on third parties facilitating non-compliant runs, not blanket country sanctions.

## About This Research

This analysis represents our first major foray into AI governance research, emerging from a systematic red-teaming exercise that won first place in Apart Research's hackathon. As researchers new to governance, we bring an outsider's perspective that may catch vulnerabilities domain experts might miss.

We're continuing through Apart Lab Studio with mentorship from the ControlAI team, focusing on technical verification mechanisms implementable without consensus, economic incentives favoring compliance, and adaptive governance evolving with the technology.

*For questions, critiques, or collaboration: [contact information]*