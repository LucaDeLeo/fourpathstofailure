# Perfect Implementation Isn't Enough: Four Paths Around an ASI Moratorium and How to Block Them

> **TL;DR:**
> 
> **Four critical vulnerabilities threaten any AI moratorium:**
> • Regulatory havens enabling jurisdiction shopping
> • Distributed GPU swarms training models below detection thresholds  
> • Covert state programs hiding behind national security classifications
> 
> **Our countermeasures to close these gaps:**
> • Cryptographic compute passports for all accelerators
> • $50M whistleblower bounties with legal immunity
> • Performance bonds and "anywhere, anytime" inspections
> 
> **Timeline & Investment:** 90-day emergency response, 18-month full implementation, $300-400M Year 1 cost (less than one frontier training run)

> **What happens next quarter:**
> • **14-day Model Run Notice** for ≥10^24 FLOP runs (strict liability: $250M or 2% global turnover)
> • **Driver-level software attestation** turned on by default  
> • Stand up a **fusion watchfloor** (cloud + IXPs + bulk-power telemetry)
> • Announce **whistleblower awards** (10 to 30% of fines, capped at $50M)
> • Start **bond/insurance quotes** for frontier runs
> • Publish **first threshold recalibration** calendar
> • Begin **voluntary peer review** between aligned nations

