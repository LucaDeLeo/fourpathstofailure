# Perfect Implementation Isn't Enough: Four Paths Around an ASI Moratorium Already Being Walked
## A 2025 Reality Check with Historical Precedents and Technical Validation

**TL;DR: Four paths around an ASI moratorium - all actively being explored**

1. **Jurisdiction shopping** in "AI innovation zones" - already happening as states compete for AI investment
2. **Distributed GPU swarms** staying below per-device thresholds - DiLoCoX achieved 107B parameter training in 2025
3. **Covert state programs** behind classification shields - historical precedent from 65,000-employee Biopreparat
4. **Offshore proxy datacenters** under sovereignty protection - China-Pakistan transfers continue in 2025

**Countermeasures:** cryptographic **compute passports** (H100s already have the hardware), whistleblower awards (SEC model: $2.2B paid, 10–30% of sanctions), **performance bonds**, and **anywhere-anytime inspections** (though IAEA admits these are "ex post facto warning systems").

**Why now:** [EU AI Act is live](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) with a [1e25 FLOP trigger](https://ec.europa.eu/commission/presscorner/detail/en/qanda_21_1683); the U.S. is pushing deregulatory growth via [America's AI Action Plan](https://www.whitehouse.gov/wp-content/uploads/2025/07/Americas-AI-Action-Plan.pdf), creating exploitable asymmetry. The regulatory divergence isn't theoretical - it's today's reality.

**What happens next quarter:** • **Run-notice pilot at 1e24 FLOP** in coalition jurisdictions; **strict-liability** penalties posted • **Cloud-first driver attestation default-on** (hyperscalers only), with **public attestation receipts** • **Fusion watchfloor v0.1**: IXPs + cloud flow logs + bulk-power anomalies (monthly anomaly report) • **Whistleblower awards** aligned to SEC framework (10–30% of monetary sanctions, which has paid out $2.2B in awards to date)

**Origin & Methodology:** This analysis emerged from winning first place in [Apart Research's "Red-Teaming the Narrow Path" hackathon](https://apartresearch.com/project/four-paths-to-failure-red-teaming-asi-governance-se53), where we systematically stress-tested proposed AI governance frameworks through adversarial thinking. We're continuing this work through Apart Lab Studio with mentorship from the ControlAI team. This enhanced version integrates 50+ peer-reviewed sources, congressional testimony from program insiders, and real-time evidence from 2024-2025.

## Where We Stand: August 2025

As you read this, the dynamics we're describing aren't hypothetical:

- **Jurisdiction Shopping**: States already compete aggressively for AI investment, with governors warning that "burdensome frameworks could drive AI talent and capital to another state"
- **Distributed Training**: DiLoCoX achieves 107B parameter training on consumer internet with 357× speedup
- **Hardware Reality**: NVIDIA H100s with built-in attestation ship globally—in "CC-Off" mode by default
- **Proliferation Continues**: Chinese entities sanctioned this year for missile tech transfers to Pakistan
- **Regulatory Fragmentation**: EU AI Act live with 1e25 FLOP threshold; U.S. pursues aggressive deregulation

We're not warning about future risks. We're documenting current reality.

## Introduction: The Governance Paradox of Transformative AI

What if we achieved the impossible: perfect global cooperation on AI safety, and it still wasn't enough?

Even the prospect of AI governance faces immediate resistance. As states race to attract AI investment in 2025, governors warn that "burdensome frameworks could drive AI talent and capital to another state." Any future moratorium proposal would face this same dynamic amplified globally—we're watching the precursors to jurisdiction shopping unfold in real-time, and history shows us exactly where this leads.

*Epistemic status: We're governance research newcomers who approached this problem through systematic adversarial analysis. While our fresh perspective may catch overlooked vulnerabilities, we defer to domain experts on political feasibility and implementation details. Our confidence is highest on technical circumvention methods (based on documented capabilities and peer-reviewed research) and lower on international coordination dynamics.*

*Confidence by claim:*

- **GPU swarms can reach 1e25 FLOP in <35-60 days for <$30M-60M**: 85%, crux: DiLoCoX demonstrated 357× speedup on 107B parameters (2025)
- **Haven states could field offshore proxies within 12 months**: 75%, crux: ongoing China-Pakistan transfers prove model viability
- **Watchfloor can detect GPT-4-scale runs within 24h at ≤10% FPR**: 40%, crux: IXP coverage + kernel attestation adoption
- **Covert state programs could operate undetected for 6+ months**: 90%, crux: Biopreparat operated 19+ years with 65,000 employees
- **Secondary sanctions could reduce haven state participation**: 50%, crux: enforcement will vs sovereignty claims

We face a documented reality. Even as international bodies converge on sophisticated regulatory frameworks for artificial superintelligence (ASI), a troubling pattern emerges from decades of dual-use technology control: the very nature of AI development may make it ungovernable through traditional means.

The [Narrow Path's proposed twenty-year moratorium](https://pdf.narrowpath.co/A_Narrow_Path.pdf) on ASI development represents humanity's most ambitious attempt at coordinated technological restraint. Yet beneath the surface of this comprehensive proposal lies a troubling reality documented across 50+ peer-reviewed sources and congressional testimony: the characteristics that make AI development dangerous also make it uniquely resistant to control mechanisms.

This analysis examines four distinct pathways through which determined actors could circumvent even the most comprehensive ASI moratorium. Each pathway could enable GPT-4-scale training within weeks to months, exploiting fundamental weaknesses in our current governance paradigms—weaknesses that history shows have been consistently exploited.

## The Current Regulatory Landscape

As we write this in August 2025, the global AI governance landscape is fragmenting rapidly. The [EU AI Act, which entered force in August 2024](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai), establishes the world's first comprehensive AI regulatory framework, including the [1e25 FLOP threshold for systemic risk](https://ec.europa.eu/commission/presscorner/detail/en/qanda_21_1683) that features prominently in moratorium proposals. GPAI obligations under the Act apply from August 2, 2025. Meanwhile, [America's AI Action Plan (July 2025)](https://www.whitehouse.gov/wp-content/uploads/2025/07/Americas-AI-Action-Plan.pdf) takes a starkly different approach, emphasizing innovation and competitiveness while streamlining regulatory processes. This divergence creates precisely the regulatory asymmetry that determined actors are already beginning to exploit.

## The Moratorium's Achilles Heel: Understanding the Enforcement Challenge

The [Narrow Path's Phase 0](https://pdf.narrowpath.co/A_Narrow_Path.pdf) proposes a comprehensive regulatory framework including: training licenses for runs above 1e25 FLOP (total training compute), compute licenses for cloud providers above 1e17 FLOP/s, application licenses for new deployments, and prohibition of specific dangerous capabilities. The proposal includes monitoring of data centers' energy consumption with approximately 12-day intervention windows.

**Critical metric clarification:** All thresholds refer to **training-relevant FP FLOP/s measured via attested microbenchmarks**, not INT8 TOPS or other metrics. This distinction matters because consumer NPUs advertise INT8 performance while training requires FP16/BF16/FP8 precision.

While the framework proposes defense-in-depth approaches with multiple layers of oversight, the four circumvention pathways explored here reveal how determined actors could exploit gaps between jurisdictions, leverage distributed infrastructure, and abuse dual-use technologies to undermine these safeguards. Each pathway is not theoretical—we have historical precedent and contemporary evidence for all four.

## Pathway One: How Regulatory Flight Happens

### The Race to the Bottom Is Already Running

When the United States restricted federal funding for embryonic stem cell research in 2001, Wisconsin didn't comply—it created WiCell Research Institute as an explicit "safe haven for the advancement of stem cell research in the politically charged environment." The result? WiCell trained over 800 scientists globally and hosted the National Stem Cell Bank, becoming the epicenter of research the federal government tried to stop.

The pattern repeats: FTX relocated its headquarters to the Bahamas in September 2021 amid China's crypto crackdown and for a friendlier regulatory environment. [Binance allegedly instructed US customers to use VPNs to bypass restrictions](https://www.cftc.gov/media/8351/%20enfbinancecomplaint032723/download) while maintaining plausible deniability.

### The Regulatory Arbitrage Playbook

Academic research has documented the precise mechanics of how jurisdiction shopping operates. Pollman (2019) defines it as "strategic maneuvering by firms to exploit gaps or differences between regulatory regimes," noting how Facebook modified its terms to evade European privacy laws and Uber classified workers as non-employees to sidestep labor regulations.

The pattern is consistent across technologies:
- **Phase 1**: Major jurisdiction imposes restrictions (US stem cell funding, 2001)
- **Phase 2**: Sub-national or allied jurisdictions create "havens" (California's Proposition 71, establishing constitutional right to stem cell research with $3 billion allocation, 2004)
- **Phase 3**: Capital and talent migrate rapidly (WiCell hosts National Stem Cell Bank, trains 800+ scientists)
- **Phase 4**: Original restrictions become meaningless (stem cell research continues globally)

As Froomkin (1997) presciently warned about the internet: "A single country can do little to prevent its citizens from communicating with the rest of the world without crippling the medium's value." Replace "communicating" with "training AI models" and the challenge becomes clear.

### The AI Innovation Zone Scenario

Small nations could establish "AI Innovation Zones" offering tax holidays and state protection. The instant transmissibility of trained models means breakthroughs achieved anywhere can deploy globally through CDN endpoints.

The [A.Q. Khan network operated for decades](https://core.ac.uk/download/pdf/36732689.pdf) despite export controls, using shell companies in Dubai and Malaysia. When US export controls threatened PGP encryption, [Phil Zimmermann published the source code as a book](https://en.wikipedia.org/wiki/Pretty_Good_Privacy#Criminal_investigation), leveraging First Amendment protections.

### The Economic Logic of AI Havens

The Sustainability Directory's analysis of "pollution havens" reveals why developing nations become willing hosts: the promise of foreign investment, jobs, and technological leapfrogging. These aren't rogue states but rational economic actors. When faced with a choice between adhering to a moratorium that keeps them technologically dependent or hosting AI development that brings billions in investment, the choice is predetermined.

Consider: If even U.S. states in 2025 refuse coordination for fear of losing AI investment to neighboring states, how can we expect global coordination among nations with vastly different economic incentives? The SEC whistleblower program received tips from 99 foreign countries in 2021 alone, showing the global reach of regulatory arbitrage.

## Pathway Two: How GPU Swarms Scale

### From Theory to Achieved Reality

Training frontier AI models on distributed consumer hardware isn't just feasible—it's happening. [Deep Gradient Compression (DGC) algorithms achieved 270×–600× communication reduction](https://arxiv.org/abs/1712.01887) back in 2018, making training viable over home internet connections.

But 2025 brought the paradigm shift: [0G Labs with China Mobile announced](https://thedefiant.io/news/press-releases/0g-labs-achieves-breakthrough-in-decentralized-ai-training-with-100-billion-parameters) their DiLoCoX framework achieving 357× speedup in distributed AI training. They successfully trained a 107 billion parameter model on 1 Gbps networks using decentralized clusters. Related research like [OpenDiLoCo](https://arxiv.org/abs/2407.07852) demonstrates cross-continent training with 90-95% utilization.

### BOTEC 2.0: From Conservative Estimates to Proven Capabilities

Our original calculation was conservative. With DiLoCoX validation, let's recalibrate:

**Original Assumptions (Conservative)**:
- 50,000 RTX GPUs @ 40 TFLOP/s effective
- 20% utilization → 290 days to 1e25 FLOP

**DiLoCoX-Validated Assumptions (Achievable Today)**:
- Same 50,000 RTX GPUs
- 357× communication efficiency gain
- But: 18.9-40% computational slowdown (Sharma et al., 2025)
- Net result: **35-60 days** to 1e25 FLOP

*Adjust the 40 TFLOP/s assumption or efficiency gains to test sensitivity. Cost estimates of $30-60M assume a mix of approaches including rental markets, used hardware, or illicit access to compute.*

### The Folding@home Precedent: Infrastructure Already Exists

[Folding@home achieved 1.5 exaFLOP/s](https://foldingathome.org/2021/01/05/2020-in-review-and-happy-new-year-2021/) during COVID-19, coordinating:
- **280,000 GPUs** globally
- **4.8 million CPU cores** contributing cycles
- **1.5 exaFLOPS** sustained (exceeding top 100 supercomputers combined)
- **All volunteer-driven** with no financial incentive

Now imagine the same infrastructure, but:
- Financially incentivized (cryptocurrency rewards or direct payment)
- Technically optimized (DiLoCoX-style algorithms with 357× speedup)
- Purpose-built (dedicated to AI training, not protein folding)
- State-sponsored (unlimited funding and coordination)

The infrastructure for distributed training at scale doesn't need to be built—it already exists.

### The Distributed Training Arms Race

We're witnessing a technical revolution in real-time:

- **2018**: Deep Gradient Compression achieves 270-600× communication reduction
- **2020**: Folding@home aggregates 280,000 GPUs and 4.8 million CPU cores, achieving 1.5 exaFLOPS
- **2023**: Evaluation shows ACP-SGD achieves 4.06× speedup over standard distributed training
- **2025**: DiLoCoX trains 107B parameters on consumer-grade internet

But there's a counter-narrative. Sharma et al. (2025) found that even in ideal datacenter conditions with A100s and H100s, the overlapping of communication and computation causes an average 18.9% slowdown, maxing out at 40%. On unreliable consumer networks? The penalty could be severe.

This creates a fascinating dynamic: As compression algorithms improve exponentially, coordination challenges grow linearly. The race is on—and the offense is winning.

### The Botnet Precedent

The [Smominru botnet infected 500,000+ machines generating $8,500/day](https://www.proofpoint.com/us/threat-insight/post/smominru-monero-mining-botnet-making-millions-operators) in cryptocurrency. BitTorrent had approximately 150 million monthly active users at peak. The engineering for distributed AI training (asynchronous gradient updates, fault tolerance, dynamic participation) is largely solved.

## Pathway Three: How Covert State Programs Hide

### From the Horse's Mouth: A Bioweapons Chief Confesses

The Soviet Union operated Biopreparat from 1974-1991, reportedly employing tens of thousands across dozens of facilities while violating the Biological Weapons Convention. But we don't need to speculate—we have testimony.

In 2001, Dr. Ken Alibek sat before the U.S. House of Representatives. As the former First Deputy Chief of Biopreparat, he wasn't speculating about covert programs—he ran one:

> "The Soviet Union continued an offensive BW program after signing the 1972 BWC... When trilateral inspections were conducted in 1991, the program was still active, and the Soviets covered up the evidence as best they could."

The numbers are staggering:
- **65,000 employees** at peak operation
- **52 secret sites** disguised as civilian facilities
- **90-100 tons** annual production capacity for weaponized smallpox
- **20+ years** of successful concealment despite treaty obligations

Most damning? Alibek reveals the program didn't just continue after the BWC—it accelerated, specifically to leverage genetic engineering breakthroughs. The treaty didn't stop development; it incentivized going underground.

For AI governance, the parallel is chilling: Just as the BWC coincided with the biotechnology revolution, an AI moratorium would coincide with the deep learning revolution. History suggests this timing isn't coincidental—it's catalytic.

The 1979 Sverdlovsk anthrax leak killed approximately 68+ civilians, yet the program remained hidden until defector exposure in 1989. Only 2 defectors (Pasechnik, Alibek) revealed the truth—out of 65,000 employees.

### The Art of Dual-Use Deception

Leitenberg (2005) decoded Biopreparat's structure: a civilian component called "Biopreparat" provided cover for the military planning codenamed "Ferment." Facilities produced vaccines and antibiotics by day, weaponized anthrax by night. Staff published legitimate research in international journals while developing chimeric pathogens in classified labs.

Modern AI facilities have even better cover:
- **Climate modeling** requires identical hardware and similar algorithms
- **Pharmaceutical research** uses the same transformer architectures
- **Financial modeling** needs comparable compute scales
- **Academic research** provides perfect publication cover

As Chas Bartolome (2022) notes: "The full extent of the program was only revealed following the defection of high-placed insiders." External inspections found nothing. Satellite surveillance saw only buildings. The program ended not through detection but through state collapse.

### Repurposing Existing Infrastructure

Countries operate exascale supercomputers for climate modeling, pharmaceutical research, and nuclear simulations. These facilities already have cleared personnel and city-scale power. Repurposing requires only new software. Staff could continue using existing terminology: "molecular dynamics simulations" could describe AI training to outside observers.

[Israel's Dimona facility, initially described as a textile plant, successfully managed US inspections in the 1960s](https://nsarchive.gwu.edu/briefing-book/nuclear-vault/2020-11-10/duplicity-deception-self-deception-israel-united-states-dimona-inspections-1964-65) using fake control rooms and false walls. Iraq reportedly dispersed centrifuge workshops across nondescript buildings. These examples show even physical infrastructure can be hidden; software-based AI training is inherently more concealable.

## Pathway Four: How Offshore Proxy Datacenters Operate

### The Proliferation That Never Stopped

The Congressional Research Service reported in 2025—yes, this year—that "Chinese entities" continue supplying missile-applicable items to Pakistan's ballistic missile program, triggering U.S. sanctions. The nuclear assistance that began in the 1980s hasn't stopped; it's evolved.

During the 1980s-1990s, China reportedly provided Pakistan with nuclear assistance, including 50 kg of weapons-grade uranium delivered via military jet in 1982. Both nations invoked sovereignty when confronted. Despite tracking from 1977, the international community proved powerless until Pakistan's 1998 nuclear tests—16 years after receiving Chinese uranium.

### The Three Tactics of Treaty Circumvention

China's nuclear assistance to Pakistan, meticulously documented across decades, reveals three sophisticated tactics that would translate perfectly to AI:

**1. The Fait Accompli**
When China agreed to sell additional reactors to Pakistan after joining the Nuclear Suppliers Group—seemingly violating its commitments—it simply "grandfathered" them under previous agreements. The NSG didn't approve but ultimately acquiesced (Siddi, 2011).

**Lesson for AI**: Present the violation as irreversible. "The training run is 90% complete."

**2. The Dual Justification**
Every facility has a civilian cover story. Dimona was a "textile plant." Pakistan's enrichment was for "energy independence." China's assistance was for "peaceful nuclear cooperation."

**Lesson for AI**: Every datacenter is for "climate modeling" until proven otherwise.

**3. The Strategic Triangle**
The Heritage Foundation (1998) revealed the motivation: China used Pakistan to counterbalance India, their mutual rival. The client gets capability, the sponsor gets deniability, the rival gets checked.

**Lesson for AI**: Proxy relationships aren't about technology—they're about strategic competition.

### Technical Implementation and Diplomatic Protection

A technologically advanced nation could offer a partner $2 billion in "infrastructure loans" for computing facilities. Constructed as 40 modular units with 200 GPUs each (each below 1e17 FLOP/s threshold), disguised as 5G edge nodes. With hardware outlays near $60 million [±2× depending on GPU generation] and compute costs of $40 million [±50% based on energy prices], GPT-4-class training could complete within seven months.

Units could be designated for telecommunications or research. The host nation invokes sovereignty to block inspections. North Korea's missile proliferation despite MTCR demonstrates how state actors sustain prohibited technology transfer for decades. Trained weights could transfer through [diplomatic pouches, legally untouchable under the Vienna Convention on Diplomatic Relations](https://legal.un.org/ilc/texts/instruments/english/conventions/9_1_1961.pdf).

## Pathway × Detection × Countermeasure Matrix

| Attacker | Pathway | Cost (BOTEC) | Time | Key observables | Countermeasure | Residual risk |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| **Aligned lab in haven** | Regulatory flight | $10–100M | 6–12 mo | Sudden GPU imports; unusual DC buildouts; policy changes | Passports + secondary sanctions | Weights exfil via neutral CDNs/diplomatic channels |
| **Open-source/criminal** | GPU swarm | $30–60M | 35-60 days | IXP bursts; grid micro-signatures; kernel mix; all-reduce patterns | Driver/HSM attestations; fusion watchfloor | Short-lived pop-up swarms; adversarial traffic shaping |
| **State lab** | Covert program | $100M–$1B | 6–18 mo | Sustained HPC load; procurement euphemisms; nighttime anomalies | Peer review → inspectorate; foundry leverage | Classification shields; national-security carve-outs |
| **Sponsor ↔ client** | Offshore proxies | $100–200M | 6–12 mo | "Edge" nodes with abnormal PUE; thermal signatures; GPU imports | Attested exports; insurer/bond gating | Sovereignty claims; diplomatic pouch transfers |

*Detection confidence: At 24h aggregation, we estimate our fusion watchfloor would flag ~90% of GPT-4-scale runs at 10% false positive rate across member-state grids, assuming 60% IXP coverage and hardware-rooted attestation on 80% of datacenter GPUs. These are author estimates based on analysis of detectable signatures across multiple channels.*

## The Defection Cascade: A Mathematical Certainty

The interaction of these pathways creates predictable dynamics documented by research on regulatory arbitrage. Pollman (2019) documents how tech companies don't just exploit individual loopholes—they create systemic pressure that forces jurisdictional competition:

1. **First Mover**: One jurisdiction defects for economic gain (Singapore with stem cells, 2001)
2. **Competitive Response**: Neighboring jurisdictions must follow or lose investment (South Korea, UK follow suit)
3. **Race to the Bottom**: Standards progressively lower (from "ethical guidelines" to "notification requirements")
4. **Regime Collapse**: Original restrictions become meaningless (stem cell research continues globally)

**Predicted Timeline for AI Moratorium Cascade**:
- Month 0-3: Major powers agree to moratorium
- Month 3-6: Small nation announces "AI Innovation Zone"
- Month 6-9: 3-5 nations follow with competitive offerings
- Month 9-12: Major power claims "defensive exception"
- Month 12-18: Moratorium exists in name only

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

Treat every accelerator above 1e13 FLOP/s (training-relevant FP operations) like fissile material: embedded secure elements must sign device ID, instantaneous power, and rolling hash of executed kernels to an immutable Merkle log. [NVIDIA H100 GPUs already include attestation capabilities](https://developer.nvidia.com/blog/confidential-computing-on-h100-gpus-for-secure-and-trustworthy-ai/), proving technical feasibility. The hardware exists—it ships in "CC-Off" mode by default.

### 2. Dynamic, Auto-Updating Risk Thresholds

Static FLOP caps age badly as algorithmic efficiency doubles every 16 months. The International AI Safety Commission should recalibrate thresholds quarterly, mirroring the [EU ETS cap-tightening approach](https://climate.ec.europa.eu/eu-action/carbon-markets/eu-emissions-trading-system-eu-ets/eu-ets-emissions-cap_en).

### 3. Extraterritorial Enforcement & Secondary Sanctions

Export licenses, foundry access, and dollar-clearing must hinge on compute passport compliance. Non-compliant entities face escalating sanctions up to full financial blocking.

### 4. Whole-of-Network Detection for Distributed Training

A fusion center must correlate passport logs, backbone flow patterns, and bulk-power telemetry. Even sub-threshold GPUs collectively create detectable signatures (all-reduce operations every tens of seconds, sustained power 5-15% above baseline). AI training creates distinctive "IO storms" detectable at IXPs according to Kentik research, though NetDiffusion shows AI can generate synthetic traffic to mask signatures—an ongoing arms race.

### 5. International Inspectorate with Graduated Authority

**Phase 1 (Months 0-6):** Voluntary peer review among G7+ nations
**Phase 2 (Months 6-12):** Reciprocal inspection agreements with strong export-control leverage
**Phase 3 (Months 12+):** Work toward "anywhere, anytime" authority modeled on [IAEA nuclear inspections](https://www.iaea.org/sites/default/files/publications/magazines/bulletin/bull34-1/34102451624.pdf)

*Note: IAEA's Gruemm admits: "Safeguards cannot prevent diversion... they are an ex post facto warning system." Full UNSCOM-style authority required UN Security Council backing after military conflict; we start with achievable voluntary frameworks.*

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

First insiders reporting unlicensed training earn 10-30% of monetary sanctions with legal immunity. [The SEC whistleblower program has paid over $2.2 billion](https://www.sec.gov/enforcement-litigation/whistleblower-program) and has awarded over $50 million in individual cases. We propose a similar framework with comparable incentives. In 2021 alone, the SEC received tips from 99 foreign countries, showing global reach.

### Why Insiders Matter More Than Inspectors

History's most successful detection mechanism isn't technology—it's defection:

| Program | Duration Hidden | Detection Method | Insider Impact |
|---------|----------------|------------------|----------------|
| Biopreparat | 19+ years | 2 defectors (out of 65,000) | Revealed entire program |
| Pakistan Nuclear | 16+ years | A.Q. Khan network exposure | Mapped proliferation web |
| Dimona | 10+ years | Mordechai Vanunu | Provided photographs |
| Iraq WMD | 12+ years | Hussein Kamel defection | Triggered inspections |

**The Statistical Reality**:
- Average covert program: 15+ years undetected
- Average number of insiders needed for revelation: 1-2
- Percentage of workforce that defects: <0.01%
- Impact of single defector: Program termination

This is why our whistleblower bounty program isn't optional—it's essential.

### 9. Conditional Infrastructure Aid & Pre-Certified Templates

Development loans require pre-certified datacenter blueprints with built-in telemetry. Low-capacity states gain infrastructure while agreeing to verification.

### 10. Sunset & Iteration Clause

All rules expire after 30 months unless renewed, forcing continual updates as capabilities evolve.

## The Countermeasure Reality Check

Our proposed countermeasures have precedent—both encouraging and sobering:

**Compute Passports: Technically Ready, Politically Fraught**
- ✅ NVIDIA H100 already includes hardware attestation, secure boot, and TEE capabilities
- ✅ Device attestation can verify "authentic NVIDIA GPUs in a known, trusted secure state"
- ⚠️ Requires opt-in ("CC-On" mode)—political will needed for mandates
- ❌ Only works for compliant actors—black market GPUs remain untracked

**International Inspectorate: Warning System, Not Prevention**
- ✅ IAEA model shows international verification is possible
- ⚠️ IAEA's Gruemm admits: "Safeguards cannot prevent diversion... they are an ex post facto warning system"
- ⚠️ Iraq's clandestine program revealed fundamental inability to detect undeclared activities
- ❌ Resource requirements immense: IAEA struggles with flat budget despite growing mandate

**Whistleblower Bounties: Powerful but Complementary**
- ✅ SEC program generated $2.2B in awards, $5B in recoveries
- ✅ Global reach: tips from 99 countries in 2021 alone
- ✅ 83% of whistleblowers reported internally first—bounties complement, not replace, compliance
- ⚠️ Requires rule of law and extradition treaties
- ❌ Authoritarian states can eliminate whistleblower threats

**Network Detection: Arms Race in Progress**
- ✅ AI training creates distinctive "IO storms" detectable at IXPs (Kentik)
- ✅ Traffic fingerprinting can identify activities through encrypted connections
- ⚠️ NetDiffusion shows AI can generate synthetic traffic to mask signatures
- ❌ Adversarial actors will develop countermeasures faster than detection improves

### The Lesson of Every Arms Control Regime

Garfinkel et al. (2024) identify compute's unique properties: detectable, excludable, quantifiable, and concentrated supply chain. But they also warn: "Incentives for circumvention... smuggling... algorithmic progress making compute a less reliable proxy."

Every dual-use technology follows the same pattern:
1. Initial control regime with high confidence
2. Technological advancement reduces barriers
3. Economic incentives drive circumvention
4. Geopolitical competition ensures defection
5. Control regime becomes ceremonial

We're currently at step 1. The research suggests we'll reach step 5 faster than any previous technology.

## From Theory to Practice: Phased 18-Month Implementation

### Phase 1: Emergency Response (Days 0-90) - Cloud & Hyperscaler Focus

**Week 1: Activate existing frameworks**

- Issue emergency orders for 1e24 FLOP run notices (14-day advance)
- Announce whistleblower bounties using existing SEC/FCA frameworks ($2.2B precedent)
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

- **Network:** All-reduce patterns every 10-60 seconds (95% confidence at IXPs) - "IO storms" per Kentik
- **Power:** Sustained draw 5-15% above baseline, especially nights/weekends (80% confidence)
- **Thermal:** Datacenter heat plumes visible in satellite imagery (60% confidence)
- **Kernels:** Distinctive matmul/attention sequences via attestation (99% confidence if deployed)
- **Procurement:** Bulk GPU purchases and "AI accelerator" euphemisms (70% confidence)

Combined multi-signal fusion enables ~90% detection probability within 24 hours for GPT-4-scale runs (author estimate based on analysis of signature visibility across channels).

## Specific Predictions (Falsifiable Within 24 Months)

1. **≥1 covert run above 1e25 FLOP detected** via power + IXP fusion in a member state by June 2026 (75% confidence, up from 60%)
2. **First distributed swarm achieving 1e24 FLOP** reported publicly by December 2025 (90% confidence, up from 75%)
3. **≥3 countries establish "AI Innovation Zones"** with explicit moratorium exemptions by March 2026 (85% confidence, up from 70%)
4. **Attestation adoption reaches 50% of datacenter GPUs** in US/EU by December 2025 (30% confidence, down from 40% given "CC-Off" default)
5. **First $100M+ penalty issued** for unauthorized frontier training by September 2026 (50% confidence)

## Conclusion: The Window of Opportunity

The challenges outlined establish requirements for governance that might actually work. Twenty years might provide sufficient time to solve alignment challenges, but only if we address these circumvention pathways from the outset—and the evidence shows all four are already being explored.

Success depends not on assuming compliance but anticipating creative non-compliance. We must design systems robust to partial adherence, fragmented enforcement, and determined adversaries. This means integrating verification into hardware (H100s already have it), updating rules before obsolescence, and aligning economic incentives with safety goals.

The four pathways of ASI moratorium circumvention represent fundamental challenges validated by decades of precedent and contemporary evidence. Addressing them requires continuous innovation in AI safety governance.

Perfect control remains unachievable—history proves this repeatedly. The question is whether we can raise the bar high enough, quickly enough, to buy time for alignment research. The window narrows with each passing month.

**The path forward requires neither naive optimism nor paralyzing pessimism, but clear-eyed analysis coupled with determined action.** With the [EU AI Act now in force](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) and [America's AI Action Plan](https://www.whitehouse.gov/wp-content/uploads/2025/07/Americas-AI-Action-Plan.pdf) pulling in the opposite direction, the regulatory asymmetry creates immediate exploitable gaps—gaps that actors are already beginning to probe.

*Begin with what's achievable: cloud-first attestation, fusion watchfloors, and whistleblower protections. Build momentum through voluntary adoption before mandates. The perfect must not be the enemy of the good when the stakes are existential.*

## Technical Glossary

### Computing Thresholds & Metrics

**FLOP (Floating-Point Operations)** - Standard unit for measuring computational work. One FLOP equals one arithmetic operation on decimal numbers. Distinguished from FLOPS (operations per second).

**1e25 FLOP** - Total compute budget for GPT-4-class training, adopted by EU AI Act as systemic risk threshold. This is cumulative compute, not throughput.

**Training-relevant FP FLOP/s** - Specifically FP16/BF16/FP8 operations used in training, measured via attested microbenchmarks. Not INT8 TOPS used in inference.

**1e17 FLOP/s** - Proposed licensing threshold for compute facilities (throughput, not total).

**1e13 FLOP/s** - Individual accelerator threshold for mandatory attestation.

### Security & Verification Infrastructure

**Compute passports** - Cryptographic attestation from embedded secure elements in GPUs, signing operations to immutable logs. NVIDIA H100s already include this capability via Confidential Computing features.

**Hardware Security Module (HSM)** - Tamper-resistant device storing model weights, requiring attestation for access.

**Merkle log** - Append-only cryptographic structure preventing retroactive falsification.

### Distributed Training Technical

**Gradient compression** - Bandwidth optimization achieving 270×-600× reduction ([DGC](https://arxiv.org/abs/1712.01887)), enabling training over 1 Gbps links.

**DiLoCoX** - December 2024 framework achieving 357× speedup for distributed training, successfully training 107B parameters on consumer internet (0G Labs/China Mobile).

**All-reduce operations** - Synchronized gradient exchanges creating detectable network patterns every 10-60 seconds, visible as "IO storms" at IXPs.

**Asynchronous updates** - Protocol allowing nodes to contribute without tight synchronization, increasing fault tolerance.

### Historical Precedents

**Biopreparat** - Soviet biological weapons program (1974-1991) with 65,000 employees across 52 sites, demonstrating large-scale covert dual-use programs. Only revealed through 2 defectors out of entire workforce.

**WiCell** - Wisconsin institute created as explicit "safe haven" for stem cell research, training 800+ scientists despite federal restrictions.

**Dimona deception** - Israeli nuclear facility disguised as textile plant, managing US inspections 1960s using fake control rooms and false walls.

**0G Labs/DiLoCoX** - December 2024 announcement of distributed 107B parameter training achieving 357× speedup.

### Regulatory Frameworks

**EU AI Act** - Entered force August 2024, GPAI obligations from August 2025, 1e25 FLOP systemic risk threshold.

**America's AI Action Plan** - July 2025 framework emphasizing innovation and streamlined regulatory processes, creating divergence from EU approach.

**SEC Whistleblower Program** - Paid $2.2B in awards, generated $5B in recoveries, receives tips from 99 countries annually.

**Nuclear liability minimum** - IAEA conventions establish minimum coverage requirements, precedent for AI performance bonds.

**Secondary sanctions** - Penalties on third parties facilitating non-compliant runs, not blanket country sanctions.

## About This Research

This analysis represents our first major foray into AI governance research, emerging from a systematic red-teaming exercise that won first place in Apart Research's hackathon. As researchers new to governance, we bring an outsider's perspective that may catch vulnerabilities domain experts might miss.

This enhanced version integrates 50+ peer-reviewed sources, congressional testimony from program insiders who ran covert WMD programs, and real-time evidence from 2024-2025 showing these dynamics actively unfolding.

We're continuing through Apart Lab Studio with mentorship from the ControlAI team, focusing on technical verification mechanisms implementable without consensus, economic incentives favoring compliance, and adaptive governance evolving with the technology.

*For questions, critiques, or collaboration: [contact information]*
