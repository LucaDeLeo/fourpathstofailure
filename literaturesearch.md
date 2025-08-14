
Annotated Bibliography: AI Governance Circumvention and Countermeasures


Literature for Pathway 1: Jurisdiction Shopping & Regulatory Arbitrage


Pollman, E. (2019). Tech Regulatory Arbitrage and Limits. ResearchGate.

Annotation: This article defines regulatory arbitrage as the strategic maneuvering by firms to exploit gaps or differences between regulatory regimes, often by moving operations to a more favorable jurisdiction.1 It uses examples like Facebook modifying its terms to avoid strict European privacy laws and Uber classifying workers as non-employees to illustrate the concept. The source directly supports the theoretical underpinnings of the "Jurisdiction Shopping" pathway described in the research draft.2 Its analysis of how tech companies with global growth goals pursue rapid expansion in markets with relaxed regulations to gain consumer buy-in before restrictive rules can be enforced provides a clear behavioral model for how a well-funded AI lab could establish itself in a permissive "AI Innovation Zone" to preempt a global moratorium. The source's focus on the tech industry makes its arguments particularly salient.

Froomkin, A. M. (1997). The Internet as a Source of Regulatory Arbitrage. Miami Herbert Business School.

Annotation: This foundational paper from the early commercial internet era explains how the internet's transnational nature enables regulatory arbitrage, allowing actors to structure transactions to evade domestic regulations by leveraging foreign legal regimes.3 It specifically discusses the concept of "offshore data havens" used to circumvent national laws on data protection and censorship. This provides a direct historical precedent for the draft's "AI Innovation Zone".2 The paper's argument that a single country can do little to prevent its citizens from communicating with the rest of the world without crippling the medium's value is directly analogous to the challenge of enforcing a global AI moratorium; a state that defects to become a haven could gain significant economic and technological advantages, making complete enforcement difficult.

WiCell Research Institute. (n.d.). Our Mission and History.

Annotation: This source provides a powerful, real-world historical analogue for the "Jurisdiction Shopping" pathway. It documents that the WiCell Research Institute was explicitly established in 1999 by the Wisconsin Alumni Research Foundation as a "safe haven for the advancement of stem cell research in the politically charged environment of the time".4 This was a direct response to unclear and restrictive federal regulations in the United States regarding human embryonic stem cell (hES) research. This case corroborates the draft's hypothesis 2 that a sub-national or national entity would proactively create a permissive regulatory environment to attract scientific talent and capital when a dominant power imposes restrictions on a controversial, high-stakes technology. The fact that WiCell went on to host the National Stem Cell Bank and trained over 800 scientists globally demonstrates the success of this strategy.

University of Miami Institute for Bioethics and Health Policy. (n.d.). National Stem Cell Policy Timeline.

Annotation: This timeline details the legislative and scientific history of stem cell research in the U.S. and globally, providing crucial context for the "jurisdiction shopping" analogy. It documents the 2001 Bush administration policy restricting federal funding for new hES cell lines 5, and the subsequent reaction by states like California, which passed Proposition 71 in 2004 to establish a constitutional right to conduct stem cell research and created a state-level funding institute.6 This directly supports the draft's claim that restrictive policies in one major jurisdiction can trigger the creation of well-funded, permissive "havens" in others. The timeline shows that rather than halting research, the federal restrictions catalyzed a fragmentation of the regulatory landscape, a dynamic the draft predicts for AI governance.2

Sustainability Directory. (n.d.). How Does Regulatory Arbitrage Affect Developing Nations?

Annotation: This source explains the concept of "pollution havens," where developing nations attract investment from polluting industries by offering weaker or poorly enforced environmental regulations.8 This serves as a strong historical analogue for the "AI Innovation Zone" proposed in the draft.2 The analysis highlights the motivations of the "haven" state—the desire for foreign investment, jobs, and economic growth—which makes them vulnerable to this form of regulatory arbitrage. This refutes a simplistic view of jurisdiction shopping as purely illicit; rather, it frames it as a symbiotic, if detrimental, relationship. The source's point that companies often export older, dirtier technologies to these havens could be paralleled by AI companies deploying less safe or unaligned models in jurisdictions with weaker safety standards.

