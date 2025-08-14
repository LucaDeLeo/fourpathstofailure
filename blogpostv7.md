# Perfect Implementation Isn't Enough: Four Paths Around an ASI Moratorium Already Being Walked
## A 2025 Reality Check with Historical Precedents and Technical Validation

## What This Post Is About

Imagine trying to pause the development of superintelligent AI worldwide—a technology that could transform or end civilization. Even if every nation agreed (unlikely), could we actually enforce it?

"A Narrow Path" proposes humanity's most ambitious technological restraint: a 20-year moratorium on artificial superintelligence (ASI), enforced through compute licensing, capability restrictions, and international treaties. But what if perfect global cooperation still isn't enough?

This post examines four ways determined actors could circumvent such a moratorium, based on historical precedents and current technical capabilities. We'll explore how lessons from nuclear proliferation, bioweapons programs, and today's AI landscape reveal fundamental enforcement challenges.

**Key terms you'll encounter:**
- **ASI (Artificial Superintelligence)**: AI systems substantially surpassing human intelligence across all domains
- **FLOP**: Floating-point operations—a measure of computational work (1e25 = roughly GPT-4-scale training, now an EU systemic risk threshold)
- **Compute moratorium**: A proposed pause on training AI models above certain computational thresholds
- **GPU swarms**: Networks of consumer graphics cards working together instead of supercomputers

## Reader Prerequisites

This post assumes:
- Basic familiarity with AI development (what training a model means)
- Interest in AI governance challenges
- No specialized technical knowledge required—we'll explain terms as needed

## Origin & Credibility