> **Origin & Methodology:** This analysis emerged from winning first place in [Apart Research's "Red-Teaming the Narrow Path" hackathon](https://apartresearch.com/project/four-paths-to-failure-red-teaming-asi-governance-se53), where we systematically stress-tested proposed AI governance frameworks through adversarial thinking. As researchers new to governance, we approached the problem with fresh eyes, potentially catching vulnerabilities that established experts might overlook. We're continuing this work through Apart Lab Studio with mentorship from the ControlAI team.

## Introduction: The Governance Paradox of Transformative AI

What if we achieved the impossible: perfect global cooperation on AI safety, and it still wasn't enough?

*Epistemic status: We're governance research newcomers who approached this problem through systematic adversarial analysis. While our fresh perspective may catch overlooked vulnerabilities, we defer to domain experts on political feasibility and implementation details. Our confidence is highest on technical circumvention methods (based on documented capabilities) and lower on international coordination dynamics.*

We face a documented reality. Even as international bodies converge on sophisticated regulatory frameworks for artificial superintelligence (ASI), a troubling reality emerges: the very nature of AI development may make it ungovernable through traditional means.

The Narrow Path's proposed twenty-year moratorium on ASI development represents humanity's most ambitious attempt at coordinated technological restraint. Yet beneath the surface of this comprehensive proposal lies a troubling reality: the characteristics that make AI development dangerous also make it uniquely resistant to control mechanisms.

This analysis examines four distinct pathways through which determined actors could circumvent even the most comprehensive ASI moratorium. Each pathway could enable GPT-4-scale training within 6-18 months, exploiting fundamental weaknesses in our current governance paradigms.

## The Current Regulatory Landscape

As we write this, the global AI governance landscape is rapidly evolving. The [EU AI Act, which entered force in August 2024](https://commission.europa.eu/news-and-media/news/ai-act-enters-force-2024-08-01_en), establishes the world's first comprehensive AI regulatory framework, including the [10^25 FLOP threshold for systemic risk](https://artificialintelligenceact.eu/high-level-summary/) that features prominently in moratorium proposals. Meanwhile, [America's AI Action Plan (July 2025)](https://www.whitehouse.gov/wp-content/uploads/2025/07/Americas-AI-Action-Plan.pdf) takes a starkly different approach, explicitly warning against "burdensome regulations" in favor of innovation and global competitiveness. This divergence creates precisely the regulatory asymmetry that determined actors could exploit.

## The Moratorium's Achilles Heel: Understanding the Enforcement Challenge

The Narrow Path's Phase 0 proposes a comprehensive regulatory framework including: training licenses for runs above 10^25 FLOP, compute licenses for cloud providers above 10^17 FLOP/s, application licenses for new deployments, and prohibition of specific dangerous capabilities. The proposal includes monitoring of data centers' energy consumption with approximately 12-day intervention windows.

While the framework proposes defense-in-depth approaches with multiple layers of oversight, the four circumvention pathways explored here reveal how determined actors could exploit gaps between jurisdictions, leverage distributed infrastructure, and abuse dual-use technologies to undermine these safeguards.

## Pathway One: How Regulatory Flight Happens

### Historical Precedents and Modern Parallels

When the United States restricted federal funding for embryonic stem cell research in 2001, Singapore, the UK, and South Korea became global leaders in the field. FTX relocated to the Bahamas in three months to avoid SEC oversight. Binance secretly taught US customers bypass techniques while maintaining plausible deniability.

### The AI Innovation Zone Scenario

Small nations could establish "AI Innovation Zones" offering tax holidays and state protection. The instant transmissibility of trained models means breakthroughs achieved anywhere can deploy globally through CDN endpoints.

The [A.Q. Khan network operated for thirty years](https://www.nonproliferation.org/wp-content/uploads/npr/tucker33.pdf) despite export controls, using shell companies in Dubai and Malaysia. When US export controls threatened PGP encryption, [Phil Zimmermann published the source code as a book](https://en.wikipedia.org/wiki/Pretty_Good_Privacy), leveraging First Amendment protections.

## Pathway Two: How GPU Swarms Scale

### Technical Feasibility and Historical Validation

Training frontier AI models on distributed consumer hardware is technically feasible today. Gradient compression algorithms have reduced communication requirements by 100x, making training viable over home internet connections.

[Folding@home achieved 1.5 exaFLOP/s](https://foldingathome.org/2021/01/05/2020-in-review-and-happy-new-year-2021/), exceeding the [world's top 100 supercomputers combined](https://www.tomshardware.com/news/foldinghome-coronavirus-fight-powerful-top-500-supercomputers). Now imagine 50,000 participants with consumer graphics cards below licensing thresholds. Cost modeling shows ~50,000 RTX-class cards [±2× based on secondary-market mix], obtainable for approximately $25 million, could accumulate the 10^25 FLOP budget for GPT-4-class training in 8-12 months.

Remarkably, [0G Labs with China Mobile recently announced](https://x.com/0G_labs/status/1953530200391598551) their DiLoCoX framework achieving 10x speed improvement in distributed AI training *(vendor-reported results under active validation)*. They successfully trained a 107 billion parameter model on 1 Gbps networks using decentralized clusters, offering what they describe as "strategic independence from hyperscalers."

### The Botnet Precedent

The Smominru botnet infected 500,000+ machines generating $8,500/day in cryptocurrency. BitTorrent had 150 million monthly active users at peak. The engineering for distributed AI training (asynchronous gradient updates, fault tolerance, dynamic participation) is largely solved.

## Pathway Three: How Covert State Programs Hide

### The Biopreparat Model

The Soviet Union operated [Biopreparat from 1974-1991](https://www.nonproliferation.org/wp-content/uploads/npr/tucker33.pdf), employing 60,000 people across 52 facilities while violating the Biological Weapons Convention. Facilities masqueraded as pharmaceutical plants. The 1979 Sverdlovsk anthrax leak killed ~100 people, yet the program remained hidden until defector exposure in 1989.

### Repurposing Existing Infrastructure

Countries operate exascale supercomputers for climate modeling, pharmaceutical research, and nuclear simulations. These facilities already have cleared personnel and city-scale power. Repurposing requires only new software. Staff could continue using existing terminology: "molecular dynamics simulations" could describe AI training to outside observers.

Israel's Dimona facility, originally labeled a "textile plant," successfully deceived US inspectors. Iraq dispersed centrifuge workshops across nondescript buildings. These examples show even physical infrastructure can be hidden; software-based AI training is inherently more concealable.

## Pathway Four: How Offshore Proxy Datacenters Operate

### The Pakistan-China Nuclear Model

During the 1980s-1990s, China provided Pakistan with weapons-grade uranium and warhead blueprints, violating non-proliferation norms. Both nations invoked sovereignty when confronted. Despite tracking from 1977, the international community proved powerless until Pakistan's 1998 nuclear tests.

A technologically advanced nation could offer a partner $2 billion in "infrastructure loans" for computing facilities. Constructed as 40 modular units with 200 GPUs each (each below 10^17 FLOP/s threshold), disguised as 5G edge nodes. With hardware outlays near $60 million [±2× depending on GPU generation] and compute costs of $40 million [±50% based on energy prices], GPT-4-class training could complete within seven months.

### Technical Implementation and Diplomatic Protection

Units could be designated for telecommunications or research. The host nation invokes sovereignty to block inspections. North Korea's missile proliferation despite MTCR demonstrates how state actors sustain prohibited technology transfer for decades. Trained weights could transfer through diplomatic pouches, legally untouchable under the Vienna Convention.

## The Cascade Effect: When One Domino Falls

The interaction of these pathways creates concerning dynamics:

- **Demonstration Effects**: Successful circumvention encourages others to follow
- **Investment Migration**: Capital flows to haven states after early successes
- **Technical Diffusion**: Distributed networks share techniques, accelerating capability
- **Justification Cascades**: Classified programs cite suspected violations to justify expansion
- **Partnership Proliferation**: Countries seek AI partners to avoid being left behind

All four pathways could activate simultaneously, creating a situation where the moratorium exists on paper while ASI development proceeds through multiple channels.

## Pre-Addressing Core Objections

### Privacy and Civil Liberties

Telemetry is minimal by design: device ID, coarse kernel class, aggregate FLOP count, instantaneous power, and memory bandwidth. Crucially, this includes no model weights, no data, no source code. Logs are signed on device and encrypted in transit; access requires a warrant or regulatory order and is audited by an independent third party. Summaries (not raw logs) are published quarterly.

### Incumbent Entrenchment  

All rules include 30-month sunset clauses requiring active renewal. Open reference implementations ensure smaller players can comply. Subsidized compliance assistance for organizations under $100M revenue prevents regulatory capture. The framework evolves with the technology rather than freezing current advantages.

### Sovereignty Concerns

Secondary sanctions target non-compliant *runs*, not countries or companies. Aid packages offset compliance costs for lower-capacity states. Reciprocity agreements ensure mutual benefit. The system respects sovereignty while creating strong incentives for voluntary participation.

## Toward Robust Solutions: Strengthening the Framework

To transform the moratorium from a jurisdiction-bounded freeze into a verifiable global regime, we propose ten interconnected enhancements:

### 1. Universal Cryptographic Attestation ("Compute Passports")

Treat every accelerator above 10^13 FLOP/s like fissile material: embedded secure elements must sign device ID, instantaneous power, and rolling hash of executed kernels to an immutable Merkle log. [NVIDIA H100 GPUs already include attestation capabilities](https://developer.nvidia.com/blog/confidential-computing-on-h100-gpus-for-secure-and-trustworthy-ai/), proving technical feasibility.

### 2. Dynamic, Auto-Updating Risk Thresholds

Static FLOP caps age badly as algorithmic efficiency doubles every 16 months. The International AI Safety Commission should recalibrate thresholds quarterly, mirroring the [EU ETS cap-tightening approach](https://ec.europa.eu/commission/presscorner/detail/en/qanda_21_1683).

### 3. Extraterritorial Enforcement & Secondary Sanctions

Export licenses, foundry access, and dollar-clearing must hinge on compute passport compliance. Non-compliant entities face escalating sanctions up to full financial blocking.

### 4. Whole-of-Network Detection for Distributed Training

A fusion center must correlate passport logs, backbone flow patterns, and bulk-power telemetry. Even sub-threshold GPUs collectively create detectable signatures.

### 5. International Inspectorate with "Anywhere, Anytime" Access

Diplomatically-immune teams must have authority for boot-level verification. This approach constrained [Iraq's nuclear program after 1991](https://www.iaea.org/newscenter/statements/status-nuclear-inspections-iraq).

### 6. Hardware Security Module (HSM) Weight Protection

Frontier weights must remain inside HSMs with checkpoint hashes published within 24 hours. Leaked models instantly reveal breach windows.

### 7. Kill-Switch Performance Bonds

Developers post surety proportional to risk (minimum $250 million). [Nuclear liability conventions mandate ≥300 million SDR](https://www.iaea.org/sites/default/files/gc/gc48inf-5_en.pdf); similar mechanisms would fund emergency response.

### 8. Whistleblower Shield & Bounty Program

First insiders reporting unlicensed training earn 10-30% of fines (up to $50 million) with legal immunity. The SEC has paid nearly $2 billion under similar schemes.

### 9. Conditional Infrastructure Aid & Pre-Certified Templates

Development loans require pre-certified datacenter blueprints with built-in telemetry. Low-capacity states gain infrastructure while agreeing to verification.

### 10. Sunset & Iteration Clause

All rules expire after 30 months unless renewed, forcing continual updates as capabilities evolve.

## From Theory to Practice: An 18-Month Implementation Roadmap

### The Implementation Philosophy: Market Incentives Before Mandates

Rather than waiting for consensus, leverage voluntary adoption and financial incentives. Total Year 1 investment: $300-400 million, less than one frontier training run.

### Phase 1: Emergency Response (Days 0-90)

**Model Run Notice Requirements**
- **Owner**: Digital regulator / competition authority
- **Day 1**: Issue interim rule citing emergency powers; publish notice webform and penalty table
- Any training exceeding 10^24 FLOP must file 14-day advance notice
- Strict liability: $250M or 2% global turnover

**Software-Based Compute Passports**  
- **Owner**: NVIDIA/AMD + hyperscalers
- **Week 2**: Ship signed driver updates; default on in enterprise tenants; public API for attestation receipts
- Driver-level attestation using existing TPMs

**Fusion Watchfloor**
- **Owner**: National cyber center + ISPs + grid operator  
- **Week 4**: Data-sharing MoUs; integrate IXPs, cloud flow logs, and bulk-power anomalies; publish first monthly anomaly report

**$50M Whistleblower Bounties**
- **Owner**: Financial regulator (SEC/FCA equivalent)
- **Week 1**: Authorize bounties worth 10-30% of collected fines using existing frameworks

### Phase 2: Market-Led Adoption (Months 3-6)

**Performance Bonds and Insurance Markets**
- **Owner**: Lloyd's/Munich Re + labs
- **Month 3**: Standardized underwriting questionnaire; bonds priced down for attestation + HSM checkpoints
- $250M minimum bonds for frontier runs

**"Verified Compute" Premium Features**
- **Owner**: NVIDIA/AMD
- Hardware-anchored attestation as premium enterprise feature

**Dynamic Threshold Adjustments**
- **Owner**: International AI Safety Commission (G7 AI Safety Institutes)
- Quarterly recalibration accounting for algorithmic efficiency gains

### Phase 3: Financial Leverage (Months 6-12)  

**Extraterritorial Enforcement**
- **Owner**: Export control authorities + financial regulators
- Foundry access contingent on compute passport compliance
- Secondary sanctions on facilitators

**International Inspectorate**
- **Owner**: G7 AI Safety Institutes caucus
- Starting with voluntary peer review, expanding to "anywhere, anytime" authority

### Phase 4: Infrastructure Hardening (Months 12-18)

**On-Die Compute Passports**
- **Owner**: Intel/TSMC/Samsung foundries
- Next silicon includes embedded secure elements

**Conditional Infrastructure Aid**
- **Owner**: World Bank + regional development banks
- Pre-certified datacenter loans with built-in telemetry

### Technical Architecture: Making Detection Work

Frontier training creates distinctive signatures across multiple observable channels:

```
Key Detection Features:
- Synchronized all-reduce operations with tens-of-seconds patterns
- Sustained power draw 5-15% above baseline during nights/weekends  
- Distinctive kernel execution patterns (matmul/attention sequences)
- Network bursts matching gradient exchange signatures
- Thermal anomalies visible from satellite imagery
```

The compute passport schema captures telemetry without exposing proprietary architectures:

```
Core Telemetry (every 30 seconds):
- GPU serial and host fingerprint
- Kernel operation class (not full code)
- Accumulated FLOP count
- Instantaneous power draw
- Memory bandwidth utilization
- Cryptographic signature anchored to hardware root
```

### What Success Looks Like

**< 6 months:**
- ≥80% of accelerators in member states emit attestations
- Frontier labs obtain bonds
- First threshold recalibration published

**< 12 months:**  
- Detection latency <24h for GPT-4-scale training
- No undetected runs in member states for 6 months
- Distributed training costs 5× premium versus compliant facilities

**< 18 months:**
- 40+ countries in inspection framework
- Haven state problem substantially mitigated
- Next-gen silicon ships with on-die attestation enabled by default

### Critical Uncertainties and Adaptations

**Technical**: Can 10 million existing GPUs be retrofitted? Will cryptographic overhead stay below 0.1%? How do we enable legitimate research while preventing covert training?

**Policy**: Where's the line between training, fine-tuning, and inference? Is G7 participation sufficient? How do we detect violations without enabling surveillance abuse?

**Economic**: Will compliance costs entrench incumbents? Can sanctions overcome sovereignty claims? How do we price unprecedented AI risks?

The framework addresses these through 30-month sunset clauses, quarterly threshold adjustments, and published impact assessments.

### Civil Society Oversight Pledge

We commit to publishing annual impact reports including: false positive rates, appeals processed, sanctions applied, market concentration effects, and compliance costs for different organization sizes. An independent review board with civil liberties organizations will audit the program's privacy protections and recommend improvements. All telemetry data older than 24 months will be automatically deleted unless under active investigation.

### The Window Is Closing

Between our initial analysis and publication, 0G Labs demonstrated distributed training at scale with China Mobile, proving theoretical risks are materializing. The implementation roadmap must begin immediately, not after years of negotiation.

The next 90 days are critical. Emergency measures using existing authority can create momentum for comprehensive governance. Waiting for unanimous agreement guarantees circumvention pathways will be exploited first.

## Strategic Implications for AI Safety

This analysis reveals three fundamental insights:

First, even innovative regulatory approaches face structural challenges when governing AI development. The technology's unique characteristics demand continuous evolution of governance mechanisms.

Second, perfect enforcement is impossible; our goal must be raising circumvention costs while maintaining adaptive capacity. This means accepting some non-compliance while working to minimize impact and detect quickly.

Third, technical verification must be built into the computational substrate itself. Post-hoc detection cannot match digital proliferation speed.

## Conclusion: The Window of Opportunity

The challenges outlined establish requirements for governance that might actually work. Twenty years might provide sufficient time to solve alignment challenges, but only if we address these circumvention pathways from the outset.

Success depends not on assuming compliance but anticipating creative non-compliance. We must design systems robust to partial adherence, fragmented enforcement, and determined adversaries. This means integrating verification into hardware, updating rules before obsolescence, and aligning economic incentives with safety goals.

The four horsemen of ASI moratorium circumvention represent fundamental challenges even to sophisticated frameworks. Addressing them requires continuous innovation in AI safety governance.

Perfect control remains unachievable. The question is whether we can raise the bar high enough, quickly enough, to buy time for alignment research. The window narrows with each passing month.

As we stand at this technological crossroads, the goal centers on ensuring progress proceeds safely. The circumvention pathways demand careful design, international cooperation, and technical innovation.

The path forward requires neither naive optimism nor paralyzing pessimism, but clear-eyed analysis coupled with determined action. With the EU AI Act now in force and divergent national strategies emerging, the window for unified governance narrows daily. The stakes could not be higher.

## About This Research

This analysis represents our first major foray into AI governance research, emerging from a systematic red-teaming exercise that won first place in Apart Research's hackathon. As researchers new to governance, we bring an outsider's perspective that may catch vulnerabilities domain experts might miss.

We're continuing through Apart Lab Studio with mentorship from the ControlAI team. Our ongoing work focuses on:

1. **Technical verification mechanisms** implementable without waiting for consensus
2. **Economic incentive structures** making compliance more attractive than circumvention  
3. **Adaptive governance frameworks** that evolve as fast as the technology

Effective AI governance requires both fresh perspectives and deep expertise. This is why we're combining our adversarial analysis with guidance from established practitioners.

## Join the Conversation

This analysis represents one attempt to stress-test AI governance proposals. We need more minds on these challenges:

**For Researchers & Technologists:** What circumvention pathways have we missed? Can you identify technical solutions?

**For Policymakers:** Adversaries may already be following these blueprints. How can we update current frameworks?

**For Everyone:** Share this analysis with others who care about AI safety. Challenge our assumptions. Propose better solutions.

*The window for effective action is narrowing. Let's use it wisely.*

## Technical Glossary

### Computing Thresholds & Metrics

**FLOP (Floating-Point Operations)** - Standard unit for measuring computational work. One FLOP equals one arithmetic operation on decimal numbers.

**10^25 FLOP** - Total compute budget for GPT-4-class training, adopted by EU AI Act as systemic risk threshold.

**10^17 FLOP/s** - Proposed licensing threshold for compute facilities.

**10^13 FLOP/s** - Individual accelerator threshold for mandatory attestation.

**Exascale (10^18 FLOP/s)** - Current supercomputer tier capable of GPT-4 training in 2 weeks vs 6 months commercially.

**Gradient compression** - Bandwidth optimization achieving 100x reduction, enabling training over home internet.

### Security & Verification Infrastructure

**Merkle log** - Append-only cryptographic structure preventing retroactive falsification of compute logs.

**Hardware Security Module (HSM)** - Tamper-resistant device for storing model weights with attestation requirements.

**Compute passports** - Embedded secure elements in GPUs cryptographically signing operations to immutable logs.

**Salted hash** - One-way cryptographic fingerprint allowing checkpoint verification without revealing weights.

### Historical Precedents & Programs

**Biopreparat** - Soviet biological weapons program (1974-1991) demonstrating feasibility of large-scale covert programs.

**CoCom controls** - Cold War export regime circumvented through shell companies and falsified certificates.

**Folding@home** - Distributed computing achieving 1.5 exaFLOP/s through voluntary participation.

**Smominru botnet** - Cryptocurrency mining malware demonstrating distributed compute monetization at scale.

**DiLoCoX/0G Labs** - December 2024 breakthrough achieving 10x improvement in distributed training *(vendor-reported claims)*.

### Regulatory Mechanisms

**The Narrow Path** - 20-year ASI moratorium proposal with licenses for >10^25 FLOP training and >10^17 FLOP/s facilities.

**SDR (Special Drawing Rights)** - IMF currency basket for nuclear liability, proposed for AI development bonds.

**MTCR** - Voluntary 35-nation missile control agreement demonstrating both successes and failures of technology governance.

**Vienna Convention diplomatic pouches** - Sealed containers with legal immunity, potential vector for weight transfers.

**Secondary sanctions** - Penalties on third parties doing business with violators, key enforcement for non-compliant jurisdictions.

### Distributed Training Infrastructure

**Asynchronous gradient updates** - Protocol allowing nodes to contribute without synchronized coordination.

**Backbone flow patterns** - Network signatures at internet exchanges revealing synchronized training operations.

**Edge computing nodes** - Distributed infrastructure ostensibly for 5G/IoT, potentially repurposable as training clusters.