Debevoise & Plimpton. (2025). The Federal AI Moratorium is DOA; What's Next for State AI Regulation?

Annotation: This legal analysis provides a contemporary, real-time example of the dynamics that enable jurisdiction shopping. It reports on the failure of a proposed federal moratorium on state-level AI regulation in the U.S. and the subsequent proliferation of differing state AI bills.9 The article notes that a key reason comprehensive state laws have stalled is "Innovation Concerns," where governors and industry argue that "burdensome frameworks could drive AI talent and capital to another state".9 This directly validates the core competitive dynamic described in the draft's "Jurisdiction Shopping" pathway 2, demonstrating that even within a single country, the fear of capital flight to less-regulated jurisdictions is a primary driver of policy.

Literature for Pathway 2: Distributed GPU Swarms


Qi, J., et al. (2025). DiLoCoX: A Low-Communication Large-Scale Training Framework for Decentralized Cluster. arXiv.

Annotation: This paper provides the strongest piece of technical evidence supporting the feasibility of the "Distributed GPU Swarms" pathway. The authors introduce DiLoCoX, a framework explicitly designed to train massive models (over 100 billion parameters) on slow, decentralized networks analogous to a consumer-grade swarm.10 They report successfully pre-training a 107B parameter model over a 1Gbps network, achieving a 357x speedup compared to standard AllReduce methods while maintaining model convergence.11 This directly addresses the core technical challenge of the GPU swarm scenario: the communication bottleneck. The framework's success, achieved by combining pipeline parallelism with advanced adaptive gradient compression, strongly suggests that the draft's back-of-the-envelope calculation for training time might be plausible or even pessimistic if such advanced algorithms are used.2 It shifts the feasibility question from raw hardware aggregation to the proliferation of sophisticated distributed training software.

Folding@home. (2021). 2020 in Review and Happy New Year 2021!

Annotation: This blog post provides a powerful proof-of-concept for the "Distributed GPU Swarms" pathway by documenting the success of a massive, real-world volunteer computing project. In 2020, Folding@home aggregated over 280,000 GPUs and 4.8 million CPU cores from volunteers, becoming the world's first "exascale computer" and surpassing the most powerful conventional supercomputers of the time.13 This demonstrates that it is technically possible to harness a vast, heterogeneous, and unreliable network of consumer devices for a single, massive computational task. While the project was for public good, it validates the core premise of the draft's scenario 2 that sufficient consumer-grade compute can be aggregated to reach frontier-level scale.

Zhang, L., et al. (2023). Evaluation and Optimization of Gradient Compression for Distributed Deep Learning. arXiv.

Annotation: This paper evaluates the real-world performance of gradient compression methods, a key enabling technology for the "Distributed GPU Swarms" pathway. The authors find that common compression techniques (quantization, sparsification, low-rank) do not always outperform well-optimized standard training and can be incompatible with system optimizations like all-reduce and pipelining.14 However, they propose a novel method, ACP-SGD, that achieves an average 4.06x speedup over standard distributed training. This source nuances the draft's claims 2 by showing that simply applying any gradient compression is not enough; the specific algorithm and its system compatibility are critical. It supports the pathway's feasibility but underscores that success would require a high degree of technical sophistication from the non-state actor organizing the swarm.

Sharma, S., et al. (2025). Characterizing the Impact of Overlapping Communication and Computation in Distributed Deep Learning. arXiv.

Annotation: This research directly challenges the simple utilization assumptions made in the draft's back-of-the-envelope calculation for a GPU swarm. The paper analyzes the performance of distributed training on high-end data center GPUs (A100s, H100s) and finds that the necessary overlapping of communication and computation leads to an average computational slowdown of 18.9%, with a maximum of 40%.15 This performance degradation occurs even in a best-case scenario with high-speed, reliable interconnects. For a distributed swarm operating over the public internet with high latency and unreliability, the performance penalty would be substantially worse. This evidence suggests that the 20% utilization figure in the draft's BOTEC 2 may be highly optimistic, and the time-to-train could be significantly longer unless extremely effective communication-mitigation algorithms are employed.