This analysis emerged from winning first place in [Apart Research's "Red-Teaming the Narrow Path" hackathon](https://apartresearch.com/project/four-paths-to-failure-red-teaming-asi-governance-se53), where we systematically stress-tested proposed AI governance frameworks through adversarial thinking. We're continuing this work through Apart Lab Studio with mentorship from the ControlAI team. This enhanced version integrates 50+ peer-reviewed sources, congressional testimony from program insiders, and real-time evidence from 2024-2025.

*Epistemic status: We're governance research newcomers who approached this problem through systematic adversarial analysis. While our fresh perspective may catch overlooked vulnerabilities, we defer to domain experts on political feasibility and implementation details.*

**Ethical note**: This is governance red-teaming intended to strengthen AI safety measures by identifying vulnerabilities before they're exploited. We detail circumvention methods not to enable them, but to ensure robust countermeasures are developed. Think of this as penetration testing for global AI governance.

## TL;DR: Even Perfect Agreement Faces Four Proven Circumvention Paths

**The challenge**: A proposed 20-year moratorium on training AI above 10²⁵ FLOPs (GPT-4 scale) faces four actively-exploited circumvention paths: **jurisdiction shopping** (AI havens), **distributed training** (GPU swarms), **secret programs** (classification shields), and **proxy partnerships** (deniable development).

**The evidence**: U.S. states already compete for AI investment while the EU enforces compute thresholds. DiLoCoX achieves 107B parameter training on home internet. Soviet bioweapons hid 65,000 employees for 19+ years. China-Pakistan tech transfers continue despite decades of sanctions.

**The countermeasures**: Compute passports, performance bonds, whistleblower bounties, and fusion detection could raise the bar—but history shows determined actors find ways around even nuclear controls. Success requires anticipating creative non-compliance, not assuming it away.

## Where We Stand: August 2025

As you read this, the dynamics we're describing aren't hypothetical:

- **Jurisdiction Shopping**: States already compete aggressively for AI investment, with governors warning that "burdensome frameworks could drive AI talent and capital to another state"
- **Distributed Training**: DiLoCoX achieves 107B parameter training on consumer internet with 357× speedup
- **Hardware Reality**: NVIDIA H100s (flagship AI chips) have confidential computing capabilities—but ship with CC features **disabled by default** in standard deployments
- **Proliferation Continues**: Chinese entities sanctioned this year for missile tech transfers to Pakistan
- **Regulatory Fragmentation**: EU AI Act live with 1e25 FLOP threshold; U.S. pursues aggressive deregulation

We're not warning about future risks. We're documenting current reality.

## The Governance Paradox of Transformative AI

What if we achieved the impossible: perfect global cooperation on AI safety, and it still wasn't enough?

Even the prospect of AI governance faces immediate resistance. As states race to attract AI investment in 2025, governors warn that "burdensome frameworks could drive AI talent and capital to another state." Any future moratorium proposal would face this same dynamic amplified globally—we're watching the precursors to jurisdiction shopping unfold in real-time, and history shows us exactly where this leads.

## Understanding the Moratorium Proposal

[The Narrow Path's Phase 0](https://pdf.narrowpath.co/A_Narrow_Path.pdf) proposes comprehensive regulatory framework including:

- **Training licenses** for AI models requiring more than 10^25 FLOP (roughly GPT-4 scale compute)
- **Compute licenses** for cloud providers operating above 10^17 FLOP/s (about 1,000 high-end GPUs)
- **Application licenses** for deploying new AI systems
- **Prohibited capabilities**: No AI improving AI, no AI breaking containment, no unbounded AI systems

The proposal assumes we can monitor data centers' energy consumption and intervene within 12 days if violations are detected. But as we'll show, each assumption has exploitable weaknesses that history proves will be exploited.

## The Current Regulatory Landscape

As we write this in August 2025, the global AI governance landscape is fragmenting rapidly:

- **Europe**: [EU AI Act entered force August 2024](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai), establishing the world's first comprehensive AI regulatory framework with [10^25 FLOP systemic risk threshold](https://ec.europa.eu/commission/presscorner/detail/en/qanda_21_1683)
- **United States**: [America's AI Action Plan (July 2025)](https://www.whitehouse.gov/wp-content/uploads/2025/07/Americas-AI-Action-Plan.pdf) emphasizes innovation and streamlined regulation
- **The Gap**: This divergence creates precisely the regulatory asymmetry that determined actors are already beginning to exploit

## Pathway One: How Regulatory Flight Happens

### The Race to the Bottom Is Already Running

History doesn't just rhyme—it provides the playbook. When the United States restricted federal funding for embryonic stem cell research in 2001, Wisconsin didn't comply. Instead, it created WiCell Research Institute as an explicit "safe haven for the advancement of stem cell research in the politically charged environment." 

The result? WiCell trained over 800 scientists globally and hosted the National Stem Cell Bank, becoming the epicenter of research the federal government tried to stop.

The pattern repeats across technologies:
- **Crypto**: FTX relocated to Bahamas in 2021 for friendlier regulation
- **Data privacy**: Facebook modified terms to evade European laws
- **Labor laws**: Uber classified workers as non-employees to sidestep regulations

### The AI Innovation Zone Scenario

Small nations could establish "AI Innovation Zones" tomorrow, offering:
- Tax holidays and sovereign protection
- Instant global deployment through CDN endpoints
- Diplomatic immunity for trained model weights

The precedent? The [A.Q. Khan network operated for decades](https://core.ac.uk/download/pdf/36732689.pdf) despite export controls, using shell companies in Dubai and Malaysia. When faced with choosing between a moratorium keeping them technologically dependent or hosting AI development bringing billions in investment, the choice is predetermined.

Academic research documents the precise mechanics: Pollman (2019) defines jurisdiction shopping as "strategic maneuvering by firms to exploit gaps between regulatory regimes." The four-phase pattern is consistent:

1. Major jurisdiction imposes restrictions
2. Sub-national or allied jurisdictions create "havens"
3. Capital and talent migrate rapidly
4. Original restrictions become meaningless

If even U.S. states in 2025 refuse coordination for fear of losing AI investment to neighbors, how can we expect global coordination among nations with vastly different economic incentives?

## Pathway Two: How GPU Swarms Scale

### From Theory to Achieved Reality

Training frontier AI models on distributed consumer hardware isn't just feasible—it's happening now.

**The breakthrough**: [0G Labs with China Mobile announced](https://thedefiant.io/news/press-releases/0g-labs-achieves-breakthrough-in-decentralized-ai-training-with-100-billion-parameters) their DiLoCoX framework in 2025, achieving:
- 357× communication efficiency improvement (not end-to-end speedup)
- Successfully trained 107 billion parameter model
- Using only 1 Gbps home internet connections
- Across decentralized consumer hardware clusters

*Note: DiLoCoX results come from startup announcements, not peer-reviewed publications. However, the mechanism is consistent with established research like Deep Gradient Compression (270-600× communication reduction).*

### The Math of Distributed Training

Let's break down what's possible with today's technology:

**Scenario Analysis for 10²⁵ FLOP Training**:

| Scenario | GPUs | Effective TFLOP/s per GPU | Overhead | Raw Days | Adjusted Days | Cost Estimate |
|----------|------|---------------------------|----------|----------|---------------|---------------|
| **Conservative** | 50,000 | 40 (verified throughput) | 40% | 58 | 81-97 | $60-80M |
| **Moderate** | 50,000 | 70 (mixed precision) | 30% | 33 | 43-52 | $40-60M |
| **Aggressive** | 75,000 | 100 (peak utilization) | 20% | 15 | 18-35 | $30-50M |

**Key assumptions**:
- GPUs: RTX 4090 class or better
- DiLoCoX's 357× communication reduction enables commodity internet
- Costs include: rental/grey market hardware + bandwidth + coordination overhead
- Lower bound assumes some illicit access or state subsidy

### The Infrastructure Already Exists

[Folding@home during COVID-19](https://foldingathome.org/2021/01/05/2020-in-review-and-happy-new-year-2021/) proved the scale possible:
- **280,000 GPUs** coordinated globally
- **4.8 million CPU cores** contributing
- **1.5 exaFLOPS** sustained (exceeding top 100 supercomputers combined)
- All volunteer-driven with zero financial incentive

Now imagine the same infrastructure, but:
- Financially incentivized (cryptocurrency or direct payment)
- Optimized with DiLoCoX algorithms (357× speedup)
- Purpose-built for AI training
- State-sponsored with unlimited funding

The distributed training revolution timeline:
- **2018**: Deep Gradient Compression achieves 270-600× communication reduction
- **2020**: Folding@home aggregates 280,000 volunteer GPUs
- **2023**: Evaluation shows 4× speedup over standard distributed training
- **2025**: DiLoCoX achieves 357× communication reduction, trains 107B parameters on consumer internet

The infrastructure for distributed training doesn't need to be built—it already exists.

## Pathway Three: How Covert State Programs Hide

### From the Horse's Mouth: A Bioweapons Chief Confesses

We don't need to speculate about covert programs—we have testimony. In 2001, Dr. Ken Alibek sat before the U.S. House of Representatives. As the former First Deputy Chief of Biopreparat, he wasn't speculating—he ran one:

> "The Soviet Union continued an offensive BW program after signing the 1972 BWC... When trilateral inspections were conducted in 1991, the program was still active, and the Soviets covered up the evidence as best they could."

The numbers are staggering:
- **65,000 employees** at peak operation
- **52 secret sites** disguised as civilian facilities
- **20+ years** of successful concealment despite treaty obligations
- **Only 2 defectors** (out of 65,000) revealed the truth

The 1979 Sverdlovsk anthrax leak killed 68+ civilians, yet the program remained hidden until 1989. For AI governance, the parallel is chilling: Just as the Biological Weapons Convention coincided with the biotechnology revolution, an AI moratorium would coincide with the deep learning revolution.

### The Art of Dual-Use Deception

Modern AI facilities have even better cover than bioweapons labs:
- **Climate modeling** requires identical hardware and algorithms
- **Pharmaceutical research** uses the same transformer architectures
- **Financial modeling** needs comparable compute scales
- **Academic research** provides perfect publication cover

Countries already operate exascale supercomputers for these purposes. Repurposing requires only new software. Staff could continue using existing terminology: "molecular dynamics simulations" could describe AI training to outside observers.

[Israel's Dimona nuclear facility](https://nsarchive.gwu.edu/briefing-book/nuclear-vault/2020-11-10/duplicity-deception-self-deception-israel-united-states-dimona-inspections-1964-65), initially described as a textile plant, successfully managed US inspections in the 1960s using fake control rooms and false walls. These examples show even physical infrastructure can be hidden; software-based AI training is inherently more concealable.

## Pathway Four: How Offshore Proxy Datacenters Operate

### The Proliferation That Never Stopped

The Congressional Research Service reported in 2025—yes, this year—that Chinese entities continue supplying missile-applicable items to Pakistan's ballistic missile program, triggering U.S. sanctions. The nuclear assistance that began in the 1980s hasn't stopped; it's evolved.

China reportedly provided Pakistan with:
- 50 kg of weapons-grade uranium (1982)
- Complete nuclear weapon designs
- Ongoing missile technology (still active 2025)

Despite tracking since 1977, the international community proved powerless until Pakistan's 1998 nuclear tests—16 years after receiving Chinese uranium.

### The Three Tactics of Treaty Circumvention

China's nuclear assistance to Pakistan reveals three tactics that translate perfectly to AI:

**1. The Fait Accompli**
When China sold reactors to Pakistan after joining the Nuclear Suppliers Group, it simply "grandfathered" them under previous agreements. The NSG acquiesced.
*AI parallel*: "The training run is 90% complete."

**2. The Dual Justification**
Every facility has a civilian cover story. Dimona was a "textile plant." Pakistan's enrichment was for "energy independence."
*AI parallel*: Every datacenter is for "climate modeling" until proven otherwise.

**3. The Strategic Triangle**
China used Pakistan to counterbalance India. The client gets capability, the sponsor gets deniability, the rival gets checked.
*AI parallel*: Proxy relationships aren't about technology—they're about strategic competition.

### Technical Implementation

A technologically advanced nation could offer a partner:
- $2 billion in "infrastructure loans" for computing facilities
- 40 modular units with 200 GPUs each (each below detection threshold)
- Disguised as 5G edge nodes or research centers
- GPT-4-class training complete within seven months

Trained weights could transfer through [diplomatic pouches, which are inviolable under Vienna Convention Article 27](https://legal.un.org/ilc/texts/instruments/english/conventions/9_1_1961.pdf). *Note: While pouches cannot be opened or detained, they must contain official items—abuse would violate Article 27(4), though practical inspection barriers remain.*

## Detection vs. Reality: A Sobering Matrix

| Attacker | Pathway | Cost | Time | Key Signs | Countermeasure | What Still Gets Through |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| **Aligned lab in haven** | Regulatory flight | $10–100M | 6–12 mo | Sudden GPU imports; unusual DC buildouts | Passports + sanctions | Weights via CDNs/diplomatic channels |
| **Open-source/criminal** | GPU swarm | $30–80M | 18-97 days* | Network bursts; power anomalies | Driver attestations | Pop-up swarms; traffic masking |
| **State lab** | Covert program | $100M–$1B | 6–18 mo | Sustained HPC load; procurement patterns | Inspections + whistleblowers | Classification shields |
| **Sponsor ↔ client** | Offshore proxies | $100–200M | 6–12 mo | "Edge" nodes with high power use | Export controls | Sovereignty claims |

*Range depends on GPU efficiency assumptions—see scenario table

*Detection confidence: ~90% of GPT-4-scale runs detectable within 24h at 10% false positive rate, assuming 60% network coverage and 80% hardware attestation. These are author estimates.*

## The Defection Cascade: A Mathematical Certainty

Regulatory arbitrage research (Pollman, 2019) documents how tech companies create systemic pressure forcing jurisdictional competition:

**Predicted Timeline for AI Moratorium Cascade**:
- **Month 0-3**: Major powers agree to moratorium
- **Month 3-6**: Small nation announces "AI Innovation Zone"
- **Month 6-9**: 3-5 nations follow with competitive offerings
- **Month 9-12**: Major power claims "defensive exception"
- **Month 12-18**: Moratorium exists in name only

All four pathways could activate simultaneously, creating a situation where the moratorium exists on paper while ASI development proceeds through multiple channels.

## Pre-Addressing the Three Biggest Pushbacks

### 1. "But compute passports enable mass surveillance!"

**Our response:** The telemetry is minimal by design:
- Device ID (hashed)
- Coarse kernel class (type of computation, sampled every 30s)
- Aggregate compute count
- Power usage

**No model weights, no data, no source code.**

Access requires:
- Warrant for individual queries
- Quarterly key rotation
- Auto-deletion after 90 days
- Annual transparency reports

### 2. "This locks out startups!"

**Our response:** Tiered implementation with subsidies:

| Organization Size | Compliance Cost | Support Available |
| :---- | :---- | :---- |
| <$10M revenue | ~$50K/year | 80% subsidized, open-source tools |
| $10M-$100M | ~$200K/year | 50% subsidized, implementation support |
| >$1B | ~$2M/year | Custom integration |

All rules include 30-month sunset clauses to prevent regulatory capture.

### 3. "Secondary sanctions violate sovereignty!"

**Our response:** We sanction non-compliant *runs*, not countries:
- Lab trains without passports → weights rejected by global clouds
- Country refuses inspections → new GPU exports require attestation
- Creates incentives for voluntary compliance while respecting boundaries

## Toward Robust Solutions: Ten Interconnected Enhancements

### 1. Universal Cryptographic Attestation ("Compute Passports")
Treat every GPU above gaming-level (1e13 FLOP/s) like fissile material. [NVIDIA H100s already include attestation capability](https://developer.nvidia.com/blog/confidential-computing-on-h100-gpus-for-secure-and-trustworthy-ai/)—but CC features are **off by default** in common fleet deployments unless explicitly enabled by operator policy.

### 2. Dynamic Risk Thresholds
Static FLOP caps age badly as algorithms improve. Quarterly recalibration needed, mirroring [EU carbon credit tightening](https://climate.ec.europa.eu/eu-action/carbon-markets/eu-emissions-trading-system-eu-ets/eu-ets-emissions-cap_en).

### 3. Secondary Sanctions
Export licenses, chip foundry access, and banking must require compute passport compliance. Non-compliant entities face escalating sanctions.

### 4. Network Detection Fusion
Correlate passport logs, internet traffic patterns, and power grid telemetry. AI training creates distinctive "IO storms" every 10-60 seconds, detectable at internet exchange points.

### 5. International Inspectorate
- **Phase 1 (Months 0-6)**: Voluntary peer review among G7+ nations
- **Phase 2 (Months 6-12)**: Reciprocal inspection agreements
- **Phase 3 (Months 12+)**: Work toward "anywhere, anytime" authority

*Note: IAEA safeguards are designed primarily to **detect and deter** diversion; they often function as warning systems that identify violations after they occur rather than preventing them entirely.*

### 6. Hardware Security for Model Weights
Frontier weights must remain inside secure hardware with checkpoint hashes published within 24 hours. Leaked models instantly reveal breach windows.

### 7. Performance Bonds
Developers post $250M+ bonds before training, forfeit for violations. [Nuclear liability conventions](https://www.iaea.org/sites/default/files/gc/gc48inf-5_en.pdf) provide precedent.

### 8. Whistleblower Bounties
10-30% of monetary sanctions for first insider reports. [SEC program has paid $2.2B](https://www.sec.gov/enforcement-litigation/whistleblower-program) with awards over $50M. In 2021, tips came from 99 countries.

**Why insiders matter more than inspectors**:
- Biopreparat: 19+ years hidden, revealed by 2 defectors (of 65,000)
- Pakistan nuclear: 16+ years hidden, exposed by network leaks
- Average covert program: 15+ years undetected
- Percentage of workforce needed to expose: <0.01%

### 9. Conditional Infrastructure Aid
Development loans require pre-certified datacenter designs with built-in telemetry. Low-capacity states gain infrastructure while accepting verification.

### 10. Sunset Clauses
All rules expire after 30 months unless renewed, forcing continual updates as capabilities evolve.

## The Countermeasure Reality Check

Our proposed countermeasures have precedent—both encouraging and sobering:

**Compute Passports: Ready but Requires Political Will**
- ✅ H100 hardware already includes attestation capability
- ⚠️ Requires opt-in activation—political mandate needed
- ❌ Black market GPUs remain untracked

**International Inspectorate: Detection, Not Prevention**
- ✅ IAEA model shows verification is possible
- ⚠️ "Cannot prevent diversion... ex post facto warning system"
- ❌ Resource requirements immense

**Whistleblower Bounties: Powerful but Limited**
- ✅ SEC program generated $2.2B awards, $5B recoveries
- ✅ Global reach: tips from 99 countries
- ❌ Authoritarian states can eliminate whistleblowers

**Network Detection: Ongoing Arms Race**
- ✅ AI training creates detectable "IO storms"
- ⚠️ Adversarial traffic masking evolving rapidly
- ❌ Detection improvements lag circumvention innovation

## From Theory to Practice: The 18-Month Roadmap

### Phase 1: Emergency Response (Days 0-90)
**Focus: Cloud providers and hyperscalers**
- Week 1: Activate 1e24 FLOP run notices, announce whistleblower bounties
- Week 2: Enable driver attestation on AWS, Azure, GCP
- Week 4: Stand up fusion watchfloor v0.1

### Phase 2: Market Adoption (Months 3-6)
**Focus: Financial incentives**
- Performance bonds go live ($250M minimum)
- Phased attestation: Hyperscalers → Government → Enterprise
- Open-source tools for smaller players

### Phase 3: Financial Leverage (Months 6-12)
**Focus: International coordination**
- Secondary sanctions framework
- G7+ inspection pilot
- Graduated penalties

### Phase 4: Infrastructure Hardening (Months 12-18)
**Focus: Long-term solutions**
- On-die attestation in next silicon generation
- Conditional development aid tied to compliance
- Pre-certified datacenter designs

## Specific Predictions (Falsifiable Within 24 Months)

1. **≥1 covert run above 10²⁵ FLOP detected** via power/network fusion by June 2026 (75% confidence)
2. **First distributed swarm achieving 10²⁴ FLOP** reported by December 2025 (90% confidence)
3. **≥3 countries establish "AI Innovation Zones"** with exemptions by March 2026 (85% confidence)
4. **Attestation reaches 50% datacenter GPUs** in US/EU by December 2025 (30% confidence)
5. **First $100M+ penalty** for unauthorized training by September 2026 (50% confidence)

## What Would Change Our Mind

**We would significantly update our assessment if:**

- **≥70% of datacenter GPUs** in US/EU run with verifiable attestation enabled AND internet exchange points adopt standardized training-pattern detection → *Detection confidence for Pathway 2 rises from 40% to 65%*

- **Robust secondary sanctions** achieve >80% compliance on chip exports to non-participating nations → *Pathway 4 (proxy partnerships) becomes 3-5× more expensive*

- **Algorithmic breakthroughs** reduce compute requirements by >100× while maintaining capability → *All pathways become easier; thresholds need complete recalibration*

- **Successful precedent** emerges of international tech governance working at scale (e.g., meaningful climate commitments with verified compliance) → *Updates our prior on coordination feasibility*

- **DiLoCoX-style frameworks** fail to scale beyond 200B parameters due to fundamental limitations → *Pathway 2 timeline extends by 2-3 years*

## Conclusion: The Window of Opportunity

The four pathways of ASI moratorium circumvention represent fundamental challenges validated by decades of precedent and contemporary evidence. Perfect control remains unachievable—history proves this repeatedly. The question is whether we can raise the bar high enough, quickly enough, to buy time for alignment research.

Success depends not on assuming compliance but anticipating creative non-compliance. We must:
- Integrate verification into hardware (H100s already have it)
- Update rules before obsolescence
- Align economic incentives with safety goals

With the [EU AI Act now in force](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) and [America's AI Action Plan](https://www.whitehouse.gov/wp-content/uploads/2025/07/Americas-AI-Action-Plan.pdf) pulling opposite directions, regulatory asymmetry creates immediate exploitable gaps—gaps that actors are already beginning to probe.

**The path forward requires neither naive optimism nor paralyzing pessimism, but clear-eyed analysis coupled with determined action.** Begin with what's achievable: cloud-first attestation, fusion watchfloors, and whistleblower protections. Build momentum through voluntary adoption before mandates. 

The perfect must not be the enemy of the good when the stakes are existential. The window narrows with each passing month.

## About This Research

This analysis represents our first major foray into AI governance research, emerging from a systematic red-teaming exercise that won first place in Apart Research's hackathon. As researchers new to governance, we bring an outsider's perspective that may catch vulnerabilities domain experts might miss.

This enhanced version integrates 50+ peer-reviewed sources, congressional testimony from program insiders who ran covert WMD programs, and real-time evidence from 2024-2025 showing these dynamics actively unfolding.

We're continuing through Apart Lab Studio with mentorship from the ControlAI team, focusing on technical verification mechanisms implementable without consensus, economic incentives favoring compliance, and adaptive governance evolving with the technology.

*For questions, critiques, or collaboration: [contact information]*

---

## Confidence Levels by Core Claims

*For transparency, here's our confidence in key assertions:*

- **GPU swarms can reach 1e25 FLOP in <35-60 days for <$30M-60M**: 85%
  - *Crux*: DiLoCoX demonstrated 357× speedup on 107B parameters (2025)
- **Haven states could field offshore proxies within 12 months**: 75%
  - *Crux*: Ongoing China-Pakistan transfers prove model viability
- **Watchfloor can detect GPT-4-scale runs within 24h at ≤10% FPR**: 40%
  - *Crux*: IXP coverage + kernel attestation adoption
- **Covert state programs could operate undetected for 6+ months**: 90%
  - *Crux*: Biopreparat operated 19+ years with 65,000 employees
- **Secondary sanctions could reduce haven state participation**: 50%
  - *Crux*: Enforcement will vs sovereignty claims

## Technical Glossary

**Core Concepts**
- **ASI (Artificial Superintelligence)**: AI systems substantially surpassing human cognitive capabilities across all domains
- **FLOP**: Floating-point operations—one arithmetic operation on decimal numbers
- **1e25 FLOP**: Total compute for GPT-4-class training (10,000,000,000,000,000,000,000,000 operations)
- **GPU**: Graphics Processing Unit—specialized chips originally for gaming, now powering AI

**Governance Terms**
- **Compute passports**: Cryptographic tracking built into AI chips (like serial numbers for GPUs)
- **Performance bonds**: Insurance deposits required before training large models
- **Secondary sanctions**: Penalties on third parties helping violators
- **Jurisdiction shopping**: Moving operations to countries with weaker regulations

**Technical Infrastructure**
- **DiLoCoX**: 2025 breakthrough enabling AI training on home internet connections
- **IXP (Internet Exchange Point)**: Major internet traffic hubs where detection could occur
- **All-reduce operations**: Synchronized data exchanges creating detectable network patterns
- **HSM (Hardware Security Module)**: Tamper-proof device storing AI model weights

**Historical Precedents**
- **Biopreparat**: Soviet bioweapons program (65,000 employees, hidden 19+ years)
- **WiCell**: Wisconsin stem cell "safe haven" defying federal restrictions
- **Dimona**: Israeli nuclear facility disguised as textile plant
- **A.Q. Khan network**: Pakistan's nuclear proliferation network, operated decades despite controls