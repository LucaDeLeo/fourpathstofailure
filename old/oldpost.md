# **Perfect Implementation Isn’t Enough: Four Ways an ASI Moratorium Could Fail**

By Vishakha Agrawal, Damin Curtis, Luca de Leo, Heramb Podar, Zoe Roy-Stang, Ben Smyth

# **Summary**:

In this post, we identify four mechanisms by which an international moratorium on Artificial Super-Intelligence (ASI) development could fail by allowing determined actors to circumvent regulations:

1. **Regulatory Havens**
2. **Distributed GPU Swarms**
3. **Hidden State Supercomputers**
4. **Proxy Datacenters**

This red-teaming post discusses these regulatory issues, drawing historical analogies to understand their root causes and consequences.

While this post was written as a red-teaming exercise on ‘Phase 0’ of [*A Narrow Path*](https://www.narrowpath.co/), a policy proposal for an international moratorium on Artificial Super-Intelligence, we believe that these failure modes are broadly applicable to international AI governance proposals targeting frontier capabilities training.

# Introduction

Imagine the walled city of medieval Constantinople. The Eastern Roman Empire had invested centuries into building the best-defended city in the world, with three layers of exquisitely engineered stone walls and a massive lowerable chain blocking ships from entering the golden horn, the waterway running parallel to the city. Every gate guarded, every parapet manned, from a distance it looked impenetrable—and for over a thousand years, it was—until in 1453, when Sultan Mehmed II finally took the millennium-old city. His strategy included four novel methods: digging tunnels beneath the walls, silently rolling entire naval ships over a hill to circumvent the waterway’s chain, unveiling some of the largest cannons ever deployed, and weaponizing sheer exhaustion through a relentlessly long blockade to wear down and outlast the defenders.

A determined adversary doesn’t always need to storm the battlements, and impenetrable defenses are worthless if attackers find a way around.

That, in essence, is the dynamic baked into *Phase 0* of ‘A Narrow Path’ by ControlAI: a proposed policy for implementing a global moratorium on training Artificial Super-Intelligence (ASI). ASI refers to an AI system, or collection of systems, that decisively outperforms the best human minds across virtually every cognitive task: strategy, science, invention, or persuasion. Its arrival could unlock enormous benefits or catastrophic risks, depending on who controls it and under what constraints. The moratorium’s goal is straightforward: buy humanity two safe decades to solve alignment, build institutions, and avoid a reckless race to build the first ungovernable ASI capabilities.

However, as we outline below, there are structural loopholes in this policy proposal. Even if every signatory nation enacts the rules flawlessly—licensing datacentres, tracking chips, auditing training runs—there remain four routes that a well-resourced actor can exploit without ever “breaking” the rules on paper.

History warns that bold bans often falter at the margins. Nuclear fuel cycles, bioweapon labs, even strong encryption protocols all slipped through gaps that looked tiny on the drafters’ parchment but massive in the real world. When economic and strategic incentives collide with partial enforcement, optimisation pressure pushes every actor toward whatever space remains unregulated. In cryptography it was offshore servers; in nuclear proliferation, “supplier-club” loopholes; in bioweapons, secret state labs shielded by national-security carve-outs. Advanced AI will be no different unless regulators can learn from historical examples and anticipate how adversaries will adapt.

# The “Narrow Path” Proposal Explained

At its core, the proposed moratorium that is the subject of our redteaming exercise seeks to prevent the development of Artificial Super-Intelligence for twenty years, buying time to develop the science and institutions needed to deal with ASI’s arrival safely.

Their proposed ASI-development freeze operates through four mechanisms:

1. **Prohibition of ASI Development and Capabilities that could Lead to ASI**
   A ban on funding, enabling, or performing any development, testing, or deployment of ASI. Specific dangerous capabilities are banned (namely those that could trigger an intelligence explosion or a rogue AI system).
2. **Mandatory Safety Cases for Advanced AI Systems**
   The moratorium would require that developers demonstrate models will not empower dangerous capabilities (e.g. AI self-improvement, self-replication, expert persuasion, or expert knowledge of chemical and biological weapons) before they even start training.
3. **Comprehensive Licensing and Regulatory Oversight of Advanced AI**
   National regulatory bodies would implement a tiered licensing regime for the creation, distribution, or use of advanced AI systems. A Training License would be required for model training runs above 1025 FLOPS, and a Compute License would be required for cloud compute providers operating above 1017 FLOPS (and maintaining this licence would require know-your-customer measures and physical GPU tracking to prevent smuggling/covert use), and an Application License would be required to deploy new use-cases for models.
4. **Create 12-Day Detection Windows**
   This ban proposes authorities monitor electricity grid usage to detect any non-licensed compute centers.

# Four Paths to Failure

We performed a red-teaming exercise on the Narrow Path moratorium proposal . For the purpose of this exercise, we assume successful enactment of the moratorium's four safeguards: compute licensing, training registration, capability bans, and 12-day detection windows. Our read-teaming therefore asks the question: “even if these are implemented successfully, are there other critical flaws we need to take into account?” An overarching concern is that this moratorium can only cover what can be regulated: only detectable datacenters in signatory nations. Those seeking to circumvent regulation will also optimize around avenues which are difficult to regulate in practice.

Our analysis identified four primary breach scenarios:

1. **Regulatory Flight**: A well-resourced actor could relocate their operations to a jurisdiction that does not sign the treaty. AI models, unlike physical weapons, can be trained in one jurisdiction and then instantly transmitted/accessed in another.
2. **Distributed GPU Swarms**: Training runs could be fragmented across tens of thousands of consumer graphics cards, each legally below licensing thresholds. This method could allow a model to be covertly trained without a large compute footprint, allowing its development to “hide” from regulators and outlast the shuttering of individual nodes of its training infrastructure.
3. **Covert State Supercomputers**: Classified compute infrastructure (e.g. underground structures resilient to detection/sabotage) could be deployed for ASI training. State-approved covert resources prove difficult to expose without whistleblowers, allowing state actors to circumvent international agreements.
4. **Offshore Proxy Datacenters**: An actor could partner with, say, a middle-income nation, offering "infrastructure loans" and technical assistance to build modular, distributed data centers disguised as other services (e.g., 5G edge computing nodes). These facilities could be located on military bases or universities, and host nations could invoke sovereignty arguments to resist inspections.

Each path bypasses a different cornerstone safeguard; together they sketch a blueprint for how the moratorium could fail despite perfect paperwork.

## The Four Paths: Historical Analogies

1. ### **Regulatory Flight**

#### Historical Parallel: The A.Q. Khan Network

For over 30 years, Pakistani metallurgist A.Q. Khan ran the world's most successful nuclear proliferation network. Despite comprehensive export controls and Western intelligence tracking, [Khan supplied nuclear technology to Libya, Iran, and North Korea until 2004](https://sgp.fas.org/crs/nuke/RL34248.pdf). His method? Operate from Pakistan (outside the NPT), use shell companies in Dubai and Malaysia, and exploit diplomatic immunity.
An AI company could execute the same playbook, with one crucial advantage. Unlike centrifuges, AI models can be delivered instantly over the internet.

#### The Modern Mechanism

Picture "FrontierAI Corp", a well-funded Silicon Valley startup. When the moratorium takes effect, they face a choice: abandon years of research or find a friendlier jurisdiction. Like [FTX moving to the Bahamas to avoid SEC oversight](https://www.reuters.com/legal/bankman-fried-appeals-ftx-fraud-conviction-25-year-sentence-2024-04-11/), they choose regulatory arbitrage.

They identify "Technopolis"—a small nation eager for investment that sees AI leadership as its path to relevance. Within weeks of the moratorium taking effect, Technopolis offers:

* Streamlined incorporation in their "AI Innovation Zone"
* 10-year tax holiday
* Fast-track visas for 200 engineers
* Explicit exemption from AI restrictions

The relocation mirrors Khan's blueprint. Through shell companies in Singapore, Dubai, and Malta, FrontierAI acquires 40,000 H100 GPUs. The hardware arrives at Technopolis's free port in unmarked containers, expedited through customs without inspection.

Within eighteen months, they have a fully operational facility, and may have a commercial GPT-4+ model ready for release. But here's where AI differs from nuclear weapons: the trained model sits behind innocuous API endpoints on global content delivery networks. A London user connects to what looks like a chatbot, unaware they're accessing a system trained entirely outside the moratorium.

#### How We Know This Works

The pattern of regulatory arbitrage repeats across domains:

* Nuclear: Khan's network evaded controls for 30+ years using the exact shell company structure
* Biotech: In 2001, after the US government cut federal funding for human embryonic stem cell research, [research became concentrated in US states with higher funding and other countries with more flexible regulation](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0120052)
* Cryptography: In 1991, Phil Zimmermann wrote and distributed “Pretty Good Privacy”, an open-source software program used to encrypt and decrypt emails. Pretty Good Privacy was the first widely available program implementing public-key cryptography. The program and source code were soon distributed outside of the United States, allegedly violating US export controls. [In response to a criminal investigation, Zimmerman published the source code as a book to bypass these regulations](https://philzimmermann.com/EN/essays/index.html).
* Financial: FTX relocated in 3 months; Binance banned US customers from using its services and established a US-compliant subsidiary, Binance.US, which [secretly taught US customers](https://www.forbes.com/sites/michaeldelcastillo/2020/10/29/leaked-tai-chi-document-reveals-binances-elaborate-scheme-to-evade-bitcoin-regulators/) how to bypass geographic restrictions to engage in unregulated trading.

2. ### **Distributed GPU Swarms**

#### Historical Parallel: From Napster to Neural Networks

When courts shut down Napster in 2001, file-sharing didn't die—it evolved. Gnutella swapped central servers for decentralized peer-to-peer (P2P) file-sharing, making it much harder to shut down. BitTorrent made every downloader an uploader, meaning that the efficiency of file-sharing scaled with the amount of users downloading a file. In January 2012, BitTorrent had [over 150 million](https://www.bittorrent.com/blog/2012/01/09/bittorrent-at-ces-outstanding-consumer-electronics-partners-150-million-users-and-counting/) monthly active users. Although P2P file-sharing has largely been eclipsed by commercial streaming services, the BitTorrent protocol demonstrates how swarms of basic computers (such as laptops) can replace large servers while efficiently distributing large files across a network. Similar protocols could leverage unsuspecting individuals’ personal computers to conduct distributed frontier AI training runs that are invisible to regulators.

#### The Modern Mechanism

"The Collective" starts as a subreddit of frustrated AI researchers. Traditional data centers require licenses and trigger inspections. But modern gaming computers rival yesterday's supercomputers, and millions sit idle overnight.

* Phase 1: Technical Foundation: Engineers develop "NeuralTorrent"—software fragmenting AI training across consumer GPUs. Using gradient compression algorithms, they reduce communication needs 100x, enabling training over home internet.
* Phase 2: Recruitment: Through gaming forums and crypto communities, they recruit with a simple pitch: "Earn $500/month while you sleep." To authorities, it looks like crypto mining—legal and untrackable.
* Phase 3: Invisible Scale: Within months, 50,000 participants across 60 countries run NeuralTorrent. Each node operates below thresholds, but collectively they rival major facilities.

#### How We Know This Works

Real-world precedents prove the scale:

* Folding@home: A distributed computing project, relying on volunteers’ personal computers to assist in simulating protein folding, reached 1.51018 FLOPS fighting COVID—[more than the world's top 100 supercomputers combined](https://www.tomshardware.com/news/folding-at-home-breaks-exaflop-barrier-fight-coronavirus-covid-19).
* Smominru botnet: A botnet is a network of private computers, infected with malicious software and controlled as a group without the owners’ knowledge. The Smominru botnet infected [over 500,000 Windows servers and personal computers](http://www.securityweek.com/crypto-mining-botnet-ensnares-500000-windows-machines/), capable of both stealing personal data and leveraging computing power to mine cryptocurrency. In January 2018, this botnet was [mining the equivalent of $8500USD a day](https://www.proofpoint.com/us/threat-insight/post/smominru-monero-mining-botnet-making-millions-operators).

The engineering is virtually solved—only coordination remains.

3. ### **Covert State Supercomputers**

#### Historical Parallel: The Biopreparat Cover-Up

From 1974-1991, the Soviet Union operated [Biopreparat](https://en.wikipedia.org/wiki/Biopreparat): 60,000 people across 52 facilities developing bioweapons while party to the Biological Weapons Convention. Facilities masqueraded as pharmaceutical plants. A 1979 accident killed 100 people in Sverdlovsk, yet the program stayed hidden until defector Vladimir Pasechnik exposed it. If 60,000 people kept that secret for 16 years, imagine what a classified AI program could achieve with 200 people.

#### The Modern Mechanism

Country X operates exascale supercomputers for climate modeling, nuclear simulations, and cryptanalysis. These facilities already employ thousands and consume city-scale power under highest classifications. When the moratorium begins, intelligence suggests adversaries might cheat. The temptation proves irresistible: why not "borrow" existing supercomputers?
The beauty lies in invisibility:

* Zero new infrastructure: No construction to detect, no purchases to trace.
* Perfect cover: Job names use existing terminology.
  * "atmospheric\_dynamics\_v7" → transformer pretraining
  * "molecular\_simulation\_q3" → reinforcement learning
* Built-in security: Staff already have clearances.
* Speed: What takes Google 6 months takes 2 weeks on weapons-simulation hardware.

#### How We Know This Works

There is a repeating pattern of nation states developing prohibited military technology by co-opting legitimate research and industry facilities:

* Iraq's nuclear program: Built complete facilities under IAEA monitoring using "materials production" cover.
* Soviet Biopreparat: 16 years of dual-use vaccine production hiding weapons research.
* Israel’s Dimona nuclear facility: With the aid of France, Israel built covert nuclear facilities and began manufacturing atomic weapons. Upon discovery, the facility was labelled a “textile plant” and later a nuclear research centre built for “peaceful purposes”. US inspectors were deceived by the Israelis [bricking over elevators and hallways](https://nuke.fas.org/guide/israel/nuke/) that would have allowed access to certain areas of the facility.

Lesson: Inspectors can only inspect declared facilities. Dual-use makes detection impossible without insiders.

4. ### **Offshore Proxy Datacenters**

#### Historical Parallel: The Pakistan-China Template

Throughout the 1980s-90s, China provided Pakistan with weapons-grade uranium, warhead blueprints, and missile technology, thereby violating the NPT for decades. When confronted, both nations invoked sovereignty–neither recognized third-party authority over bilateral relations. This sovereign shield enables AI development through untouchable proxy relationships.

#### The Modern Mechanism

"MegaCorp," a trillion-dollar tech giant, sees the moratorium as existential. Companies developing AGI first dominate; compliant ones become irrelevant. They need territorial sanctuary.

Enter Computia, a middle-income nation seeking modernization. MegaCorp offers:

* $2 billion in "infrastructure loans"
* Technical assistance for "national cloud computing"
* Training for 5,000 engineers
* Joint "National AI Laboratory"

But the facility design is masterful. Instead of one detectable data center, they build 40 modular units:

* Each has 200 GPUs—below licensing thresholds
* Disguised as "5G edge computing nodes"
* Distributed across military bases and universities
* Connected via "critical infrastructure" fiber

When monitors request access, Computia invokes sovereignty:

* "These support essential government functions"
* "Foreign inspection compromises national security"
* "We're fully treaty compliant"
* "Bilateral partnerships aren't subject to review"

Technically true—Computia agreed to avoid developing AI, but not to prevent others using its territory.

For Computia, it's their largest foreign investment. For MegaCorp, it's less than their jet budget.

#### How We Know This Works

Sovereignty consistently trumps controls:

* Pakistan-China nuclear: Transfers tracked from 1977 but unstoppable until 1998 tests.
* North Korea missiles: Sold to Iran, Syria, and Libya despite the Missile Technology Control Regime.
* Huawei data centers: Built facilities leaving government servers open to exfiltration; host nations cited sovereignty when questioned.

Within 7 months, the distributed facility trains a frontier model. Weights transfer through diplomatic pouches—legally untouchable. Computia keeps a copy for "national research," ensuring mutual vulnerability.

### **The Compounding Crisis**

These paths don't exist in isolation. Once one succeeds, others follow:

* Haven states attract investment after early profits
* Distributed networks share techniques openly
* Classified programs cite suspected violations to justify expansion
* Proxy relationships proliferate as countries seek AI partners

History shows this pattern with nuclear proliferation, crypto controls, and bioweapons. The terrifying reality: all four paths could activate simultaneously. While diplomats debate, FrontierAI operates from havens, The Collective coordinates swarms, classified supercomputers run experiments, and proxy facilities multiply globally.

Traditional controls assume visible infrastructure, corporate compliance, and state cooperation. But when AI development can hide in regulatory gaps, fragment across networks, disappear into classified programs, or shelter behind sovereignty, those assumptions shatter.

# The Fixes (Brief)

As part of our red-teaming exercise, we proposed a three layer solution, which is not covered in this post. However, we will include here the high-level overview:

**One system, three layers** that raise detection odds, shrink response time, and flip incentives. Each layer helps alone; together they make cheating costly.

* **Layer 1 — “Compute passports”**
  High-end chips prove who they are and what they ran via tamper-evident logs; missing or fake logs make illicit clusters easier to spot.
* **Layer 2 — Adaptive oversight**
  Don’t freeze rules: update capability thresholds on a cadence and fuse multiple signals (attestation logs, network patterns, power/heat) to catch swarms without flooding false positives.
* **Layer 3 — Human intelligence & incentives**
  Unannounced inspections, protected/bountied whistleblowing, and risk-weighted performance bonds add unpredictability and real costs for rule-breaking.

### **Quick, practical moves**

* [**If-then commitments**](https://carnegieendowment.org/research/2024/09/if-then-commitments-for-ai-risk-reduction?lang=en)**:** Publish initial capability triggers **and** commit to a 6-month recalibration cycle.
* **Prototype verifiable compute:** Chipmakers \+ clouds pilot an open attestation spec on a limited SKU.
* **Aid templates:** Offer pre-approved datacenter designs with built-in verification hooks.
* **Fused-signals cell:** Voluntary data from major grids/IXPs/clouds to validate swarm signatures.
* **Model laws:** Enact whistleblower protections and performance bonds.

History’s great fortifications—from Constantinople’s triple walls to nuclear nonproliferation treaties—rarely fall because their designers were careless. They fall because adversaries look for the edges, not the center, and exploit whatever cracks remain open. A moratorium on Artificial Super-Intelligence will be no different.

# Conclusion

History’s great fortifications—from Constantinople’s triple walls to nuclear nonproliferation treaties—rarely fall because their designers were careless. They fall because adversaries continually look for the edges, the subtle weaknesses, and exploit whatever they find. A moratorium on Artificial Super-Intelligence will be no different.

Our red-teaming exercise shows that even a flawlessly implemented Phase 0 moratorium could fail—not through open defiance, but through circumvention. Regulatory havens, distributed GPU swarms, covert state supercomputers, and offshore proxy datacenters each present credible, historically grounded routes for determined actors to continue ASI development under the radar. If history is any guide, once one of these routes is proven viable, the others will follow, compounding the challenge.

The point is not that a moratorium is doomed, but that its success depends on anticipating how it might fail. That means designing governance systems that assume partial compliance, fragmented enforcement, and adaptive adversaries. It means building technical verification into compute hardware, updating oversight rules before they become obsolete, and backing regulations with human intelligence and economic incentives that make cheating costly. If we can buy humanity even twenty years to solve alignment, develop better institutions, and prepare for what's coming, that might be enough.