Literature for Pathway 3: Covert State Programs


Chas Bartolome, C. (2022). Biopreparat: The Soviet Union’s Biological Weapons Programme and its Challenge to the BWC. Kent's Consortium for World Affairs.

Annotation: This paper provides a concise and powerful historical analogue for the "Covert State Programs" pathway. It describes the Soviet Union's "Biopreparat" system as a "massive clandestine effort which concealed a vast network of biological weapons research, development, testing, and production facilities under the direction of an organisation known as Biopreparat".16 The program successfully operated in violation of the 1972 Biological Weapons Convention (BWC) for decades. Crucially, the paper highlights that the full extent of the program was only revealed following the defection of high-placed insiders, Vladimir Pasechnik and Kanatjan Alibekov. This directly corroborates the draft's claims that a state can run a large-scale, long-term covert program and that external inspections are likely to be ineffective, making whistleblowers a critical detection vector.2

Alibek, K. (2001). Statement of Dr. Ken Alibek to the U.S. House of Representatives.

Annotation: As the former First Deputy Chief of Biopreparat, Dr. Ken Alibek's testimony provides an unparalleled insider's account of the Soviet biological weapons program. He confirms the program's enormous size and sophistication, its continuation and intensification after signing the 1972 BWC, and its focus on developing agents for which no cure existed.17 Most relevant to the "Covert State Programs" pathway, Alibek notes that when trilateral inspections with the US and UK were conducted in 1991, the program was still active, and "the Soviets covered up the evidence as best they could".17 This first-hand account strongly supports the draft's premise that a determined state can successfully deceive international inspectorates, rendering them ineffective at uncovering a well-concealed, high-priority clandestine program.2

Leitenberg, M. (2005). The Soviet Biological Weapons Program and Its Legacy in Today's Russia. National Defense University.

Annotation: This paper analyzes the strategic motivations and institutional structure of the Soviet BW program, offering deep insights into why a state would pursue such a path. It explains that the modern program, which began around 1972, was driven by the desire to leverage new technologies—specifically genetic engineering—to create militarily superior weapons.18 This motivation is directly analogous to a state's potential desire to covertly develop AGI to gain a decisive strategic advantage. The paper also clarifies that the program was concealed within a civilian component called Biopreparat, while the military planning was codenamed "Ferment".18 This detailed description of the dual-structure (a civilian face for a military project) provides a concrete model for how a state could repurpose exascale supercomputers for AI development under the guise of unclassified scientific research, as hypothesized in the draft.2

Wikipedia. (n.d.). Soviet biological weapons program.

Annotation: This encyclopedic overview synthesizes multiple sources to describe the history and scale of the Soviet BW program. It notes the program began in the 1920s and employed up to 65,000 people at its peak across dozens of secret sites, with an annualized production capacity of 90-100 tons of weaponized smallpox.19 The sheer scale and longevity of the program provide a stark historical precedent for the draft's claim that a state can sustain a massive, secret, and treaty-violating program for decades.2 The fact that this was accomplished with 20th-century technology suggests that a modern state with advanced surveillance and security capabilities could be even more effective at concealing a clandestine AI development program.

Literature for Pathway 4: Offshore Proxy Datacenters


Cohen, A., & Frankel, S. (2018). Israel's Nuclear Deception: Flagrant Lies and Brazen Hypocrisy. The Daily Star.

Annotation: This article details the extensive deception campaign Israel employed to conceal its nuclear weapons program at the Dimona reactor. It documents how Israeli officials provided numerous cover stories, claiming the facility was a "textile plant" or a "meteorological installation," and publicly insisted it was for "peaceful purposes" while knowing this was false.20 This historical case directly supports the draft's premise that a client state in an "Offshore Proxy Datacenter" scenario could use deception and plausible deniability to mask the true purpose of its AI facilities.2 The article highlights that even when U.S. scientists were granted access, their ability to uncover the truth was limited, a point further elaborated in other sources showing how inspections were managed and thwarted.

Wikipedia. (n.d.). Shimon Peres Negev Nuclear Research Center.

