# Perfect Implementation Isn't Enough: Four Ways an ASI Moratorium Could Fail

> **TL;DR: Even with perfect implementation, proposed AI moratoriums face four critical vulnerabilities that could enable GPT-4-scale AI development within 6-18 months:**
> 
> • **Regulatory havens:** Companies relocating to non-signatory "AI-haven" states (like FTX fleeing to the Bahamas)
> • **Distributed GPU swarms:** 50,000 gaming computers training models below detection thresholds for ~$25M
> • **Covert state programs:** Existing exascale supercomputers repurposed behind national security classifications
> • **Offshore proxy datacenters:** State-sponsored facilities hidden via sovereignty shields
> 
> **Why this matters:** 0G Labs has already demonstrated distributed training at scale with China Mobile. We propose 10 concrete enhancements to close these gaps, from cryptographic "compute passports" to $50M whistleblower bounties. The window for effective governance is closing rapidly.

> **Origin & Methodology:** This analysis emerged from winning first place in [Apart Research's "Red-Teaming the Narrow Path" hackathon](https://apartresearch.com/project/four-paths-to-failure-red-teaming-asi-governance-se53), where we systematically stress-tested proposed AI governance frameworks through adversarial thinking. As researchers new to governance, we approached the problem with fresh eyes—potentially catching vulnerabilities that established experts might overlook. We're continuing this work through Apart Lab Studio with mentorship from the ControlAI team.

## Introduction: The Governance Paradox of Transformative AI

What if we achieved the impossible (perfect global cooperation on AI safety) and it still wasn't enough?

*Epistemic status: We're governance research newcomers who approached this problem through systematic adversarial analysis. While our fresh perspective may catch overlooked vulnerabilities, we defer to domain experts on political feasibility and implementation details. Our confidence is highest on technical circumvention methods (based on documented capabilities) and lower on international coordination dynamics.*

We face a documented reality. Even as international bodies converge on sophisticated regulatory frameworks for artificial superintelligence (ASI), including novel approaches like the Narrow Path's "found systems" definitions and mandatory pre-training safety cases, a troubling reality emerges: the very nature of AI development may make it ungovernable through traditional means.

The Narrow Path's proposed twenty-year moratorium on ASI development (Phase 0) represents humanity's most ambitious attempt at coordinated technological restraint. Yet beneath the surface of even this comprehensive proposal, with its novel "found systems" definitions, mandatory safety cases, and defense-in-depth approaches, lies a troubling reality: the very characteristics that make AI development dangerous (its digital nature, distributed computational requirements, and dual-use applications) also make it uniquely resistant to control mechanisms.

This analysis—which won first place in Apart Research's "Red-Teaming the Narrow Path" hackathon—examines four distinct pathways through which determined actors could circumvent even the most comprehensive ASI moratorium: regulatory havens, distributed GPU swarms, covert state supercomputers, and offshore proxy datacenters. Each pathway could enable GPT-4-scale training within 6-18 months, exploiting fundamental weaknesses in our current governance paradigms and revealing why we need radically new approaches to AI safety governance.

## The Current Regulatory Landscape

As we write this, the global AI governance landscape is rapidly evolving. The EU AI Act, which entered force in August 2024, establishes the world's first comprehensive AI regulatory framework, including the exact 10^25 FLOP threshold for systemic risk that features prominently in moratorium proposals. Meanwhile, America's AI Action Plan (July 2025) takes a starkly different approach, explicitly rejecting "burdensome regulations" in favor of innovation and global competitiveness. This divergence between major powers creates precisely the regulatory asymmetry that determined actors could exploit.

## The Moratorium's Achilles Heel: Understanding the Enforcement Challenge

The Narrow Path's Phase 0 proposes a comprehensive regulatory framework for preventing ASI development for 20 years. The framework includes: training licenses for runs above 10^25 FLOPS (a threshold the EU has already adopted for systemic risk classification), compute licenses for cloud providers above 10^17 FLOPS, application licenses for new deployments, and prohibition of specific dangerous capabilities including AI self-improvement, AIs capable of breaking out of their environment (which would encompass self-replication), and unbounded AI systems whose capabilities cannot be reliably predicted. The proposal includes multiple detection mechanisms, including monitoring of data centers' large energy consumption and physical footprints, with breakout times calculated to provide authorities approximately 12-day windows for intervention.

While the Narrow Path acknowledges enforcement challenges and proposes defense-in-depth approaches with multiple layers of oversight, severe penalties, and adaptive mechanisms, the framework still faces fundamental challenges in practice. Even with sophisticated monitoring and enforcement mechanisms, the four circumvention pathways explored here reveal how determined actors could exploit gaps between jurisdictions, leverage distributed infrastructure, and abuse dual-use technologies to undermine these safeguards.

## Pathway One: Regulatory Flight and the Haven State Problem

### Historical Precedents and Modern Parallels

The phenomenon of regulatory flight is not theoretical; it's a well-documented pattern across multiple domains. When the United States restricted federal funding for embryonic stem cell research in 2001, the field didn't halt; it migrated. Singapore, the UK, and South Korea became global leaders in stem cell research, attracting both talent and investment that might otherwise have remained in the United States.

The cryptocurrency industry provides an even more striking parallel. FTX relocated from the United States to the Bahamas in just three months to avoid SEC oversight. Binance, operating through a complex web of shell companies, secretly taught US customers how to bypass geographic restrictions while maintaining plausible deniability. Both companies made rational responses to regulatory asymmetry.

### The AI Innovation Zone Scenario

Small nations with limited natural resources but flexible governance structures could establish "AI Innovation Zones" offering tax holidays, regulatory exemptions, and state protection for AI development. The US AI Action Plan explicitly warns against regulations that "unfairly benefit incumbents," creating pressure for competitive deregulation even among allies. The instant transmissibility of trained models means that a breakthrough achieved in one jurisdiction can be deployed globally through API endpoints on content delivery networks, making physical location increasingly irrelevant.

Consider the nuclear proliferation network run by A.Q. Khan, which operated for thirty years despite international export controls. Khan used shell companies in Dubai and Malaysia, leveraging Pakistan's sovereignty to shield his activities. His network demonstrates how determined actors can exploit jurisdictional gaps even in heavily monitored domains. AI development, being primarily software-based, presents even fewer physical constraints.

The Phil Zimmermann case offers another instructive example. When US export controls threatened to restrict PGP encryption software, Zimmermann published the source code as a book, leveraging First Amendment protections to circumvent technology transfer restrictions. Similar creativity could easily be applied to AI model distribution.

## Pathway Two: The Distributed GPU Swarm Revolution

### Technical Feasibility and Historical Validation

Training frontier AI models on distributed consumer hardware has become technically feasible today. Modern gaming computers rival the supercomputers of a decade ago, and gradient compression algorithms have reduced communication requirements by two orders of magnitude, making training viable over standard home internet connections.

Folding@home, a distributed computing project for protein folding, achieved 1.5×10^18 FLOPS, more computational power than the world's top 100 supercomputers combined. It accomplished this through voluntary participation. Now imagine a financially incentivized network of 50,000 participants across 60 countries, each operating consumer graphics cards below licensing thresholds. Rough cost modeling shows that ~50,000 RTX-class cards, obtainable for approximately $25 million on primary or grey markets, could accumulate the 10^25 FLOP budget needed for a GPT-4-class model in 8-12 months.

This is no longer merely theoretical. Remarkably, between our original red-teaming analysis and the publication of this blog post, 0G Labs, in collaboration with China Mobile, announced a breakthrough with their DiLoCoX framework that achieved a 10x speed improvement and 95% cost reduction in AI training. They successfully trained a 107 billion parameter model on a 1 Gbps network (typical office internet speeds) using decentralized clusters. This development, emerging in the very window between identifying the risk and documenting it here, with China Mobile's involvement demonstrating state-affiliated interest, proves that distributed training has evolved from academic possibility to practical reality, offering what they describe as "strategic independence from hyperscalers" and the ability to train massive models "without centralized supercomputers."

### The Botnet Precedent

The Smominru botnet infected over 500,000 machines and generated $8,500 USD equivalent per day in cryptocurrency mining in January 2018. This demonstrates both the scale achievable through distributed systems and the difficulty of detection and attribution. BitTorrent, at its peak, had 150 million monthly active users, showing that massive peer-to-peer networks can operate successfully despite legal challenges.

The engineering challenges for distributed AI training are largely solved. Techniques for asynchronous gradient updates, fault tolerance, and dynamic node participation have been developed and tested. A determined actor could leverage these technologies to create a training infrastructure that exists everywhere and nowhere, impossible to regulate through traditional means.

## Pathway Three: Covert State Supercomputers and Dual-Use Deception

### The Biopreparat Model

From 1974 to 1991, the Soviet Union operated Biopreparat, a massive biological weapons program employing 60,000 people across 52 facilities, all while being party to the Biological Weapons Convention. These facilities masqueraded as pharmaceutical plants, vaccine production centers, and agricultural research stations. The 1979 Sverdlovsk anthrax leak killed approximately 100 people, yet the program remained hidden until defector Vladimir Pasechnik exposed it in 1989.

This historical example demonstrates three critical points: large-scale covert programs can operate for decades undetected, dual-use cover stories provide plausible deniability, and even catastrophic accidents may not lead to program exposure if state security apparatus remains intact.

### Repurposing Existing Infrastructure

Countries currently operate exascale supercomputers for ostensibly civilian purposes: climate modeling, pharmaceutical research, materials science, and nuclear stockpile simulations. These facilities already employ thousands of cleared personnel, consume city-scale power, and operate under security protocols that prevent external scrutiny.

Repurposing these facilities for AI training requires no new infrastructure, only new software and adjusted job priorities. Staff could continue using existing terminology: "molecular dynamics simulations" or "weather pattern analysis" could describe AI training runs to outside observers. What takes Google six months on commercial hardware could be accomplished in two weeks on weapons-simulation supercomputers.

Israel's Dimona nuclear facility provides an instructive case study. Originally labeled a "textile plant," then a "nuclear research center," it successfully deceived US inspectors through bricked-over elevators and hidden hallways. Iraq dispersed centrifuge workshops across nondescript buildings, evading inspectors until post-war surprise visits. The Toshiba-Kongsberg affair showed how front companies falsified end-user documents to smuggle five-axis CNC machines to the USSR, despite CoCom controls. These examples demonstrate that even physical infrastructure can be hidden; software-based AI training is inherently more concealable.

## Pathway Four: Offshore Proxy Datacenters and Sovereignty Shields

### The Pakistan-China Nuclear Model

During the 1980s and 1990s, China provided Pakistan with weapons-grade uranium, complete warhead blueprints, and missile technology, all in violation of non-proliferation norms. When confronted, both nations invoked sovereignty and refused to recognize third-party authority over their bilateral relations. Despite tracking these transfers from 1977, the international community proved powerless to stop them until Pakistan's 1998 nuclear tests made the issue moot.

This model could be directly applied to AI development. A technologically advanced nation could offer a middle-income partner $2 billion in "infrastructure loans" to build computing facilities. These could be constructed as 40 modular units with 200 GPUs each, with each unit below the 10^17 FLOP s^-1 licensing threshold, disguised as 5G edge computing nodes or distributed across military bases and universities. With hardware outlays near $60 million and compute costs of approximately $40 million, a GPT-4-class model could be trained on such a cluster within seven months.

### Technical Implementation and Diplomatic Protection

The distributed nature of such facilities provides multiple advantages. Units could be officially designated for telecommunications, scientific research, or national security applications. The host nation could invoke sovereignty to block inspections, while the sponsoring nation maintains plausible deniability about the facilities' true purpose.

North Korea's missile proliferation to Iran, Syria, and Libya, despite the Missile Technology Control Regime, demonstrates how determined state actors can sustain prohibited technology transfer for decades. The Huawei case, where facilities were built with deliberate vulnerabilities allowing state access, shows how infrastructure projects can serve hidden agendas.

Trained model weights could transfer through diplomatic pouches, legally untouchable under the Vienna Convention. A distributed facility operating across multiple sites could train a frontier model within seven months, with results instantly transmissible to the sponsoring nation.

## The Cascade Effect: When One Domino Falls

The truly concerning aspect lies in the interaction and mutual reinforcement of these circumvention pathways. Once one pathway succeeds, others become more likely:

- **Demonstration Effects**: A successful circumvention proves the moratorium's weakness, encouraging others to follow suit
- **Investment Migration**: Capital flows to haven states once early movers demonstrate profitability
- **Technical Diffusion**: Distributed networks naturally share techniques and improvements, accelerating collective capability
- **Justification Cascades**: Classified programs cite suspected violations by adversaries to justify their own expansion
- **Partnership Proliferation**: Countries seek AI development partners to avoid being left behind

All four pathways could activate simultaneously, creating a situation where the moratorium exists on paper while ASI development proceeds through multiple channels. Traditional control mechanisms, designed for visible infrastructure, corporate compliance, and state cooperation, cannot address this fundamental challenge.

## Toward Robust Solutions: Strengthening and Extending the Narrow Path Framework

While the Narrow Path already incorporates several sophisticated mechanisms including hardware tracking, dynamic threshold adjustments, international oversight frameworks, and near-miss reporting systems, the circumvention pathways identified above suggest areas where these mechanisms could be strengthened or extended. To transform the moratorium from a jurisdiction-bounded freeze into a verifiable, adaptive global regime, we propose ten interconnected enhancements: some building on existing Narrow Path provisions, others addressing gaps:

### 1. Universal Cryptographic Attestation ("Compute Passports")

Treat every accelerator above 10^13 FLOP·s^-1 like fissile material: embedded secure elements must sign device ID, instantaneous power, and a rolling hash of executed kernels to an immutable Merkle log. This creates an environment where illicit clusters become increasingly difficult to hide, as missing or falsified logs immediately flag suspicious activity.

### 2. Dynamic, Auto-Updating Risk Thresholds

Building on the Narrow Path's provision for adjustable thresholds, we recommend more frequent recalibration. Static FLOP caps age badly as algorithmic efficiency doubles roughly every 16 months. While the EU requires model evaluations and adversarial testing for systemic-risk models, these measures lack the cryptographic verification and real-time monitoring needed to prevent circumvention. The proposed International AI Safety Commission should recalibrate thresholds quarterly, mirroring mechanisms like the EU ETS's cap-tightening approach. Actors can no longer "wait out" fixed thresholds.

### 3. Extraterritorial Enforcement & Secondary Sanctions

Export licenses, foundry access, and dollar-clearing privileges must hinge on compute-passport compliance. Non-compliant entities face escalating sanctions up to full financial blocking, making haven-seeking uneconomic when every bank and chip-fab risks losing core markets.

### 4. Whole-of-Network Detection for Distributed Training

A fusion center must correlate passport logs, backbone flow patterns, and bulk-power telemetry. Even if each GPU stays sub-threshold, collective traffic and power spikes can flag covert megaprojects in near-real time.

### 5. International Inspectorate with "Anywhere, Anytime" Access

Extending the Narrow Path's international treaty framework with more specific inspection powers, diplomatically-immune teams must have authority to demand boot-level verification and validate logs on-site. This approach finally constrained Iraq's hidden enrichment program after 1991 and could similarly expose covert AI training.

### 6. Hardware Security Module (HSM) Weight Protection

Frontier weights must remain inside HSMs with every checkpoint publishing a salted hash within 24 hours. A leaked model instantly reveals the breach window, enabling narrow forensics and full bond forfeiture.

### 7. Kill-Switch Performance Bonds

Developers post surety proportional to externality risk (minimum $250 million). Nuclear liability conventions already mandate ≥300 million SDR per reactor; similar mechanisms would fund rapid emergency response and deter reckless deployments.

### 8. Whistleblower Shield & Bounty Program

First insiders reporting unlicensed frontier training earn 10-30% of enforcement fines (up to $50 million) and receive legal immunity. The SEC has paid almost $2 billion under similar schemes. Big bounties make leaks near-certain.

### 9. Conditional Infrastructure Aid & Pre-Certified Templates

Development bank loans and tariff-free chip exports require pre-certified datacenter blueprints with built-in passport telemetry and smart-metering. Low-capacity states gain modern infrastructure while agreeing upfront to verification hooks.

### 10. Sunset & Iteration Clause

All telemetry rules, thresholds, and sanctions expire after 30 months unless renewed, forcing continual political attention and technical updates while preventing ossification as capability landscapes shift.

## From Theory to Practice: An 18-Month Implementation Roadmap

While the ten solutions above outline what needs to be built, the question remains: how do we actually implement these measures before circumvention pathways are exploited? Drawing from successful technology control regimes and market dynamics, we've developed an 18-month roadmap that transforms these proposals into operational reality.

### The Implementation Philosophy: Market Incentives Before Mandates

Rather than waiting for perfect international consensus, the implementation strategy leverages voluntary market adoption, financial incentives, and gradual formalization. The total Year 1 investment of $300-400 million—less than the cost of a single frontier model training run—could fundamentally reshape the AI governance landscape.

### Phase 1: Emergency Response (Days 0-90)

The first 90 days focus on standing up minimal viable controls using existing infrastructure:

**Model Run Notice Requirements**: Any training exceeding 10^24 FLOP must file notice 14 days before starting, with strict liability penalties of $250M or 2% global turnover. This creates immediate visibility into frontier development.

**Software-Based Compute Passports**: Driver-level attestation using existing Trusted Platform Modules begins collecting telemetry from datacenters. GPU vendors can push signed drivers within weeks, not years.

**Fusion Watchfloor**: National compute auditors correlate Model Run Notices with cloud logs, network flows, and power telemetry. Even basic anomaly detection can flag undeclared training within this timeframe.

**$50M Whistleblower Bounties**: Using existing financial crime frameworks, authorities can authorize bounties worth 10-30% of collected fines, with immunity for incidental participation. The SEC's program has paid nearly $2 billion in similar schemes—big bounties make leaks near-certain.

### Phase 2: Market-Led Adoption (Months 3-6)

Creating voluntary adoption through competitive advantage:

**Performance Bonds and Insurance Markets**: Lloyd's and Munich Re begin offering $250M minimum bonds for frontier runs, creating market pressure for compliance. Labs that can't get insurance can't train legally.

**"Verified Compute" Premium Features**: NVIDIA and AMD implement hardware-anchored attestation as a premium feature, marketed as essential for enterprise trust. Cloud providers offer Hardware Security Module weight protection as a differentiating service tier.

**Dynamic Threshold Adjustments**: The first quarterly recalibration accounts for the ~16-month doubling time of algorithmic efficiency, preventing actors from gaming static FLOP limits through improved techniques.

### Phase 3: Financial Leverage (Months 6-12)

Economic pressure forces broader compliance:

**Extraterritorial Enforcement**: Foundry access and export licenses become contingent on compute passport compliance. Secondary sanctions target facilitators of non-compliant training.

**International Inspectorate**: Starting with voluntary peer review between aligned nations (UK, Canada, Japan), "anywhere, anytime" inspection teams gain authority for boot-level verification. The model follows IAEA precedents but adapted for digital infrastructure.

### Phase 4: Infrastructure Hardening (Months 12-18)

Embedding verification in hardware itself:

**On-Die Compute Passports**: Next silicon tapeouts include embedded secure elements that cryptographically sign all operations. This makes circumvention require semiconductor manufacturing capability—raising the bar from software to hardware attacks.

**Conditional Infrastructure Aid**: World Bank facilities for pre-certified datacenters include built-in telemetry as a loan condition. Kenya, Philippines, and Chile pilot programs demonstrate the model.

### Technical Architecture: Making Detection Work

The detection pipeline operates on a simple principle: frontier training creates distinctive signatures across multiple observable channels. By correlating these signals, we can achieve ≥90% detection recall with ≤5% false positives:

```
Key Detection Features:
- Synchronized all-reduce operations with 10-60 second patterns
- Sustained power draw 5-15% above normal during nights/weekends
- Distinctive kernel execution patterns (matmul/attention sequences)
- Network bursts matching gradient exchange signatures
- Thermal anomalies visible from satellite imagery
```

The compute passport schema captures sufficient telemetry without exposing proprietary model architectures:

```
Core Telemetry (collected every 30 seconds):
- GPU serial and host fingerprint
- Kernel operation class (not full code)
- Accumulated FLOP count
- Instantaneous power draw
- Memory bandwidth utilization
- Cryptographic signature anchored to hardware root of trust
```

### Success Metrics and Realistic Expectations

The system doesn't need to be perfect—it needs to make legitimate pathways more attractive than circumvention:

**6-Month Targets**:
- 80% of accelerators in member states emitting telemetry
- 3+ frontier labs voluntarily adopt enhanced measures
- First successful threshold adjustment based on efficiency gains

**12-Month Targets**:
- Detection latency <24 hours for GPT-4 scale training
- No undetected frontier training for 6+ consecutive months
- Distributed training costs 5× premium versus compliant facilities

**18-Month Targets**:
- 40+ nations participating in inspection framework
- Haven state problem substantially mitigated through sanctions
- Next-generation hardware includes embedded attestation

### Critical Uncertainties and Adaptations

This implementation faces genuine challenges that require continuous adaptation:

**Technical Uncertainties**: Can 10 million existing GPUs be retrofitted with secure attestation? Will cryptographic overhead stay below 0.1% performance impact? How do we enable legitimate distributed research while preventing covert training?

**Policy Uncertainties**: Where exactly is the line between training, fine-tuning, and inference? Is G7 participation sufficient, or is China essential? How do we detect violations without creating surveillance infrastructure ripe for abuse?

**Economic Uncertainties**: Will compliance costs entrench incumbents at the expense of innovation? Can financial sanctions overcome sovereignty claims? How do we price insurance for unprecedented AI risks?

The framework addresses these through built-in adaptation mechanisms: 30-month sunset clauses force regular reauthorization, quarterly threshold adjustments prevent static gaming, and published impact assessments maintain transparency.

### The Window Is Closing

Between our initial red-teaming exercise and publishing this analysis, 0G Labs demonstrated distributed training at scale with China Mobile—proving that one of our theoretical risks has already materialized. The implementation roadmap must begin immediately, not after years of negotiation.

The next 90 days are critical. Emergency measures using existing authority can create momentum for comprehensive governance. The alternative—waiting for unanimous international agreement—guarantees that circumvention pathways will be exploited before controls are in place.

## Strategic Implications for AI Safety

This analysis reveals three fundamental insights for AI governance:

First, even innovative regulatory approaches like those in the Narrow Path, with their novel "found systems" definitions, safety cases, and multi-tier thresholds, face structural challenges when governing AI development. The technology's unique characteristics demand continuous evolution and enhancement of governance mechanisms.

Second, perfect enforcement is impossible; our goal must be raising circumvention costs while maintaining adaptive capacity. This means accepting that some level of non-compliance will occur while working to minimize its impact and detect it quickly.

Third, technical verification must be built into the computational substrate itself. Post-hoc detection and enforcement cannot match the speed of digital proliferation. By the time a violation is detected through traditional means, the damage may be irreversible.

## Conclusion: The Window of Opportunity

The challenges outlined here establish requirements for designing governance that might actually work. Twenty years might provide sufficient time to solve alignment challenges and develop robust international institutions, but only if we acknowledge and address these fundamental circumvention pathways from the outset.

Success depends not on assuming compliance but on anticipating creative non-compliance. We must design systems robust to partial adherence, fragmented enforcement, and determined adversaries. This means integrating verification into hardware, updating oversight rules before they become obsolete, and aligning economic incentives with safety goals.

The four horsemen of ASI moratorium circumvention (regulatory flight, distributed swarms, covert state programs, and proxy datacenters) represent fundamental challenges even to sophisticated governance frameworks like the Narrow Path. Addressing them requires continuous innovation and enhancement in how we approach AI safety governance.

Perfect control remains unachievable. The question is whether we can raise the bar high enough, quickly enough, to buy time for alignment research and institutional development. The window for implementing effective governance narrows with each passing month. Our response must be proportional to both the magnitude of the opportunity and the severity of the risk.

As we stand at this technological crossroads, we must remember that the goal centers on ensuring progress proceeds safely. The circumvention pathways analyzed here represent challenges that demand careful design, international cooperation, and technical innovation. The future of AI governance depends on our willingness to confront these challenges honestly and develop solutions that match the unique nature of the technology we seek to govern.

The path forward requires neither naive optimism nor paralyzing pessimism, but rather clear-eyed analysis coupled with determined action. With the EU AI Act now in force and divergent national strategies emerging, the window for unified global governance narrows daily. The stakes could not be higher, and the time for half-measures has passed.

## About This Research

This analysis represents our first major foray into AI governance research, emerging from a systematic red-teaming exercise that won first place in Apart Research's hackathon. As researchers new to governance, we bring an outsider's perspective that may catch vulnerabilities that domain experts, immersed in existing frameworks, might miss.

We're not stopping here. Through Apart Lab Studio, we're continuing to develop practical solutions to the governance challenges identified in this analysis, with mentorship from the ControlAI team who bring real-world policy implementation experience. Our ongoing work focuses on three areas:

1. **Technical verification mechanisms** that can be implemented without waiting for international consensus
2. **Economic incentive structures** that make compliance more attractive than circumvention
3. **Adaptive governance frameworks** that can evolve as fast as the technology they seek to regulate

We believe that effective AI governance requires both fresh perspectives and deep expertise—which is why we're combining our adversarial analysis approach with guidance from established governance practitioners.

## Join the Conversation

This analysis represents just one attempt to stress-test AI governance proposals. We need more minds working on these challenges:

**For Researchers & Technologists:** What circumvention pathways have we missed? Can you identify technical solutions to the vulnerabilities outlined here? Share your analysis and proposals.

**For Policymakers:** Adversaries may already be following these blueprints. How can we update current frameworks to address these specific threats?

**For Everyone:** The future of AI governance affects us all. Share this analysis with others who care about getting AI safety right. Challenge our assumptions. Propose better solutions.

Have you identified additional vulnerabilities in proposed AI governance frameworks? Do you see solutions we've overlooked? Join the discussion and help strengthen our collective approach to AI safety.

*The window for effective action is narrowing. Let's use it wisely.*

## Technical Glossary

### Computing Thresholds & Metrics

**FLOPs (Floating-Point Operations)** - Standard unit for measuring computational work in AI training. One FLOP equals one basic arithmetic operation (addition, multiplication, etc.) on decimal numbers.

**10^25 FLOP** - Total compute budget for GPT-4-class training, now adopted by EU AI Act as threshold for systemic risk classification.

**10^17 FLOP/s** - Proposed licensing threshold for compute facilities under moratorium frameworks.

**10^13 FLOP/s** - Individual accelerator threshold for mandatory cryptographic attestation monitoring.

**Exascale (10^18 FLOP/s)** - Current supercomputer tier operated by major powers, theoretically capable of GPT-4 training in 2 weeks vs 6 months on commercial hardware.

**Gradient compression** - Bandwidth optimization transmitting only significant gradient updates, achieving 100x reduction to enable training over home internet connections.

### Security & Verification Infrastructure

**Merkle log** - Append-only cryptographic data structure where each entry includes hash of all previous entries, preventing retroactive falsification of compute logs.

**Hardware Security Module (HSM)** - Tamper-resistant cryptographic device proposed for storing model weights with attestation requirements for any checkpoint access.

**Compute passports** - Proposed embedded secure elements in GPUs that cryptographically sign device ID, power draw, and kernel execution patterns to immutable logs.

**Salted hash** - One-way cryptographic fingerprint with added randomness, allowing public verification of model checkpoints without revealing actual weights.

### Historical Precedents & Programs

**Biopreparat** - Soviet biological weapons program (1974-1991) employing 60,000 people across 52 facilities while violating BWC, demonstrating feasibility of large-scale covert technical programs.

**CoCom controls** - Cold War technology export regime circumvented through shell companies and falsified end-user certificates, precedent for modern dual-use restrictions.

**Folding@home** - Distributed computing achieving 1.5 exaFLOPS through voluntary participation, exceeding top 100 supercomputers combined.

**Smominru botnet** - Cryptocurrency mining malware infecting 500,000+ machines generating $8,500/day (2018), demonstrating distributed compute monetization at scale.

**DiLoCoX/0G Labs** - December 2024 breakthrough with China Mobile achieving 10x speed improvement in distributed training over 1 Gbps networks, proving feasibility of decentralized frontier model development.

### Regulatory Mechanisms

**The Narrow Path** - Specific 20-year ASI moratorium proposal requiring licenses for training >10^25 FLOP, compute facilities >10^17 FLOP/s, with 12-day breakout detection windows.

**SDR (Special Drawing Rights)** - IMF reserve currency basket used for nuclear liability calculations (300M SDR minimum), proposed basis for AI development bonds.

**MTCR (Missile Technology Control Regime)** - Voluntary 35-nation agreement limiting missile proliferation, demonstrating both successes and failures of non-binding technology governance.

**Vienna Convention diplomatic pouches** - Sealed containers with legal immunity from inspection, potential vector for physical transfer of model weights between nations.

**Secondary sanctions** - Penalties on third parties doing business with primary violators, key enforcement mechanism when primary actors operate from non-compliant jurisdictions.

### Distributed Training Infrastructure

**Asynchronous gradient updates** - Training protocol allowing nodes to contribute improvements without synchronized coordination, enabling fault-tolerant operation across heterogeneous hardware.

**Backbone flow patterns** - Detectable network signatures at internet exchanges revealing synchronized data transfers characteristic of distributed training operations.

**Edge computing nodes** - Distributed processing infrastructure ostensibly for 5G/IoT, potentially repurposable as disaggregated training clusters below facility thresholds.