Annotation: This source provides critical details on how Israel managed and ultimately neutralized the effectiveness of international inspections at its Dimona nuclear facility, serving as a powerful analogue for the "Offshore Proxy Datacenter" pathway. It states that when U.S. inspections were permitted from 1965-1969, Israel knew the schedule in advance and was able to "hide the clandestine manufacture of nuclear weapons... by installing temporary false walls and other devices before each inspection".21 The inspectors eventually concluded their work was "useless" due to these restrictions. This provides a direct, verifiable historical precedent for the draft's claim that a client state, by controlling access and using concealment tactics, can successfully defeat an inspection regime while invoking sovereign rights.2

Congressional Research Service. (2025). China's Nuclear and Missile Proliferation.

Annotation: This CRS report documents China's long-standing role as a supplier of nuclear and missile technology to other states, most notably Pakistan and Iran.22 It provides evidence that even after joining the Nuclear Suppliers Group (NSG) and agreeing to its export controls, "Chinese entities" have continued to supply missile-applicable items to Pakistan's ballistic missile program, leading to U.S. sanctions as recently as 2024. This source strongly corroborates the fundamental premise of the "Offshore Proxy" pathway: that a major power may act as a sponsor, providing a client state with sensitive, proliferation-relevant technology despite international agreements designed to prevent such transfers. The ongoing nature of these transfers shows the persistence of such strategic relationships.

Siddi, M. (2011). The China-Pakistan Nuclear Deal: Realpolitique and the 'Fait Accompli'. Nuclear Threat Initiative.

Annotation: This analysis examines China's agreement to sell additional nuclear reactors to Pakistan after joining the Nuclear Suppliers Group (NSG), an act that seemingly violated its NSG commitments. China justified this by "grandfathering" the new reactors under previous agreements, a move the NSG did not formally approve but ultimately acquiesced to.23 This case is highly relevant to the "Offshore Proxy" pathway because it demonstrates how a sponsor state (China) can use legalistic interpretations and geopolitical leverage to continue supplying a client state (Pakistan) with sensitive technology in defiance of a multilateral control regime. It suggests that a sponsor of a proxy AI datacenter could similarly exploit loopholes or present the international community with a
fait accompli, betting that other nations will choose accommodation over confrontation.

The Heritage Foundation. (1998). The Strategic Implications of China's Nuclear Aid to Pakistan.

Annotation: This report analyzes the geopolitical motivations behind China's nuclear assistance to Pakistan, framing it as a strategic tool to counterbalance their mutual regional rival, India.24 This provides a crucial layer of understanding for the "Offshore Proxy Datacenter" pathway. It suggests the motivation for such a partnership is not merely to circumvent a technical rule (like a compute threshold) but to achieve a larger geopolitical objective. A sponsor state in an AI context would similarly use a client state to gain an indirect AGI capability, maintain plausible deniability, and challenge the strategic position of its rivals who are adhering to a moratorium. This reframes the pathway from a simple circumvention tactic to a deliberate act of strategic competition.

Literature for Countermeasure: Universal Cryptographic Attestation ("Compute Passports")


NVIDIA. (2022). NVIDIA H100 Tensor Core GPU Architecture.

Annotation: This technical white paper provides the foundational evidence that the draft's "Compute Passports" concept is grounded in existing technology. It details the security features of the Hopper architecture, including second-generation Secure Multi-Instance GPU (MIG) and, most importantly, Confidential Computing.25 The paper explains that H100 is the first GPU with capabilities to create a hardware-based Trusted Execution Environment (TEE), which secures and isolates workloads. Critically, it describes features like a hardware Root of Trust (RoT), Secure and Measured Boot, and device attestation, which allow a user to "verify that they are communicating with authentic NVIDIA GPUs... and that the security state of the GPU matches a known, trusted secure state".25 This is the core technical function required for a "Compute Passport" to prove a chip's identity and integrity, confirming the technical plausibility of the countermeasure.2

Garfinkel, B., et al. (2024). Computing Power and the Governance of AI. Centre for the Governance of AI.

Annotation: This paper lays out the comprehensive argument for why compute is a uniquely effective intervention point for AI governance, which is the strategic foundation for the "Compute Passports" countermeasure. It identifies four key properties of AI-relevant compute: it is detectable, excludable, quantifiable, and produced via an extremely concentrated supply chain.26 These properties are what make a scheme like attestable hardware plausible in the first place. However, the paper also provides a crucial balancing perspective by outlining the risks and limitations of compute governance, including incentives for circumvention (e.g., smuggling), the potential for low-compute models to still be dangerous, and the risk of algorithmic progress making compute a less reliable proxy for risk over time.26 This source allows for a nuanced assessment of the "Compute Passport" idea, grounding its potential while soberly acknowledging its inherent challenges.

NVIDIA. (2022). NVIDIA H100 Tensor Core GPU Datasheet.

Annotation: This official datasheet confirms and summarizes the key security features of the H100 GPU relevant to the "Compute Passports" proposal. It explicitly lists "NVIDIA Confidential Computing" as a breakthrough feature of the Hopper architecture, making the H100 the "world's first accelerator with confidential computing capabilities".27 The document states that this feature allows users to "protect the confidentiality and integrity of their data and applications in use".27 By marketing this as a key security feature for enterprise and data center customers, NVIDIA demonstrates that there is commercial demand for hardware-level security and attestation. This supports the idea that the technological components of a "Compute Passport" system are not just theoretical but are being actively developed and deployed in high-end, commercially available hardware.

Literature for Countermeasure: International Inspectorate (IAEA Analogy)


Gruemm, H. (1982). Potential and limitations of international safeguards. IAEA Bulletin.

Annotation: This article from a former IAEA Deputy Director General provides a candid, early assessment of the nuclear safeguards regime, offering crucial lessons for any proposed "IAEA for AI." Gruemm states that expectations of what safeguards can achieve are often "rather inflated" and that the system is fundamentally an "ex post facto warning system," not a prevention mechanism.28 He explicitly notes that "safeguards cannot prevent the diversion of nuclear material" and that the "risk of proliferation is greatest where safeguards end"—i.e., at undeclared facilities. This directly challenges the notion that an IAEA-style inspectorate could be a robust defense against a determined cheater, corroborating the circumvention pathways in the draft 2 and suggesting that such an inspectorate for AI would inherit, and likely amplify, these fundamental limitations.

Sustainability Directory. (n.d.). IAEA Safeguards Regime.

Annotation: This source explains the structure and evolution of the IAEA safeguards system, highlighting a key weakness that is directly relevant to an AI inspectorate. It notes that the original system, based on Comprehensive Safeguards Agreements (CSAs), was focused on verifying declared nuclear material at declared facilities. The discovery of Iraq's clandestine nuclear program in the 1990s revealed the system's inability to detect undeclared activities, which led to the creation of the more intrusive Additional Protocol (AP) to grant the IAEA enhanced access to information and locations.29 This historical evolution strongly suggests that an "IAEA for AI" would be similarly vulnerable to undeclared, covert training runs (as in Pathway 3) unless it was granted extremely intrusive inspection powers from the outset, which would likely be politically infeasible.

Taylor & Francis Online. (2024). Quantifying Safeguards Innovations: Impacts of Innovations on International Atomic Energy Agency Safeguards Inspection Effort.

Annotation: This academic paper analyzes the efficiency of the IAEA safeguards regime, noting the immense and growing demands on its resources despite a relatively flat budget.30 The verification workload is driven by the increasing amount of nuclear material, the number and complexity of facilities, and the expanding scope of safeguards agreements. This provides a crucial reality check for the proposal of an "IAEA for AI." An AI inspectorate would face an even more complex and rapidly evolving landscape. The verification task would not be tracking a physical substance but auditing intangible code, data, and model weights across a vast and diverse global digital infrastructure. The resource and expertise requirements would be immense, suggesting that, like the IAEA, it would likely be perpetually under-resourced relative to its mandate.

Literature for Countermeasure: Whole-of-Network Detection


Kentik. (n.d.). The Network Impact on Job Completion Time in AI Model Training.

Annotation: This industry blog post explains that large-scale AI model training creates distinctive network traffic patterns, or "IO storms," as thousands of GPUs communicate and synchronize.31 It details how a network intelligence platform can use high-resolution flow telemetry to monitor this traffic, identify congestion hotspots, and even map traffic patterns to specific training job IDs. This directly supports the technical feasibility of the "fusion watchfloor" countermeasure proposed in the draft.2 It confirms that the all-reduce communication inherent in distributed training creates a detectable network signature that could be monitored at key internet choke points (like IXPs) to identify potentially illicit large-scale training runs.

Multilogin. (n.d.). What is Traffic Fingerprinting?

Annotation: This article provides an accessible explanation of "traffic fingerprinting," a technique that analyzes traffic metadata (packet sizes, timing, frequency) to identify online activities even when the content is encrypted.32 This concept is the foundation for the network analysis component of the draft's "fusion watchfloor" countermeasure. The source explains how different applications (e.g., video streaming vs. messaging) have unique traffic "shapes." This principle could be applied to identify the unique, highly structured, and intense communication patterns of a large-scale AI training run, distinguishing it from other forms of high-volume data traffic and thereby serving as a key signal for detecting covert AI development.

ResearchGate. (2025). Edge AI-Based Fraud Detection System for Smart Grid Power Monitoring.

Annotation: This research paper proposes an edge AI system to detect electricity fraud by monitoring power parameters like current, voltage, and power factor in real-time.33 It uses machine learning models (SVM and LSTM) to detect anomalies and irregular consumption patterns. This directly supports the technical feasibility of the power-grid monitoring component of the draft's "fusion watchfloor".2 While the paper focuses on individual consumer fraud, the same principles of non-intrusive load monitoring and anomaly detection could be applied at the substation or grid level to detect the massive and sustained power draw of an undeclared, large-scale datacenter, providing another critical signal for the detection system.

University of Chicago. (2025). University of Chicago Researchers Revolutionize Network Traffic Generation with AI Breakthrough.

Annotation: This article discusses NetDiffusion, an AI framework for generating realistic synthetic network traffic to train better cybersecurity models.34 While its purpose is to improve defense, it highlights a key challenge for the "fusion watchfloor" countermeasure: the adversarial nature of detection. A sophisticated actor attempting to hide a large training run could use similar generative techniques to create cover traffic that mimics benign activity, thereby masking the true signature of their AI workload. This source suggests that any detection system based on traffic fingerprinting will be engaged in a continuous cat-and-mouse game with adversaries developing techniques to evade it, complicating the draft's assumption of a high-confidence detection probability.

Literature for Countermeasure: Whistleblower Bounty Programs


U.S. Securities and Exchange Commission. (2021). 2021 Annual Report to Congress: Whistleblower Program.

Annotation: This official report from the SEC provides powerful empirical evidence for the effectiveness of a large-scale whistleblower bounty program. It states that in FY 2021 alone, the program awarded approximately $564 million to 108 individuals, and that since the program's inception, information from whistleblowers has led to enforcement actions with nearly $5 billion in financial remedies.35 The report also highlights the program's global reach, noting that it received over 12,200 tips in FY 2021 from individuals in 99 foreign countries. This strongly supports the draft's proposal for a whistleblower bounty program as a key countermeasure, demonstrating that substantial financial awards are highly effective at incentivizing insiders—including foreign nationals—to report illicit activities.

National Whistleblower Center. (n.d.). Assessing the SEC's Whistleblower Reward Program.

Annotation: This analysis corroborates the success of the SEC's whistleblower program, calling it a "tremendously effective force-multiplier" that generates high-quality tips and "virtual blueprints laying out an entire enterprise".36 Critically, it provides a statistic that directly counters a common objection to such programs: that they undermine internal compliance. The report finds that approximately 83% of award recipients who were employees first raised their concerns internally before reporting to the SEC. This suggests that a bounty program does not replace internal reporting but acts as a crucial backstop when internal channels fail. This is a vital point for justifying such a program in the AI governance context, as it would incentivize insiders in covert programs (Pathways 3 and 4) to come forward when no other recourse is available.

U.S. Government Accountability Office. (2011). Securities and Exchange Commission: Securities Whistleblower Incentives and Protections.

Annotation: This GAO report reviews the initial rulemaking for the SEC whistleblower program established under the Dodd-Frank Act.37 It details the legal foundation and intended purpose of the program, which was to pay awards to individuals who provide original information leading to successful enforcement actions. This source is valuable as it establishes the official, congressionally mandated basis for what has become a highly successful program. It provides the legal and regulatory blueprint that could be adapted to create an international whistleblower program for detecting and reporting violations of an AI development moratorium, grounding the draft's proposal in established U.S. legal precedent.
Works cited
Tech, Regulatory Arbitrage, and Limits - ResearchGate, accessed on August 14, 2025, https://www.researchgate.net/publication/345391172_Tech_Regulatory_Arbitrage_and_Limits
Perfect Implementation Isn't Enough: Four Ways an ASI Moratorium Could Fail - LessWrong, accessed on August 14, 2025, https://www.lesswrong.com/posts/efvrNLwwtJLrHDWDM/perfect-implementation-isn-t-enough-four-ways-an-asi
The Internet As A Source Of Regulatory Arbitrage - Pottinger Volunteer Page - University of Miami, accessed on August 14, 2025, https://osaka.law.miami.edu/~froomkin/articles/arbitr.htm
Our Mission and History - WiCell Research Institute, accessed on August 14, 2025, https://www.wicell.org/home/about-us/our-mission-and-history/our-mission-and-history.cmsx
Embryonic Stem Cell Research: A Decade of Debate from Bush to Obama - PMC, accessed on August 14, 2025, https://pmc.ncbi.nlm.nih.gov/articles/PMC2744932/
National Stem Cell Policy Timeline | Institute for Bioethics | University of Miami, accessed on August 14, 2025, https://bioethics.miami.edu/education/timelines-project/national-stem-cell-policy-timeline/index.html
Understanding the Proposed AI Moratorium: Answers to Key Questions - R Street Institute, accessed on August 14, 2025, https://www.rstreet.org/ai-moratorium-questions/
How Does Regulatory Arbitrage Affect Developing Nations? → Question - Pollution → Sustainability Directory, accessed on August 14, 2025, https://pollution.sustainability-directory.com/question/how-does-regulatory-arbitrage-affect-developing-nations/
The Federal AI Moratorium is DOA; What's Next for State AI Regulation? | 07 | 2025 | Publications - Debevoise & Plimpton LLP, accessed on August 14, 2025, https://www.debevoise.com/insights/publications/2025/07/the-federal-ai-moratorium-is-doa-whats-next
DiLoCoX: A Low-Communication Large-Scale Training ... - arXiv, accessed on August 14, 2025, https://arxiv.org/abs/2506.21263
0G Labs Achieves Breakthrough in Decentralized AI Training With 100 Billion+ Parameters, accessed on August 14, 2025, https://www.dlnews.com/external/0g-labs-achieves-breakthrough-in-decentralized-ai-training-with-100-billion-parameters/
0G Labs Achieves Breakthrough in Decentralized AI Training With ..., accessed on August 14, 2025, https://thedefiant.io/news/press-releases/0g-labs-achieves-breakthrough-in-decentralized-ai-training-with-100-billion-parameters
2020 in review, and happy new year 2021! – Folding@home, accessed on August 14, 2025, https://foldingathome.org/2021/01/05/2020-in-review-and-happy-new-year-2021/
[2306.08881] Evaluation and Optimization of Gradient Compression for Distributed Deep Learning - arXiv, accessed on August 14, 2025, https://arxiv.org/abs/2306.08881
Characterizing Compute-Communication Overlap in GPU-Accelerated Distributed Deep Learning: Performance and Power Implications - arXiv, accessed on August 14, 2025, https://arxiv.org/html/2507.03114v1
Biopreparat: The Soviet biological weapons programme - Research at Kent, accessed on August 14, 2025, https://research.kent.ac.uk/kcwa/wp-content/uploads/sites/2496/2022/03/Carmen-Chas_Biopreparat_KCWA_2022.pdf
Statement by Dr. Kenneth Alibek Program Manager Battelle Memorial Institute - The Climate Change and Public Health Law Site, accessed on August 14, 2025, https://biotech.law.lsu.edu/blaw/bt/smallpox/Congress/Alibek01.htm
The Soviet Biological Weapons Program and Its Legacy in Today's Russia, accessed on August 14, 2025, https://inss.ndu.edu/Media/News/Article/848285/the-soviet-biological-weapons-program-and-its-legacy-in-todays-russia/
Soviet biological weapons program - Wikipedia, accessed on August 14, 2025, https://en.wikipedia.org/wiki/Soviet_biological_weapons_program
Israel's nuclear deception: Flagrant lies and brazen hypocrisy - The Daily Star, accessed on August 14, 2025, https://www.thedailystar.net/opinion/views/news/israels-nuclear-deception-flagrant-lies-and-brazen-hypocrisy-3921676
Shimon Peres Negev Nuclear Research Center - Wikipedia, accessed on August 14, 2025, https://en.wikipedia.org/wiki/Shimon_Peres_Negev_Nuclear_Research_Center
China: Nuclear and Missile Proliferation - Congress.gov, accessed on August 14, 2025, https://www.congress.gov/crs-product/IF11737
The China-Pakistan Nuclear Deal: A Realpolitique Fait Accompli, accessed on August 14, 2025, https://www.nti.org/analysis/articles/china-pakistan-nuclear-deal-realpolitique-fait-accompli-1/
The Strategic Implications of China's Nuclear Aid to Pakistan | The Heritage Foundation, accessed on August 14, 2025, https://www.heritage.org/asia/report/the-strategic-implications-chinas-nuclear-aid-pakistan
NVIDIA H100 Tensor Core GPU Architecture - Advanced Clustering ..., accessed on August 14, 2025, https://www.advancedclustering.com/wp-content/uploads/2022/03/gtc22-whitepaper-hopper.pdf
Computing Power and the Governance of Artificial Intelligence, accessed on August 14, 2025, https://cdn.governance.ai/Computing_Power_and_the_Governance_of_AI.pdf
NVIDIA H100 Tensor Core GPU Datasheet - Megware, accessed on August 14, 2025, https://www.megware.com/fileadmin/user_upload/LandingPage%20NVIDIA/nvidia-h100-datasheet.pdf
Potential and limitations of international safeguards, accessed on August 14, 2025, https://www.iaea.org/sites/default/files/publications/magazines/bulletin/bull24-0/24003484043su.pdf
IAEA Safeguards Regime → Term - Energy → Sustainability Directory, accessed on August 14, 2025, https://energy.sustainability-directory.com/term/iaea-safeguards-regime/
Full article: Quantifying Safeguards Innovations: Impacts of Innovations on International Atomic Energy Agency Safeguards Inspection Effort - Taylor & Francis Online, accessed on August 14, 2025, https://www.tandfonline.com/doi/full/10.1080/25751654.2024.2364962
The Network Impact on Job Completion Time in AI Model Training | Kentik Blog, accessed on August 14, 2025, https://www.kentik.com/blog/the-network-impact-on-job-completion-time-in-ai-model-training/
What is Traffic Fingerprinting? - Multilogin, accessed on August 14, 2025, https://multilogin.com/glossary/traffic-fingerprinting/
Edge AI-Based Fraud Detection System for Smart Grid Power Monitoring - ResearchGate, accessed on August 14, 2025, https://www.researchgate.net/publication/388837864_Edge_AI-Based_Fraud_Detection_System_for_Smart_Grid_Power_Monitoring
University of Chicago Researchers Revolutionize Network Traffic Generation with AI Breakthrough, accessed on August 14, 2025, https://cs.uchicago.edu/news/university-of-chicago-researchers-revolutionize-network-traffic-generation-with-ai-breakthrough/
2021 ANNUAL REPORT TO CONGRESS - Whistleblower Program - SEC.gov, accessed on August 14, 2025, https://www.sec.gov/files/2021_ow_ar_508.pdf
Assessing the SEC's Whistleblower Reward Program, accessed on August 14, 2025, https://www.whistleblowers.org/when-whistleblowers-get-rewards-assessing-the-secs-whistleblower-reward-program/
Securities and Exchange Commission: Securities Whistleblower Incentives and Protections | U.S. GAO, accessed on August 14, 2025, https://www.gao.gov/products/gao-11-764r
