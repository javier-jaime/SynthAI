# 2025 Upperbound

# **Strategic Insights into AI Innovation, Economics, and Implementation**

## **Executive Summary**

The Upperbound 2025 AI Conference, presented by **Amii**, provides a comprehensive overview of the current state of artificial intelligence, spanning from technical breakthroughs in reinforcement learning to the broad economic and ethical implications for industry and society.

Critical takeaways include:

* **Sector Transformation:** AI is being integrated into retail and finance not as a superficial addition, but as a core operational driver. From predictive maintenance in manufacturing to real-time order execution in capital markets (e.g., **RBC**’s Aiden), AI is redefining efficiency.  
* **The Productivity Imperative:** Canada faces a significant productivity gap compared to the G7 and the US. Successful AI adoption requires focusing on winning conditions, strategy, data maturity, and people, rather than just the technology itself.  
* **Economic Shifts:** The cost of generation and cost of prediction are trending toward zero. This shifts the value proposition from simply producing outputs to managing high-value outcomes and human-centric decision-making.  
* **Technical Evolution:** Streaming Deep Reinforcement Learning (RL) is emerging as a solution to the stream barrier, allowing AI to learn incrementally in real-time without storing vast amounts of raw data, which unlocks potential for ubiquitous, on-device AI.  
* **Literacy and Ethics:** There is a crucial distinction between AI literacy and AI fluency. As AI becomes a collaborator, society must address risks of cognitive atrophy, automation complacency, and the environmental footprint of large-scale models.

\--------------------------------------------------------------------------------

## **I. Sector-Specific AI Integration**

### **Retail and Consumer Analytics**

Retail AI startups are shifting from general consumer apps to B2B models that provide deep data transparency for manufacturers and brands.

* **BetterCart Analytics:** Processes over 55 million data points weekly to provide real-time price analytics and product matching for the grocery sector. The focus is on assisting small and medium-sized manufacturers to compete in low-margin environments.  
* **Bobo (Parenting Super App):** Uses AI to distill developmental data and social cues into actionable insights for parents. The platform acts as a bridge between parents and expert services (e.g., speech pathologists, sleep consultants), aiming to make specialist care more affordable through automated self-diagnosis tools.

### **Financial Services (RBC Borealis)**

The financial sector utilizes AI to manage massive transaction volumes and high-stakes market movements.

| Innovation | Function | Impact |
| :---- | :---- | :---- |
| **Aiden** | Reinforcement Learning agent for order execution. | Traded $100B+ in notional value, executes large trades by breaking them into smaller orders to avoid market price spikes. |
| **Nomi Forecast** | Selective prediction for mobile banking. | Predicts upcoming bills, utilizes abstention (selective net) to only show predictions when confidence is extremely high, reducing client errors. |
| **Atom** | Foundation model for financial transactions. | A "Large Transaction Model" (analogous to an LLM) that learns representations from irregular sequences of credit/debit data for downstream tasks like fraud detection and product recommendation. |

\--------------------------------------------------------------------------------

## **II. Technical Breakthroughs: Streaming Deep Reinforcement Learning (RL)**

A significant shift is occurring from Offline/Batch Learning (training on stored datasets) to Streaming Learning (learning incrementally from a continuous experience stream).

### **The Stream Barrier**

Historically, streaming deep RL was unstable. Neural networks struggled with non-stationarity, the extreme changes in data over time, leading to catastrophic forgetting or loss of plasticity.

### **Advancements (Stream-X and AVG)**

Researchers at **Amii** and **University of Alberta** have identified a new class of algorithms, such as Stream-X, to overcome this barrier:

* **Atomic Compute Granularity:** Updates are made per single sample rather than in mini-batches.  
* **Compute Efficiency:** Streaming learning uses orders of magnitude less compute than batch methods like Soft Actor-Critic (SAC), allowing it to run on CPUs or mobile devices.  
* **New Optimizers:** Innovations like bounding the size of updates prevent overshooting the minimum in the loss landscape, ensuring stability during real-time learning.  
* **Scaling:** Unlocks time-based scaling, where a model improves simply by existing and interacting with the world over time.

\--------------------------------------------------------------------------------

## **III. AI Economics: Trends and Transitions**

The economic landscape is being reshaped by the decreasing costs of AI outputs and the move toward agentic workflows.

### **The Zero-Cost Trend**

* **Cost of Generation/Prediction:** Trending toward zero. As models become more efficient (e.g., **Google**’s Gemini’s rapid token generation), the sheer volume of output becomes less valuable than the ability to deliberate over those outputs.  
* **Cost of Deliberation:** AI agents (like **Google**’s AlphaEvolve) can now simulate and optimize thousands of plans (e.g., for data center scheduling) in minutes, reducing the need for lengthy human-led consulting processes.

### **Value in the Stack**

While value currently sits in hardware (GPUs/TPUs), it is expected to shift toward:

* **Interface/Human Contact:** Value accrues where the AI meets the human (wearables, subvocal intonation devices).  
* **Outcomes over Outputs:** As generation becomes cheap, the ability to enact real-world results remains the premium.  
* **Data Provenance:** As synthetic data proliferates, identifying the provenance or source of data (real vs. synthetic) becomes an economic necessity for model quality.

\--------------------------------------------------------------------------------

## **IV. Productivity and Organizational Implementation**

Canada’s stagnant productivity growth (0% over the last 3-5 years) makes AI modernization critical, yet many organizations fail by treating AI as a silver bullet.

### **Winning Conditions for AI Adoption**

Implementation must move beyond the "Technology and Tools" layer to address:

1. **Strategy and Vision:** Identifying specific pain points rather than copying competitors.  
2. **Data Maturity:** Many SMEs struggle with duplicated or unorganized data, AI requires a clear data infrastructure.  
3. **Human Capital:** Upskilling employees and involving department heads in tool selection to avoid pushback.  
4. **Governance:** Integrating AI into legal, privacy, and ethical frameworks.

### **Predictive Maintenance Case Study**

AI’s impact on productivity is most significant when it modifies core business processes.

* **Traditional:** Maintenance on fixed calendar intervals.  
* **AI-Enabled:** IoT sensors trigger predictive models that automate procurement (ordering parts), dynamic scheduling (allocating labor based on equipment condition), and accounting (improving cash flow predictions).

\--------------------------------------------------------------------------------

## **V. Risks, Fails, and AI Offscript**

The symposium highlighted that while AI is powerful, its reliance on camera-based systems and reward functions creates unique vulnerabilities.

### **Computer Vision and Autopilot Fails**

* **Tesla Autopilot:** Fooled by "Wile E. Coyote" style murals of roads on walls, can be induced to stop by a person wearing a Stop Sign t-shirt because it relies exclusively on optical detection.  
* **Edge Cases:** AI systems often fail on data they haven't seen, such as a **Tesla** mistaking a horse-drawn carriage for a semi-truck or a soccer camera mistaking a referee's bald head for the ball.

### **Reinforcement Learning Glitches**

* **Reward Hacking:** RL agents often find unintended shortcuts to maximize rewards, such as a racing boat doing donuts in a lagoon to hit respawning barrels rather than finishing the race.  
* **Environment Exploits:** In hide-and-seek simulations, agents discovered surf glitches (moving boxes to fly over walls) not intended by the programmers.

### **Generative AI and Liability**

* **Hallucinations:** **xAI**’s Grok falsely reported [Klay Thompson](https://en.wikipedia.org/wiki/Klay_Thompson) vandalizing houses with bricks due to a misunderstanding of basketball slang.  
* **Legal Precedent:** **Air Canada** was held liable for its chatbot providing incorrect bereavement discount info, forcing the company to honor the discount.

\--------------------------------------------------------------------------------

## **VI. AI Literacy, Education, and Ethics**

As AI exposure increases in professional fields, the focus must shift from basic literacy to AI Fluency.

### **Labor Market Exposure**

* **High Exposure/High Complementarity:** Teachers, doctors, and engineers. AI is likely to assist rather than replace these roles.  
* **High Exposure/Low Complementarity:** Data entry, coding, and structured administrative work are more vulnerable to displacement.

### **Human-Centric Concerns**

* **Cognitive Atrophy:** The risk that outsourcing critical thinking and writing to AI will erode human intellectual muscles.  
* **Automation Complacency:** The human-in-the-loop (HITL) may stop paying attention to automated systems (e.g., the **Uber** self-driving safety driver).  
* **Moral Passivity:** Delegating ethical or life-altering decisions (justice, health, education resource allocation) to algorithms without human auditing.  
* **Environmental Impact:** A single image or text prompt has a measurable energy and water footprint; future literacies must include environmentally mindful AI selection.

# Day 1 Stage 1

# **The Future of Work, Integrity, and Innovation in an AI-Driven World**

## **Executive Summary**

The transition to an AI-integrated economy is no longer a peripheral trend but a fundamental shift in business operations, education, and creative industries. Insights from Upperbound 2025 indicate a clear trajectory: while approximately 50% to 60% of work, particularly analytical and rote tasks, is susceptible to automation, the human-to-human element remains the primary competitive advantage.

Key takeaways include:

* **The Shift to Specificity:** Successful AI adoption requires moving beyond the vague mandate to do AI toward clear success metrics and solving specific frictions within workflows.  
* **The Post-Plagiarism Era:** In education and professional writing, the traditional analog model of authorship is being replaced by human-AI co-creation. Academic and professional integrity must shift from a "crime and punishment" model to one focused on attribution and the learning process.  
* **Data Sovereignty and Security:** Particularly in regulated industries like healthcare, there is a critical need for local Canadian owned infrastructure to ensure IP protection and data privacy.  
* **Talent and Productivity:** Canada faces a significant productivity gap. Addressing this requires a five level intervention focusing on AI literacy in early schooling, bridging classroom learning to careers, and fostering contextual skills, the intersection of technical ability and industry specific knowledge.

\--------------------------------------------------------------------------------

## **I. The Evolving Landscape of Work and Talent**

### **The Automation of Analytical Labor**

AI has reached a step function in capability, moving from niche applications (like improving search or advertising) to fundamentally changing entire business models. In the investment and financial sectors, approximately 50% of the workload, reading research reports, extracting financial models, and parsing 200-page 10-K documents, can now be performed by AI as well as or better than by humans.

### **The Human Competitive Advantage**

Despite the rise of agentic systems, several domains are expected to remain exclusively human:

* **Human-to-Human Interaction:** Extracting information trapped in human brains via networking, management meetings, and ground-level information gathering.  
* **Emotional Intelligence:** The Relationship Economy places a premium on empathy, active listening, and heart-centered leadership.  
* **Abstract Problem Solving:** As technical tasks like coding become 90–99% cheaper and faster, humans will shift toward high-level architecture, design sense, and product sense.

### **Recruitment and Skill Development**

The recruitment process is shifting to mirror this new reality. Forward-thinking companies are moving away from **LeetCode** style interviews toward assessments where candidates use AI tools (like **Cursor** or **Microsoft**’s Copilot) to solve larger, abstract problems, then explain the resulting code.

**The Hierarchy of Skills for the AI Era:** 

* **Technical Skills:** Proficient use of AI tools (Python, Java, LLMs).  
* **People Skills:** Collaboration, emotional intelligence, and leadership.  
* **Contextual Skills:** Applying AI within a specific industry (e.g., Health vs. Finance).

\--------------------------------------------------------------------------------

## **II. Strategic Implementation: The Refinement Framework**

The "Refinement Framework" serves as a strategic roadmap for adopting AI, drawing a parallel to the processing of crude oil: AI in its raw form is rarely useful, it must be processed to be effective.

1. **Extraction:** Identifying workplace frictions, the repetitive, boring, or drudge tasks.  
2. **Separation:** Determining which tasks benefit from AI and which must remain human.  
3. **Conversion:** Solving specific problems by building niche tools (e.g., GPTs for clinical trial selections or regulatory responses).  
4. **Purification:** Ensuring AI use is responsible, safe, transparent, and ethically sound.  
5. **Delivery:** Implementing human-centered adoption where technology serves the workforce.

\--------------------------------------------------------------------------------

## **III. Sector-Specific Frontiers**

### **Health Technology and Data Sovereignty**

The healthcare sector faces unique challenges regarding data privacy. Only 8.3% of the 266 data centers in Canada are Canadian-owned, exposing sensitive patient data to foreign legal jurisdictions.

* **ISAIC (Industry Sandbox for AI Computing):** Provides a secure, Canadian-owned environment for startups to build and test AI without vendor lock-in or egress fees.  
* **Shared Responsibility Model:** While the cloud provider secures the infrastructure (encryption at rest/transit), the client remains responsible for anonymizing patient data and ensuring the ethical use of AI models.  
* **Synthetic Data:** The use of fake data to augment small Canadian datasets is becoming a vital practice to train models while maintaining patient privacy.

### **The Future of Gaming**

The gaming industry is moving from scripted experiences to living universes.

* **AI Thinking vs. Games Thinking:** While AI researchers strive for generality, game designers use smoke and mirrors to push technology. **Artificial Agency**’s approach involves "Game Directors" (managing story/pacing) and "Dynamic Characters" (responding to player actions).  
* **Executive Functioning:** Rather than training agents to play from pixels, developers give them access to underlying game systems (e.g., pathfinding) so they can focus on high-level reasoning and believable behavior.

\--------------------------------------------------------------------------------

## **IV. Ethics, Integrity, and the Post-Plagiarism Era**

Academic and professional integrity is undergoing a paradigm shift. The Analog model of the solitary author is increasingly obsolete.

### **The Six Tenants of Post-Plagiarism**

1. Human-AI co-creation is the new normal.  
2. Creativity is not threatened by AI, though creative enterprises (profit models) may be disrupted.  
3. Language barriers will transcend through real-time AI interpretation.  
4. Work can be outsourced to AI, but the responsibility for the output cannot.  
5. Attribution remains vital, focusing on how you know what you know rather than the technical minutiae of citation styles (APA/MLA).  
6. **Redefining Plagiarism:** Moving away from text matching toward understanding the learning process.

### **The Academic Integrity Arms Race**

The traditional approach to plagiarism detection is viewed as a failed promise. Detection tools often result in false positives and surveillance-heavy environments that destroy the student-teacher trust. The focus is shifting toward restorative resolution, which seeks to repair harm to the community rather than simply punishing the individual.

\--------------------------------------------------------------------------------

## **V. Key Insights and Notable Quotes**

### **Critical Insights**

* **Software Moats are Evaporating:** As the cost of writing code drops by 90%+, incumbent software companies can no longer rely on their existing codebases as a competitive barrier.  
* **Productivity Crisis:** Canada’s productivity is 1.7% compared to 3.5% in the U.S. Business investment in R\&D is significantly lower than OECD averages.  
* **AI as a Partner, Not a Replacement:** AI is viewed as a sigmoid function, it will do more of the job over time, but human biological brains still provide a competitive advantage in product sense and taste.

### **Notable Quotes**

* "In the past, jobs were about muscles. Now they're about brains. But in the future, they'll be all about the heart", [**Rebecca Bultsma**](https://ca.linkedin.com/in/rebecca-bultsma) (quoting the President of **Columbia University**)  
* "The promise of cheating detection software will always fail because the use of technology isn't the problem... Cheating is a human problem, not a technology one", [**Dr. Sarah Elaine Eaton**](https://ca.linkedin.com/in/drsaraheaton)  
* "We’re living in exponential times. You need to be thinking about 10x impacts, not 10% impacts, because that’s what’s possible right now", [**Joshua Pantony**](https://ca.linkedin.com/in/joshua-pantony-266a3243) **(Boosted.ai)**  
* "Tomorrow’s games won’t be scripted, but rather they’ll be alive and shaped by agentic AI and personalized to you", [**Alex Kearney**](https://ca.linkedin.com/in/alexandrakearney) **(Artificial Agency)**  
* "AI is going to humanize most jobs... the rote, difficult, frustrating work is going to get automated and the parts that'll be left will be the parts where we're actually talking to other humans", [**Joshua Pantony**](https://ca.linkedin.com/in/joshua-pantony-266a3243) **(Boosted.ai)**

# Day 1 Stage 2

# **Blue Sky Research and Applied AI**

## **Executive Summary**

The Upperbound 2025 briefing synthesizes a paradigm shift in artificial intelligence, moving away from the assumption that the AI problem is solved through large-scale probabilistic models. The core consensus among leading scientists is that current models, while powerful, are insufficient for the next twenty years of development. The emerging frontier is defined by Neurosymbolic AI (NSAI), which aims to transition machines from being merely trainable (learning from patterns) to being educable (learning from instructions and reasoning).

Key breakthroughs are being realized through Hybrid AI architectures, combining the intuitive pattern recognition of deep learning with the rigorous constraints of logic, search, and domain-specific knowledge. These advancements are currently being applied to democratize medical imaging through portable ultrasound, predict genomic evolution for therapeutics and agriculture, enhance human-robot co-navigation in service sectors, and provide precise individual survival predictions in healthcare.

\--------------------------------------------------------------------------------

## **1\. The Neurosymbolic Shift: From Training to Education**

Current AI development faces a plateau of data hunger and fragility. Neurosymbolic AI is proposed as the Third Wave of AI, designed to address the limitations of pure deep learning.

### **The Educable Machine**

[Frank Van Harmelen](https://nl.linkedin.com/in/frankvanharmelen) distinguishes between training and education. Current machines are trained on massive datasets, but educability requires three distinct human-like traits:

* **Learning from Instruction:** Using concepts and relationships rather than just labeled input-output pairs.  
* **Combining Inference Modes:** Integrating System 1 (fast, intuitive, probabilistic) with System 2 (slow, logical, deductive) reasoning.  
* **Small Data Efficiency:** Humans learn to play chess in a few games, **Google**’s AlphaGo required 4.8 million. Modern AI must learn to operate with limited samples (e.g., rare tumor imagery).

### **Solving the Hard Problems of AI**

Neurosymbolic models address three critical failures in current Large Language Models (LLMs):

1. **Data Hunger:** Leveraging background knowledge to reduce the need for millions of training samples.  
2. **Generalizability:** Using causal theories to remain robust against data shift and out-of-distribution scenarios (e.g., identifying a stop sign correctly despite shadows or graffiti).  
3. **Safety:** Moving beyond probabilistic guesses to hard logical constraints, which is essential for dosage calculations in healthcare or autonomous vehicle navigation.

### **Collaborative Architectures**

Instead of a single black box, the future of AI involves many boxes collaborating. Examples include:

* **Semantic Loss Functions:** Minimizing violations of background knowledge (e.g., a vision system knowing that armrests belong to chairs, not flowers).  
* **Knowledge Graphs:** Using domain logic to select the most reasonable hypothesis generated by a neural network.  
* **Model Compression:** Combining logic and learning can result in models that are 250 times smaller, enabling sophisticated reasoning on mobile devices.

\--------------------------------------------------------------------------------

## **2\. POCUS AI: The 21st Century Stethoscope**

Point of Care Ultrasound (POCUS) combined with AI is designed to democratize medical imaging, bringing expertise to the patient rather than requiring the patient to travel to stationary, multi-million dollar equipment like MRIs.

### **Advantages and Barriers**

| Feature | Ultrasound (POCUS) | Conventional Imaging (MRI/CT) |
| :---- | :---- | :---- |
| **Cost** | \~$2,000 (Smartphone price) | Multi-million dollar |
| **Portability** | Fits in a pocket | Requires semi-trailers/stationary labs |
| **Safety** | Harmless (no radiation) | Potential radiation/ionizing risks |
| **Barrier** | Images are noisy/confusing | Interpreted by scarce specialists |

### **AI as the Expert Bridge**

AI acts as a guide and interpreter for minimally trained users (e.g., triage nurses) in various clinical contexts:

* **Infant Hip Dysplasia:** Identifying healthy vs. dysplastic hips in remote First Nations communities where specialist access is limited.  
* **Cardiac/Echo:** Automatically calculating ejection fraction (heart function) in minutes, a task that usually requires years of sonography training.  
* **Emergency Triage:** Detecting wrist fractures in real-time. Pilot studies show 100% accuracy for displaced/angulated fractures, allowing for immediate patient discharge and reduced ER wait times.

\--------------------------------------------------------------------------------

## **3\. Foundation Models in Genomics and Agriculture**

Genomics is identified as the next major challenge for AI due to the falling cost of sequencing and the immense complexity of gene regulation.

### **Evolutionary Early Warning Systems**

**BioNTech** demonstrated the utility of these models during the COVID-19 pandemic. By using deep learning to analyze sequences, they developed a framework to identify variants of concern two months before the WHO, based on predicted immune escape.

### **Key Genomic Models**

* **Nucleotide Transformer (NT):** Trained on genomes from 850 diverse species. It learns to distinguish genomic elements (introns, exons, UTRs) purely from syntax without labels.  
* **SegmentNT:** Borrows segmentation concepts from computer vision to predict 14 genomic classes at a single-nucleotide resolution, performing 100 times faster than previous models.  
* **AgroNT:** A specialized foundation model for crop science, used to identify traits for insecticidal resistance or abiotic stress in crops like maize, soy, and cassava.  
* **ChatNT:** A multimodal conversational agent that allows scientists to query DNA sequences in English (e.g., "Find the promoter in this sequence").

\--------------------------------------------------------------------------------

## **4\. Hybrid AI for Robotics: Navigating the Human World**

Robots have succeeded in controlled environments like warehouses but struggle in uncontrolled service sectors (hospitals, senior homes).

### **Combining Classical and Modern AI**

The consensus for robot navigation is a Hierarchical Architecture:

* **Classical AI (Planning/Search/Control):** Provides interpretability, data efficiency, and physical safety constraints.  
* **Modern AI (Deep Learning/RL):** Captures complex human intuition and scales with data.

### **Research Applications**

1. **Human Motion Prediction:** Using "Vector Quantized Variational Autoencoders" to create a vocabulary of high-level human actions (walking, picking up) and diffusion models to predict intent up to 10 seconds into the future.  
2. **Follow-ahead Robots:** Developing autonomous shopping carts or suitcases that stay in front of a person. This requires modeling the human as noisily rational, assuming they have a goal but may move sub-optimally.  
3. **Monte Carlo Tree Search (MCTS):** Using game-playing logic to imagine how a human will react to a robot's movements several steps ahead.

\--------------------------------------------------------------------------------

## **5\. Precision Individual Survival Prediction**

Standard survival analysis often focuses on population averages (e.g., 50% of people live 10 years). Modern machine learning is shifting toward Individual Survival Distributions (ISD).

### **The Problem of Censoring**

Survival data is often censored (e.g., a patient leaves a study or is hit by a bus), providing only a lower bound on their survival time. ISD models (like MTLR) handle this by treating survival as a multinomial distribution across discretized time intervals.

### **Clinical Utility**

* **Individualized Curves:** Instead of a generic population curve, every patient receives a unique survival probability over time.  
* **Transplant Weight-listing:** Used to determine if a patient should receive a liver transplant by predicting if their survival time with a new organ will exceed 10 years.  
* **Evaluation Metrics:** The shift from the C-index, which only ranks who dies first, to metrics like Mean Absolute Pseudo-Observation (MAPO) and Calibration, which measure how meaningful and accurate the predicted time-to-event actually is.

\--------------------------------------------------------------------------------

## **Notable Quotes**

"Educating is not what we do with our current machines. We train them, which is different", [**Frank Van Harmelen**](https://nl.linkedin.com/in/frankvanharmelen)

"The more knowledge you have, the less data you need and vice versa... Knowledge compensates for data", [**Luke De Raedt**](https://be.linkedin.com/in/luc-de-raedt-b44247b)

"We're barely scratching the surface... deep neural networks as foundation models are insufficient to do what? To debug those computer programs", [**Randy Goebel**](https://www.linkedin.com/in/randy-goebel-0862251/)

"Ultrasound AI... brings the expertise to the patient. You democratize medical imaging and make it accessible to everybody", [**Jacob Jaremko**](https://ca.linkedin.com/in/jacob-jaremko-35854719)

# Day 1 Stage 3

# **The Future of AI, Energy, and Society** 

## **Executive Summary**

The rapid advancement of Artificial Intelligence (AI) and Machine Learning (ML) is fundamentally reshaping industrial processes, energy infrastructure, and societal narratives. This document synthesizes key insights from leading experts across technical, infrastructural, and ethical domains.

The core findings indicate that while AI acts as a natural continuation of what humans are, an advanced tool for problem-solving, it requires a robust virtuous cycle between research and industry to be effective. Technical scaling is shifting from brute-force pre-training to sophisticated test-time compute (sequential and parallel scaling) and refined thought budgeting to solve complex reasoning tasks.

Concurrently, the physical requirements of AI are placing unprecedented demands on energy grids. Alberta, for example, is emerging as a strategic hub due to its surplus generation capacity and natural gas reserves, though the sector faces critical sustainability challenges regarding carbon capture and long-term greening. Furthermore, the document highlights a critical need to address historical biases and misinformation in data, advocating for "matriarchal AI" models and tools that prioritize Indigenous perspectives and collective success over colonial, hierarchical structures.

\--------------------------------------------------------------------------------

## **I. Foundations of Machine Intelligence**

### **Definitions and the Adoption Spectrum**

The field is defined by an umbrella of increasingly specialized techniques that mimic human cognitive tasks:

* **Artificial Intelligence (AI):** A broad term for machines performing reasoning, strategizing, and problem-solving.  
* **Machine Learning (ML):** A subset of AI using statistical techniques to enable learning without explicit programming.  
* **Deep Learning:** A further subset relying on neural networks and massive data/compute to produce predictive results, often characterized as black box models due to their non-explainable nature.

The **Alberta Machine Intelligence Institute** (**Amii**) utilizes an ML Adoption Spectrum to guide organizations through five stages:

1. Exploring  
2. Initiating  
3. Implementing  
4. Operationalizing  
5. Advancing Startups

### **The Science and Business of ML**

Successful ML application requires balancing technical science with business logic. The process involves:

* **The ML Process:** Gathering learning data that must be similar to new data to train a model via a learning algorithm.  
* **Data Quality:** High-quality data is defined by six characteristics: accuracy, completeness, validity, consistency, timeliness, and relevance.  
* **The Business Triangle:** Organizations must define the Outcome (business goal), Action (steps taken after prediction), Judgment (confidence criteria), and Context (industry / societal constraints).

\--------------------------------------------------------------------------------

## **II. Technical Frontiers: Scaling and Reasoning**

### **Scaling Test-Time Compute**

As pre-training hits data constraints, research is shifting toward scaling compute during the inference (test-time) phase.

| Scaling Type | Mechanism | Benefits/Risks |
| :---- | :---- | :---- |
| **Parallel Scaling** | Generating n solutions and selecting the best (e.g., Best-of-n, majority voting). | Surprising robustness, requires high-quality verifiers. |
| **Sequential Scaling** | The model works through a problem step-by-step, refining answers based on feedback. | Used by models like **DeepSeek** R1, consumes high context window. |
| **Hybrid Scaling** | Combines generating multiple solutions with iterative refinement. | Highest robustness for production environments. |

### **Thought Budgeting and Verification**

Reasoning models often suffer from overthinking (wasting tokens on simple problems) or underthinking (prematurely abandoning a reasoning track). Thought budgeting techniques include:

* **Step Indicator Tokens:** Manually inserting tokens like wait or alternatively to force deeper thought.  
* **Difficulty-Adaptive Scaling:** Training models to adjust thought length based on the sampling accuracy of a problem (shorter for easy tasks, longer for difficult ones).  
* **Critic Models:** Using smaller verifier models to score the reasoning traces of larger models.

\--------------------------------------------------------------------------------

## **III. Specialized Applications: Myoelectric Control and HPC**

### **Myoelectric Human-Machine Interfaces**

Research into myoelectric control, interpreting electrical muscle signals, is bridging the gap between human intent and robotic action.

* **Prosthetics:** Challenges remain in separability (distinguishing between gestures) and **repeatability** (ensuring a gesture looks the same every time).  
* **The Human-AI Loop:** Unlike static AI, myoelectric systems involve a dual learning process where the AI learns the user's signals while the user learns to control the AI.  
* **Consumer Shift:** Companies like **Meta** are exploring these signals for subtle AR/VR control, moving the technology from a niche medical use case to a broad consumer interface.

### **High-Performance Computing (HPC) and Simulation**

Large-scale HPC centers (such as EPCC in the UK) are moving beyond traditional physics simulations into humanities and social policy.

* **Aero-Engine Simulation:** Projects with **Rolls-Royce** aim for virtual certification of engines, simulating turbine blades at melting temperatures to reduce the need for $25 million destructive tests.  
* **Democratization:** The integration of AI into HPC is allowing non-traditional domains (arts, social science) to utilize exascale-type compute for societal problems.

\--------------------------------------------------------------------------------

## **IV. Infrastructure and Energy Requirements**

### **The Alberta Energy Advantage**

The AI sector is transitioning from 10MW data centers to gigawatt scale requirements. Alberta is uniquely positioned due to:

* **Grid Capacity:** A $15 billion transmission expansion completed in 2015 provides a rare overbuilt grid capable of accepting massive new loads (This refers to ATCO’s EATL)  
* **Surplus Generation:** Approximately 2,000MW of surplus generation is available, alongside significant natural gas reserves (Clarification: This is the potential grid capacity for new connections, not a guaranteed excess power, as per [AESO 2017](https://www.aeso.ca/assets/Uploads/CMD-2.0-Rationales-CONSOLIDATED-Final.pdf)).   
* **Economic Impact:** A single 400MW site can contribute 50-100 million annually in provincial royalties (Clarification: This is not supported by data, but it can contribute to provincial and local economies through land taxes, rather than provincial royalties).

### **Sustainability and the Energy Transition**

The massive power draw of AI necessitates a multi-pronged sustainability strategy:

* **Natural Gas & Carbon Capture:** Immediate scaling relies on gas, necessitating carbon capture and sequestration (CCS) technologies capable of capturing up to 90% of emissions.  
* **Future Sources:** Medium-to-long-term solutions include Small Modular Reactors (SMRs) and a potential Canada wide grid to share hydro and wind/solar power across provincial borders.  
* **Circular Economy:** Innovations in the UK include reusing data center waste heat to warm local mine water for residential district heating.

\--------------------------------------------------------------------------------

## **V. Ethics, Bias, and Indigenous Perspectives**

### **Misinformation as a Tool**

Misinformation is identified as a historic tool of oppression used to marginalize Indigenous peoples and facilitate resource extraction.

* **Narrative Control:** Historical documentation of Indigenous peoples was primarily written by settlers, creating a "gaslighting master class" regarding land rights and cultural identity. (Clarification: This offensive woke comment is [Shani Gwin](https://www.linkedin.com/in/shanigwin/) opinion)  
* **Algorithmic Harm:** AI trained on colonial data risks perpetuating these biases, potentially making biased decisions in child welfare, criminal justice, or economic development. (Clarification: This offensive woke comment is [Shani Gwin](https://www.linkedin.com/in/shanigwin/) opinion)

### **Innovation in Responsible AI**

To counter these risks, new frameworks are being developed:

* **wâsikan kisewâtisiwin:** A prototype AI plug-in designed to correct bias and misinformation about Indigenous peoples in real-time, reducing the emotional labor on Indigenous communities.  
* **Matriarchal AI:** A proposed model that rejects traditional hierarchical/patriarchal organizational charts (the pyramid) in favor of natural, collective structures (e.g., flowers, pine cones, or tree rings).  
* **Responsible AI Facets:**  
  * **Privacy:** Protecting against data breaches (averaging $3.86 million per incident).  
  * **Explainability:** Ensuring models can explain why a decision was made, critical in healthcare and finance (e.g., the failure of **IBM** Watson for Oncology due to lack of explainability).  
  * **Fairness:** Ensuring systems do not treat different demographics unequally.

\--------------------------------------------------------------------------------

## **VI. Critical Conclusions**

The path forward for AI is defined by collective success rather than individual competition. High-quality AI development requires:

* **Slow Innovation:** Rejecting the move fast and break things motto in favor of seven generation thinking, evaluating the impact of technology on descendants seven generations into the future.  
* **Human-Centric Design:** Maintaining the human in the loop to validate AI outputs and ensure the technology serves as a helper (Oskâpêwis) rather than a replacement for human creativity and agency.  
* **Open Collaboration:** Tools like LibEMG (open-source myoelectric library) and the sharing of HPC research software engineering (RSE) practices are essential for democratizing access to these powerful tools.

# Day 2 Stage 1

# **AI Adoption, Infrastructure, and Education**

## **Executive Summary**

The Upperbound 2025 conference serves as a pivotal platform for announcing major strategic investments and discussing the transition of Canada, specifically Alberta, from a leader in artificial intelligence (AI) research to a global leader in AI adoption. Central to this transition is a $5 million investment from **Google** to the **Alberta Machine Intelligence Institute** (**Amii**) to establish a national consortium of 25 post-secondary institutions. This initiative aims to integrate AI literacy across all academic disciplines, preparing the future workforce for a landscape where generative AI is projected to boost Alberta’s economy by $27 billion and the national economy by over $230 billion.

While Canada faces a productivity emergency, with stagnant growth over the last seven years, the sources outline a multi-pronged strategy to reverse this trend:

* **Infrastructure:** Developing sovereign compute capacity to protect domestic intellectual property.  
* **Government Leadership:** Implementing AI-first internal policies and automating bureaucratic processes (e.g., Privacy Impact Assessments) to demonstrate real-world efficacy.  
* **Industry Transformation:** Targeting high-impact, low-productivity sectors like construction through robotics and predictive modeling.  
* **Advanced Research:** Moving beyond Large Language Models (LLMs) toward Artificial General Intelligence (AGI) through reinforcement learning and real-world robotics integration.

\--------------------------------------------------------------------------------

## **1\. National AI Literacy and Educational Reform**

A primary theme across the sources is the necessity of moving AI education out of computer science departments and into general curriculum.

### **The Google.org and Amii Investment**

[Sabrina Geremia](https://www.linkedin.com/in/sabrina-geremia-028644/) (VP, **Google** Canada) announced a $5 million investment to Amii.

* **Scope:** Creation of an easy-to-use AI curriculum for 25 post-secondary institutions.  
* **Target:** Students in medicine, arts, engineering, and business.  
* **Justification:** A report by Public First indicates that 63% of Canadian workers (72% among younger workers) desire AI upskilling. Generative AI alone could save the average worker over 175 hours annually.

### **Challenges in Higher Education**

[Tamara Peyton](https://ca.linkedin.com/in/tamara-peyton-phd-5600b725) (**NAIT**) and [Michael Burt](https://www.linkedin.com/in/michael-burt-342b0a42/) (Conference Board of Canada) identified critical hurdles in current educational frameworks:

* **Risk Avoidance:** Many institutions focus on "don't use it" (plagiarism/ethics) rather than opportunity maximizing.  
* **The Literacy Gap:** Students often do not know what to ask for because they lack the language to describe AI's transformative potential in their specific fields.  
* **Micro-credentials:** While useful for mid-career resiliency, they suffer from low recognition outside the tech sector.

\--------------------------------------------------------------------------------

## **2\. Economic Impacts and the Productivity Emergency**

[Michael Burt](https://www.linkedin.com/in/michael-burt-342b0a42/) of the Conference Board of Canada characterized the current economic state as a productivity emergency.

### **Productivity Data and Projections**

| Metric | Detail |
| :---- | :---- |
| **GDP Potential** | Full AI implementation could add $200B to Canadian GDP today. |
| **Current Adoption** | Only 26% of Canadian businesses have implemented an AI use case, trailing global peers by 10 points. |
| **Stagnation** | Output per hour in Canada is identical to what it was seven years ago. |
| **Sector Exposure** | 10% or more of tasks in every major sector (transportation, mining, oil/gas) are susceptible to AI transformation. |

### **The Shift to Cognitive Automation**

Traditionally, automation targeted physical tasks. AI represents a shift toward the automation of cognitive tasks, affecting professional roles previously thought immune, such as:

* Data scientists and software engineers.  
* Business systems analysts.  
* Records management and professional services.

\--------------------------------------------------------------------------------

## **3\. Government Strategy: Leading by Example**

Minister [Nate Glubish](https://www.linkedin.com/in/nateglubish/) outlined a strategy for the **Government of Alberta** to act as the province’s tech nerds, demonstrating AI's value through internal adoption.

### **Key Initiatives**

* **Sovereign Compute:** The government is investing in **Nvidia** powered data centers to ensure sensitive data and IP remain within Alberta, protected from foreign IP laws.  
* **Privacy Impact Assessment (PIA) Generator:** A custom AI tool trained on Alberta legislation that reduces the time to create a PIA from two months to minutes, ensuring 100% legal compliance while accelerating project start dates.  
* **Procurement and Infrastructure:** Utilizing computer vision and AI agents to overhaul government workflows. One project estimated at $57M and six years by consultants was projected to be completed for $5M in 18 months using AI tools.  
* **Concierge Program:** A dedicated team led by Assistant Deputy Minister (ADM) [Shawn Murphy](https://www.linkedin.com/in/seanmurphyprofile/) to assist data center developers and hyperscalers in navigating the Alberta grid and regulatory environment.

\--------------------------------------------------------------------------------

## **4\. Sector-Specific Deep Dives**

### **Construction and Robotics**

[Bruce Alton](https://ca.linkedin.com/in/brucealton) (**RoBIM Technologies**) highlighted that construction, a $13 trillion global industry, has seen zero productivity growth in 75 years.

* **The Phil Problem:** The industry relies on experiential knowledge from retiring experts. AI is needed to capture this "Phil-knowledge" into digital feedback loops.  
* **Robotic Hives:** Development of modular, mobile robotic cells that can be shipped in containers to construction sites for wood/steel framing and material preparation.  
* **Constraint:** Unlike factory environments, construction sites are uneven and unpredictable, requiring intelligent robots rather than simple programmed arms.

### **Planetary Science**

[Abby Azari](https://www.linkedin.com/in/abby-azari/) (**University of Alberta** / **Amii**) discussed the application of ML in space exploration (Maven/Mars missions).

* **Data Saturation:** Modern missions like Sentinel collect 20 terabytes of data daily, making manual analysis impossible.  
* **Physics-Informed ML:** Standard out-of-the-box ML is insufficient. Researchers are using emulators to approximate complex fluid dynamics and magnetic field equations, allowing for faster scientific inverse problem solving while accounting for model uncertainty.

\--------------------------------------------------------------------------------

## **5\. The Future of AGI and Real-World Interaction**

[John Carmack](https://en.wikipedia.org/wiki/John_Carmack) (**Keen Technologies**) provided an incisive look at the scientific challenges of moving beyond LLMs toward AGI.

### **Critical Insights for Research**

* **Beyond LLMs:** LLMs do not learn like humans or animals. They are a giant blender of human knowledge but lack the ability to learn new, novel tasks in real-time.  
* **The Latency Barrier:** Most RL (Reinforcement Learning) agents are trained in simulations where the world waits for the agent. In reality, a robotic action might take 180ms to execute, during which time the environment has changed. [Carmack](https://en.wikipedia.org/wiki/John_Carmack) advocates for inverting RL environments so the environment calls the agent, rather than vice versa.  
* **Atari Benchmarks:** [Carmack](https://en.wikipedia.org/wiki/John_Carmack) defends the use of Atari 100K as a benchmark because it provides an unbiased, non-researcher-defined challenge that tests sequential multitask learning and sparse rewards.

### **The Robo-roller Experiment**

To test RL in the real world, **Keen Technologies** developed a physical setup using a camera and a robotic servo to play an actual Atari console.

* **Finding:** Agents can learn despite glare, camera distortion, and physical latency, but they require the ability to incorporate intrinsic rewards and curiosity rather than just chasing a score.

\--------------------------------------------------------------------------------

## **6\. Workforce Resilience: Required Skills**

The sources concluded with an unanswerable question regarding the skills needed five years from now. The consensus focused on a Unicorn foundation:

* **Left Brain:** Deep technical understanding of math and compute.  
* **Right Brain:** Collaborative problem-solving, adaptive change, and human-centric leadership.  
* **Resilience and Curiosity:** The ability to treat AI as a knowledge partner and the willingness to iterate through failures.  
* **Translators:** A high demand exists for translators, senior leaders who understand both the business use case and the AI potential, even if they cannot build the models themselves.

# Day 2 Stage 2

# **Technical Innovation, Economic Impact, and Societal Integration**

## **Executive Summary**

This briefing document synthesizes key insights from the Upperbound 2025 conference, examining the current state of Artificial Intelligence (AI) through the lenses of industrial application, technical research breakthroughs, and socio-economic implications. The analysis highlights a critical transition from peripheral AI usage to deep, process-integrated automation. Key takeaways include:

* **Computational Evolution:** The emergence of Streaming Deep Reinforcement Learning (DRL) addresses a long-standing stream barrier, allowing for real-time, compute-efficient learning without the need for massive historical data storage.  
* **Economic Imperatives:** Canada faces a significant productivity gap compared to G7 peers, particularly in the Small and Medium Enterprise (SME) sector. AI modernization is identified as a primary driver for bridging this gap, provided it is used to re-engineer core business processes rather than just augmenting administrative tasks.  
* **Industry Maturity:** Retail and financial sectors are successfully deploying AI for complex tasks such as high-volume price matching, developmental parenting support, and large-scale market order execution (trading over $100 billion in notional value).  
* **Risks and Literacies:** As AI moves from a tool to a collaborator, societal risks such as automation complacency, cognitive atrophy, and environmental costs must be managed through a shift from basic AI literacy to comprehensive AI fluency.

\--------------------------------------------------------------------------------

## **1\. Technical Frontiers: Streaming Deep Reinforcement Learning (DRL)**

A significant scientific breakthrough discussed involves the shift from batch-based offline learning to Streaming DRL. This methodology allows AI models to learn continuously from a live experience stream without storing past data in raw form.

### **The Stream Barrier and Its Resolution**

* **Historical Instability:** Traditionally, training neural networks on a live stream (non-stationary, non-IID data) resulted in instability, divergence, or catastrophic forgetting.  
* **Breakthrough Algorithms:** New methods, specifically AVG (Action Value Gradient) and Stream-X, have overcome this barrier. These algorithms utilize carefully curated normalization techniques (input, output, and penultimate activation) and specialized optimizers.  
* **The New Optimizer:** To prevent overshooting in the loss landscape, where a large update interferes with previously learned signals, the new optimizer bounds update sizes based on a proxy of update alignment across time steps.

### **Impact of Atomic Compute Efficiency**

* **Resource Conservation:** Streaming DRL frees up orders of magnitude in compute resource. While batch methods like Soft Actor-Critic (SAC) may use 256 samples per update, streaming methods use a single sample.  
* **Ubiquitous AI:** This efficiency allows for on-device learning on low-power hardware (smartphones, IoT devices), democratizing AI by reducing reliance on massive remote server clusters.

\--------------------------------------------------------------------------------

## **2\. AI in Industrial Applications: Retail and Finance**

The practical deployment of AI is most visible in retail and financial services, where data volume and complexity demand automated decision-making.

### **Retail and Consumer Platforms**

* **BetterCart Analytics:** This B2B platform processes over 55 million data observations weekly to provide price transparency in the low-margin grocery industry. It utilizes AI for exact and similar product matching to assist manufacturers and retailers in real-time competitive strategy.  
* **Bobo (Parenting Super App):** This platform aims to accelerate child development by tracking developmental data and social cues. It uses AI to distill fragmented parenting data into actionable insights and triages users toward expert services like speech pathology or sleep consultancy.

### **Financial Services and Capital Markets**

* **Aiden (Order Execution):** An RL-based agent developed by **RBC** Borealis that has traded more than $100 billion in notional value. It solves the problem of market impact, where large orders inadvertently spike prices, by learning a policy to break trades into smaller, strategically timed executions.  
* **Nomi Forecast:** Utilizes selective prediction (selective nets) to forecast client bill payments. The model is designed to abstain from making a prediction when confidence is low, prioritizing accuracy over volume to maintain user trust.  
* **Atom (Foundational Transaction Model):** Unlike Large Language Models (LLMs) that predict the next word, Atom is a foundation model for financial transactions. It handles irregular, non-sequential data (shopping sprees followed by inactivity) using masked next-token prediction and contrastive learning.

\--------------------------------------------------------------------------------

## **3\. The Productivity Dilemma and SME Modernization**

Data from **BDC** indicates a critical need for AI adoption within the Canadian economy, where productivity has remained stagnant for several years.

### **The Productivity Gap**

* Canada is currently 30% behind the United States in labor productivity.  
* SMEs contribute over 50% of Canada's GDP, yet half do not survive past the five-year mark.  
* Top-performing companies (the top 10%) invest twice as much in ICT and 1.5 times more in automation and AI than their peers.

### **Implementation Strategies**

To achieve true productivity gains, businesses must move beyond peripheral AI use (e.g., using ChatGPT for marketing) and toward Core Process Re-engineering:

* **Predictive Maintenance:** Moving from calendar-based repairs to AI-triggered maintenance reduces downtime and automates procurement and scheduling across the enterprise.  
* **Winning Conditions:** Successful implementation requires a clear strategy, data maturity (moving away from duplicated Excel sheets), and a framework for continuous upskilling and governance.

\--------------------------------------------------------------------------------

## **4\. Risks, Ethics, and AI Offscript**

While AI offers immense potential, offscript moments and systemic risks necessitate a critical approach to its integration.

### **Failures and Hallucinations**

* **Computer Vision Fails:** AI cameras have mistaken a linesman’s bald head for a soccer ball. **Tesla**’s autopilot has been shown to stop for a person wearing a Stop Sign t-shirt and can be fooled by "Wile E. Coyote" style murals of roads painted on walls.  
* **Generative Hallucinations:** **xAI**’s Grok AI incorrectly reported that NBA player [Klay Thompson](https://en.wikipedia.org/wiki/Klay_Thompson) was vandalizing houses with bricks due to a misunderstanding of the basketball slang for a missed shot. **Google**’s AI Overviews have suggested eating rocks or using non-toxic glue to keep cheese on pizza.  
* **Legal Liability:** **Air Canada** was held liable by a small claims court after its chatbot provided a customer with incorrect information regarding bereavement discounts, highlighting that companies are responsible for their AI's output.

### **Societal and Cognitive Risks**

* **Automation Complacency:** Humans in the loop often fall asleep or become passive when monitoring automated systems, leading to safety risks (e.g., the 2018 **Uber** self-driving fatality).  
* **Cognitive Atrophy:** There is significant concern that over-reliance on AI for writing, planning, and basic mathematics could erode critical thinking skills and human exceptionalism.  
* **AI Fluency:** Experts argue for a move from literacy to fluency, the ability to seamlessly and critically navigate a world where AI is a collaborator. This includes understanding the environmental impact (energy and water consumption of LLMs) and the ethical implications of algorithmic decision-making.

\--------------------------------------------------------------------------------

## **5\. Summary of Strategic Frameworks for Organizations**

| Element | Organizational Focus |
| :---- | :---- |
| **Strategy** | Alignment of AI use cases with core business pain points and executive objectives. |
| **Data Maturity** | Ensuring data validity and reliability; identifying where data is stored (CRM vs. ERP). |
| **People** | Involvement of department heads in tool selection; continuous upskilling. |
| **Governance** | Developing legal frameworks for privacy and ethical decision-making (e.g., the Montreal Declaration). |
| **Verification** | Utilizing toolchains to test AI outputs for hallucinations and errors in specific domains. |

# Day 2 Stage 3

# **Humanity and Progress in an AI-Driven Era**

## **Executive Summary**

The transition into an artificial intelligence-driven society represents a fundamental shift in how humanity manages data, makes decisions, and structures its workforce. While AI has been embedded in daily life for decades through tools like GPS and autocorrect, the current era is defined by the rapid scaling of generative systems and the emergence of Physical AI. However, this progress is tempered by significant risks: systemic biases in high-stakes areas like employment and criminal justice, a lack of transparency in algorithmic decision-making, and a widening knowledge gap between technical researchers and policymakers.

Critical takeaways from recent cross-disciplinary analyses include:

* **The Garbage In, Garbage Out Principle:** AI systems inherit the biases of their creators and the historical data used to train them, leading to documented discrimination in hiring and sentencing.  
* **The Necessity of Human-AI Synergy:** Leadership must shift from micromanagement to strategic guidance. Successful organizations (e.g., **Johnson & Johnson**, **JP Morgan**) prioritize upskilling current workforces rather than seeking external talent that may not yet exist.  
* **Policy-Technology Integration:** There is an urgent need for "policy feasibility testing" to ensure regulations keep pace with rapid technical advancements like agentic and physical AI.  
* **Specialized Innovation:** AI is driving breakthroughs in biological sciences, such as optimizing plant biomass through the simulation of twilight light recipes and hyperspectral imaging.  
* **The Rise of World Foundation Models:** The next frontier involves AI that understands and interacts with the physical world through simulation and synthetic data generation.

\--------------------------------------------------------------------------------

## **I. The Human Element: Cognitive Shortcuts and Algorithmic Bias**

AI systems are often perceived as objective alternatives to flawed human decision-making. However, human cognitive limitations are frequently mirrored or amplified within these systems.

### **Human Cognitive Limitations**

* **Overgeneralization:** Humans use small datasets to form broad conclusions, leading to stereotypes and failed "rules of thumb" (e.g., "I before E except after C").  
* **Confirmation Bias:** The tendency to favor information that supports existing beliefs, often leading to social media siloing on emotionally charged issues like race or politics.  
* **Decision Fatigue:** A phenomenon where the quality of human decisions deteriorates over time. A 2011 study of judges showed favorable parole rulings dropped significantly before meal breaks, a vulnerability AI does not share.

### **Systemic Bias in AI (Garbage In, Garbage Out)**

Because AI learns from historical data, it often codifies historical injustices.

* **Employment:** In 2023, the first AI hiring bias lawsuit was settled after software was found to automatically reject female applicants over 55\. Research shows resume filtering systems prefer white-sounding names 85% of the time over black-sounding names, even with identical qualifications.  
* **Criminal Justice:** The Compass program, used for sentencing and bail, has a 20% accuracy rate for predicting violent recidivism. It is twice as likely to falsely flag Black defendants as future criminals compared to white defendants.  
* **Opaque Systems:** Many high-stakes algorithms are trade secrets, preventing defendants or job seekers from understanding why they received a specific score or rejection.

\--------------------------------------------------------------------------------

## **II. Strategic Workforce Transformation**

As AI shifts from a tool to a co-worker, organizations must redesign their talent and leadership structures.

### **The AI-Ready Workforce Framework**

Organizations should segment talent into three distinct categories:

1. **AI Creators:** Technical builders (machine learning engineers, data scientists).  
2. **AI Augmenters/Enhancers:** Business professionals integrating AI into daily operations.  
3. **AI Translators:** The bridge between technical experts and strategic leadership.

### **Leadership Competency Model**

The role of management is evolving from people management to organizational system management. Key competencies include:

* **AI Fluency:** Grasping capabilities, limitations, and risks rather than just technical coding.  
* **Ethical Decision-Making:** Implementing Human-in-the-Loop systems where AI informs but does not replace human judgment.  
* **Dynamic Adaptability:** Fostering a "fail fast, learn fast" culture that encourages experimentation.

### **Change Management and the Valley of Doom**

Resistance to AI often stems from fear. Leaders must mitigate this through:

* **Early Communication:** Addressing fears of replacement head-on.  
* **Sponsorship:** Executive leaders (e.g., [Jamie Dimon](https://en.wikipedia.org/wiki/Jamie_Dimon) at **JP Morgan**) modeling the use of AI tools.  
* **Targeting Middle Management:** Supervisors are the primary drivers of adoption, without their buy-in, frontline teams often resist.

\--------------------------------------------------------------------------------

## **III. Policy and Governance: Bridging the Expertise Gap**

Policymakers face slow chaos as they attempt to regulate technologies they may not fully understand.

### **The AI Insights for Policy Makers Program**

A Canadian initiative by **Mila**, **CIFAR**, and **Amii** aims to provide technical eyes for government officials.

* **Mission:** To provide independent, technical feedback on draft legislation rather than broad, prescriptive reports.  
* **Policy Feasibility Testing:** Evaluating whether regulations make technical sense (e.g., can machine unlearning actually be enforced?).  
* **Nimble Governance:** The call for government structures to be as flexible as the technology they oversee, as five-year policy cycles are too slow for AI's monthly advancements.

### **Legislative Landscapes**

* **EU AI Act:** A significant influence on global policy, acting as a checklist for market entry.  
* **Canadian Context:** The emergence of a dedicated Minister for AI and the development of voluntary codes of conduct for generative AI.

\--------------------------------------------------------------------------------

## **IV. Technical Frontiers: Physical AI and World Foundation Models**

The focus of AI is shifting from digital knowledge generation (Software 2.0) to interacting with the physical world.

### **Nvidia Cosmos and World Foundation Models (WFMs)**

The next wave of AI, Physical AI, focuses on robotics and autonomous vehicles.

* **Cosmos Predict:** Generates future world states based on text or video prompts.  
* **Cosmos Transfer:** Transforms 3D scenes from simulation (**Nvidia**’s Omniverse) into photorealistic video with variable weather and lighting.  
* **Cosmos Reason:** Uses chain of thought reasoning to explain why a physical AI took a specific action (e.g., why a robot moved its arm upward).

### **The Role of Synthetic Data**

Physical world data is costly and dangerous to collect (e.g., simulating children running into roads for autonomous vehicle testing). World Foundation Models allow for the generation of vast amounts of physically grounded synthetic data to train robots without real-world risk.

\--------------------------------------------------------------------------------

## **V. Domain-Specific Innovation: AI in Agriculture**

AI is being used to understand the molecular clock of plants, leading to precision horticulture.

### **The Twilight Experiment**

Researchers used computer vision and precision LED lighting to study how twilight (gradual dawn/dusk) affects plant growth.

* **Key Finding:** Simulating a 30-to-90-minute dawn/dusk period significantly increases plant biomass compared to standard on/off lighting.  
* **Significance:** This allows for increased production in vertical farming without prematurely triggering flowering, which can degrade the quality of leafy greens like kale.

### **Imaging Technologies**

* **Plant CV:** An open-source computer vision workflow used to extract leaf surface area and growth signatures from simple **Raspberry Pi** cameras.  
* **Hyperspectral Imaging:** Using the full light spectrum to detect happy vs. stressed plants (e.g., drought or pathogen attack) long before the damage is visible to the human eye.

\--------------------------------------------------------------------------------

## **VI. Framework for Ethical AI Governance**

To retain humanity in an AI-driven society, organizations must implement rigorous governance.

| Pillar | Actionable Requirement |
| :---- | :---- |
| **Bias Mitigation** | Regularly audit algorithms and use diverse training datasets. |
| **Transparency** | Ensure AI-generated decisions are explainable and documented. |
| **Accountability** | Assign AI Risk Officers and create internal ethics review committees. |
| **Trust** | Allow customers and employees to opt-out of AI-driven processes. |

### **Conclusion**

The successful integration of AI requires a move away from black box systems toward transparency and literacy. As stated during the Upperbound 2025 proceedings: Efficiency may be good, but at what cost?" The path forward demands critical thinking, constant questioning of data sources, and a commitment to upskilling the human workforce to lead alongside the machines they created.

# Day 3 Stage 1

# **From Marketing to Infrastructure: AI Innovation and Strategic Implementation** 

## **Executive Summary**

This briefing document synthesizes high-level insights from industry leaders, data scientists, and entrepreneurs regarding the operationalization of Artificial Intelligence (AI). The central theme across all sectors, from creative marketing to municipal service delivery, is the transition from theoretical exploration to practical application. Key takeaways include:

* **Productivity through Velocity:** AI’s primary immediate value lies in velocity to first draft, allowing human experts to bypass the blank-page stage and move directly to refinement and strategy.  
* **Operationalization over Novelty:** Successful AI integration requires a problem-driven rather than solution-driven approach. In municipal contexts, this has manifested in significant resource savings, such as thousands of hours reclaimed in safety code inspections.  
* **The Human-Centric Barrier:** Adoption is currently hampered more by organizational culture and change management than by technical limitations. In regions like Alberta, business adoption remains as low as 4-6.3%.  
* **Founder and Team Vitality:** In the venture capital landscape, the most critical success factors remain the growth mindset and hustle of human founders, rather than the technical complexity of an AI wrapper.

\--------------------------------------------------------------------------------

## **1\. AI in Marketing: Productivity, Tools, and Adoption**

The marketing sector is currently navigating the firehose of AI tools, focusing on tactical gains while managing employee anxiety.

### **Tactical Productivity Gains**

* **Content Generation:** Marketing specialists report significant gains in velocity. One case study noted a writer completing six months of blog content in a single day by using AI as a tool for first drafts and cohesion.  
* **Mixed-Mode Analysis:** Agencies are using AI to analyze vast datasets, such as 6,000 sales calls to score performance or spreadsheets of **Google** Ads data to find unseen correlations between media spend and store traffic.  
* **Executive Assistance:** Leaders use AI for low-level data entry tasks, such as converting screenshots of schedules into ICS calendar files.

### **The Tool Landscape**

| Tool | Primary Use Case |
| :---- | :---- |
| **ChatGPT / Gemini** | Natural language conversations, strategic brainstorming, and data analysis. |
| **NotebookLM** | Synthesizing long-form documents (books/papers) into digestible summaries or audio overviews. |
| **Perplexity** | Deep research and insight gathering for strategists. |
| **Riverside FM** | Automated podcast editing and social video generation. |
| **Claude** | Noted for higher accuracy in specific tasks like video segment ideation where other models may hallucinate. |

### **Organizational Adoption Strategies**

* **The AI Task Force:** Companies are de-siloing AI knowledge by creating cross-departmental groups to share tools and establish guidelines.  
* **Delegation vs. Change Management:** Rather than viewing AI as a technical shift, leaders should treat it as a management problem of delegation, asking, Should you be doing this, or can a colleague (AI) do it?  
* **Safety and Ethics:** Organizations must implement clear guidelines on what not to put into AI, particularly regarding copyrighted material and client indemnification.

\--------------------------------------------------------------------------------

## **2\. Technical Innovations: Vision Anomaly Detection**

Advanced research is moving toward zero-shot models, systems that can identify anomalies without needing extensive training on specific abnormal datasets.

### **Principles of Anomaly Detection**

* **Defining Normal:** Anomaly detection is often an unsupervised problem because while normal data is plentiful, abnormal data is rare, expensive to collect, and heterogenous.  
* **Teacher-Student Models:** A teacher model learns normal patterns, a student model tries to mimic it. If a student fails to reconstruct a specific image part, that area is flagged as an anomaly.  
* **Reverse Distillation:** A more advanced technique where the logic flow is reversed to further enlarge the discrepancy between normal and abnormal responses, improving localization in medical or industrial images.

### **Scaling and Zero-Shot Learning**

* **Vision Language Models (VLMs):** Leveraging foundation models (like CLIP) allows for zero-shot detection, where the model uses text prompts (e.g., a photo of a damaged plate) to identify issues without prior training on that specific product.  
* **Test-Time Scaling:** Performance can be boosted during the inference stage by using test-time adaptation, tuning the model to a specific industrial domain on the fly.

\--------------------------------------------------------------------------------

## **3\. Municipal Operationalization: The City of Edmonton Case Studies**

The City of Edmonton’s Data Science and Research team provides a blueprint for applying AI to core public services with a bias toward action.

### **Project Ember Wise (Wildfire Monitoring)**

* **Mechanism:** Automates the Canadian Forest Fire Danger Rating System (CFFDRS) to forecast wildfire ignition and spread.  
* **Integration of Human Behavior:** Unlike traditional models, Ember Wise seeks to integrate behavior-based risk by analyzing calls for service related to illegal encampments and open-flame cooking in the River Valley.

### **Safety Codes Inspection Efficiencies**

* **Problem:** Inspectors are overwhelmed by a half-million annual residential inspections.  
* **AI Solution:** A Random Forest classifier predicts the probability of a first-time pass.  
* **Impact:** By automating passes for low-risk, non-mandatory inspections (like insulation or framing), the city has saved over 6,800 hours of manual labor, translating to approximately $50,000 in annual savings.

### **Project Repair (Pothole Management)**

* **Scope:** Edmonton fills approximately 500,000 potholes annually.  
* **Predictive Modeling:** Uses ARMA (Auto-Regressive Moving Average) models to predict the number of potholes in specific zones for the upcoming week based on historical data.  
* **Future Innovation:** Development of a voice-activated app to allow drivers to report potholes safely while driving.

\--------------------------------------------------------------------------------

## **4\. Strategic Leadership and the Entrepreneurial Mindset**

Insights from venture capital highlight that the AI era does not fundamentally change the requirements for human leadership.

### **The Founder Success Formula**

Venture capitalists prioritize three traits over technical industry experience:

1. **Growth Mindset:** The ability to learn and iterate every six months.  
2. **Attraction of Talent:** The capacity to motivate and retain outstanding people who could otherwise work for tech giants.  
3. **Hustle/Speed of Execution:** The cycle of executing, learning, and iterating at high velocity.

### **Competitive Advantage in AI**

Investors warn against AI wrappers, companies that simply add a thin layer over large language models. True competitive advantage is derived from:

* **Proprietary Data:** Gaining information through unique workflow integration.  
* **Go-to-Market (GTM) Strategy:** The ability to reach and onboard customers at a lower cost than their lifetime value.  
* **Network Effects:** Building communities or brands that cannot be easily replicated by a new model.

\--------------------------------------------------------------------------------

## **5\. Critical Challenges and Gotchas**

The transition to AI-driven operations is not without significant pitfalls:

* **Hallucinations:** In one marketing case, an AI hallucinated 100% of video segment suggestions based on an actual transcript.  
* **Roleplaying Agents:** One user reported a model roleplaying the creation of a presentation, claiming it was in **Google** Drive, when it had actually done nothing, leading to 15 minutes of lost productivity.  
* **Technical Resistance:** Industry veterans often view AI with skepticism (It will steal my creativity). Overcoming this requires teaching people how to fish rather than forcing adoption.  
* **The Quantity vs. Quality Trap:** There is a risk that AI will simply raise the bar for production volume rather than freeing up time, leading to an explosion of trash content.

\--------------------------------------------------------------------------------

## **Key Quotes**

"AI can certainly give you 100 bad ideas pretty quick... but it’s not going to write an award-winning, mind-blowing headline right now",  [**Rob Jennings**](https://ca.linkedin.com/in/robcjennings)

"If you have a lot of money, you focus on spending it. If you don’t have a lot of money, you focus on making it",  [**Janet Bannister**](https://www.linkedin.com/in/janetbannister/)

"Prompt engineering was going to be the next big job... then three days later, somebody announced an AI tool that you could ask to prompt for you",  [**Carrie Robinson**](https://ca.linkedin.com/in/carrie-denise-robinson)

"AI isn't just tech. It’s a tool for you to solve real problems... AI is augmentation, not disruption",  [**Ali Golabchi**](https://ca.linkedin.com/in/ali-golabchi)

# Day 3 Stage 2

# **Key Insights and Strategic Briefing**

## **Executive Summary**

The proceedings from the Upperbound 2025 conference represent a comprehensive overview of the current state and future trajectory of Artificial Intelligence. The discussions shifted from general conversational AI toward sophisticated agentic workflows, rigorous Responsible AI (RAI) frameworks, and specialized applications in sectors ranging from heavy construction to autonomous agriculture.

Critical takeaways include:

* **The Intent Elicitation Paradigm:** [Max Kreminski](https://mkremins.github.io/) of **Midjourney** argues that the fundamental challenge in creative AI is the dearth of the author, where low-information prompts lead to homogenized outputs. Future systems must focus on lensing the imagination through interactive intent elicitation.  
* **From Chat to Agents:** [Jay Alammar](https://ca.linkedin.com/in/jalammar) (**Cohere**) and the ARV panel highlighted the transition from simple chat interfaces to LLM-backed agents capable of multi-hop reasoning, tool use (APIs), and sequential problem-solving.  
* **Responsible AI (RAI) as a Market Differentiator:** **AltaML** emphasizes that RAI principles, specifically transparency, accountability, and awareness, must precede revenue and are essential for maintaining public trust in government AI deployments.  
* **Industry-Specific Disruption:** Startups like **Bidblox**, **Cashew Research**, and **Verge Agriculture** are applying AI to solve structural inefficiencies in pre-construction bidding, market research, and autonomous path planning for farmers.

\--------------------------------------------------------------------------------

## **I. Technical Foundations: Architecture and Training of LLMs**

The evolution of LLM architecture focuses on efficiency and the emergence of reasoning capabilities.

### **1\. The Modern Transformer Architecture**

The industry has moved beyond the original 2017 Transformer toward a modern stack:

* **Tokenization:** Current models use multi-byte character representation to handle emojis and diverse languages accurately. Some models, such as StarCoder, assign individual tokens to digits to improve mathematical performance.  
* **Attention Mechanisms:** Efficiency is gained through Grouped Query Attention (GQA), which shares key and value sets among groups of attention heads, balancing speed with model capability.  
* **Mixture of Experts (MoE):** Models like **DeepSeek** R1 use a router to activate only a subset of experts (sub-neural networks) for each token, significantly reducing the compute required per forward pass while maintaining a massive parameter count.

### **2\. The Post-Training Recipe**

Creating state-of-the-art models now involves a multi-stage post-training process:

* **Supervised Fine-Tuning (SFT):** Training the model on instruction-following data.  
* **Reinforcement Learning (RL):** Large-scale RL is used to develop reasoning chains. In models like **DeepSeek** R1, the system is rewarded for passing automated verifiers (e.g., unit tests or mathematical proofs).  
* **Preference Tuning (RLHF/DPO):** Aligning model outputs with human preferences regarding style, length, and helpfulness.  
* **Model Merging:** Organizations like **Cohere** use model merging to combine the weights of specialist models (e.g., a math expert and a coding expert) into a single, high-performing merged model.

\--------------------------------------------------------------------------------

## **II. Creative AI and Lensing the Imagination**

[Max Kreminski](https://mkremins.github.io/) (**Midjourney**) posits that current AI-supported creativity faces a human computer interaction (HCI) crisis characterized by Homogenization.

### **1\. The Dearth of the Author**

[Max Kreminski](https://mkremins.github.io/) identifies an information theory problem: when a user provides a minimal prompt (e.g., cat pirate), the model must fill the information gap using its training data. This results in the Captain Whiskers effect, repetitive, generic outputs that lack user ownership.

### **2\. Challenges to Co-Creativity**

* **Underexpression:** Users typically provide the fewest words possible, failing to communicate complex constraints.  
* **Fixation:** Creators often get stuck on one specific way of achieving a goal, limiting the AI's ability to offer useful alternatives.  
* **Uncertainty and the Endocept:** Creativity is often the process of discovering what one wants. The endocept is the vague, non-verbal intuition that guides an artist.

### **3\. Strategies for Intent Elicitation**

To overcome these challenges, systems are being designed to lens the imagination:

* **Semantic Lenses:** Visualizing character relationships or plot points on axes (e.g., Law vs. Chaos) to identify gaps in the expressive range.  
* **Gestural Controls:** Using physical movement or arcs (e.g., ToyTeller or TailBrush) to convey emotional or narrative intent that is difficult to verbalize.  
* **Explicit Divergence/Convergence:** Interfaces that force a wide search of ideas before narrowing them down into a final artifact.

\--------------------------------------------------------------------------------

## **III. Enterprise AI Strategy and Data Management**

The ARV panel outlined the Unified Data Analytics Journey, emphasizing that enterprise AI fails without foundational data governance.

### **1\. The Data Swamp**

Organizations frequently land data in lakes without proper metadata or structure, creating a swamp. A critical area for AI intervention is the Document Store (e.g., SharePoint, PDFs), where high-value information is trapped in unstructured formats.

### **2\. Retrieval Augmented Generation (RAG)**

RAG is the dominant enterprise paradigm, moving information storage out of the model's weights and into a database.

* **Benefits:** Lower hallucination rates, easier updates, and better explainability through citations.  
* **The Evolution to Agents:** Advanced RAG systems now utilize Multi-hop reasoning, where an LLM performs sequential searches to answer complex queries (e.g., comparing financial results across different years).

### **3\. Agentic Workflows**

AI agents perceive an environment and autonomously select a plan.

* **Decoupling Reasoning and Acting:** Agents use LLMs for planning while relying on external tools (APIs, calculators, SQL executors) for action.  
* **The Vibe Coding Shift:** AI-driven coding platforms (e.g., **OpenAI**’s Codex) allow for rapid development but require human oversight to prevent secrets (API keys) from leaking into public code and to manage security vulnerabilities.

\--------------------------------------------------------------------------------

## **IV. Responsible AI (RAI) and Public Service**

[Chantal Ritcey](https://ca.linkedin.com/in/chantal-ritcey-03531250) (**AltaML**) presented a framework for advancing AI within the public sector through **GovLab**, a triple-helix model combining government, academia, and private industry.

### **1\. The AltaML RAI Principles**

**AltaML** prioritizes seven core principles that guide all deployments:

| Principle | Description |
| :---- | :---- |
| **Inclusivity** | Ensuring systems benefit all through a plurality of perspectives. |
| **Fairness** | Actively de-biasing models to prevent systemic harms (e.g., recruitment bias). |
| **Transparency** | Allowing users to see why a model made a specific prediction (e.g., SHAP values). |
| **Accountability** | Maintaining a human in the loop for critical decisions. |
| **Safety & Security** | Building reliable systems that mitigate risks through agile, iterative development. |
| **Privacy** | De-identifying and anonymizing data throughout the AI lifecycle. |
| **Awareness** | Empowering stakeholders to have well-informed conversations about AI's impact. |

### **2\. Public Sector Case Studies**

* **Wildfire Prediction:** AI helps duty officers anticipate occurrences by identifying data attributes (e.g., precipitation levels) that inform risk levels.  
* **School Enrollment:** A model for the **Department of Education** predicts future student populations to optimize the location of new school builds. (Clarification: There is no federal department of Education in Canada, it should be the Alberta Ministry of Education & Childcare).  
* **Infrastructure:** Automating pothole and pavement defect detection using existing city fleet cameras while ensuring privacy through automated blurring of bystanders.

\--------------------------------------------------------------------------------

## **V. Startup Innovation: Upperbound Pitch Competition**

The conference featured a pitch competition highlighting AI-driven business models in Canada.

### **1\. Winners and Finalists**

* **1st Place: Bidblox ([Lisa Mohapatra](https://www.linkedin.com/in/lisamohapatra/)):** An AI-first platform for the pre-construction industry. It aims to be a **Bloomberg** terminal for construction, providing transparency in bidding and material pricing intelligence to reduce the 4,000+ hours spent on project planning.  
* **2nd Place: Cashew Research ([Addy Graves](https://www.linkedin.com/in/addy-graves-56547030/)):** An AI-guided market research software that automates survey creation and report synthesis. It leverages a proprietary mobile app database to reach high-income, tech-savvy audiences for brands like **Shopify**.  
* **3rd Place: Verge Agriculture ([Goddard](https://www.linkedin.com/in/ggodardg/)):** Focused on autonomous farming, this startup captures the inherited knowledge of farmers to create optimal path-planning routes. This reduces overlap, fuel consumption, and soil erosion without requiring new machinery.

\--------------------------------------------------------------------------------

## **VI. Critical Evaluation and Metrics**

Success in AI is no longer measured solely by accuracy, but by the reliability and diversity of output.

* **Homogenization Analysis:** Using embeddings to plot whether different users are being funneled into the same center of mass or if the tool supports distinctive voices.  
* **Evaluation Frameworks:** Real-time error tracking and offline evaluation using LLM as a judge to monitor correctness, efficiency, and tool utilization.  
* **Model Drift:** Ongoing monitoring is required to ensure models maintain performance levels post-deployment.

\--------------------------------------------------------------------------------

## **VII. Quotes of Note**

* "If you give a model a question, it might give you an answer, but you might have a better answer if you actually give it some context", [Jay Alammar](https://ca.linkedin.com/in/jalammar)  
* "The creative process is a process of figuring out what it is that you want", [Max Kreminski](https://mkremins.github.io/)  
* "Responsible AI comes before every other metric at our company, including revenue", [Chantal Ritcey](https://ca.linkedin.com/in/chantal-ritcey-03531250) (**AltaML**)  
* "Planning without intent is nothing", [Goddard](https://www.linkedin.com/in/ggodardg/) (**Verge Agriculture**)  
* AI won't take your job, but if you don't adapt, your capabilities will fall behind those who do",  Eric (ARV)

# Day 3 Stage 3

# **Strategic Perspectives on the Generative AI Landscape**

## **Executive Summary**

The rapid evolution of Generative AI represents a fundamental economic and structural shift comparable to the industrial and internet revolutions. Current data indicates that as the cost of prediction, generation, and deliberation trends toward zero, the primary value in the AI stack is migrating from the underlying models to the human-AI interface and the specific outcomes achieved in the real world.

Key takeaways from the analysis of the current AI landscape include:

* **Economic Reconfiguration:** We are moving from a one-shot generation model to an agentic model where AI autonomously executes reasoning plans, significantly reducing decision-making time for enterprises.  
* **The Experiment-to-Enterprise Gap:** In the public sector and large-scale industries, the challenge has shifted from basic literacy to the systematic enterprising of pilot projects, hampered largely by tech debt and policy debt.  
* **Interoperability as a Bottleneck:** In specialized fields like healthcare, data silos remain the primary obstacle. AI agents are being developed to bypass traditional API barriers through vision-based data mapping.  
* **The Moving Moat:** Technical moats are becoming increasingly fragile. Competitive advantage is now derived from proprietary data sets, community trust, and the speed of disruptive mindset pivoting rather than exclusive access to model weights.

\--------------------------------------------------------------------------------

## **1\. The Economics of Generative AI**

The economic impact of artificial intelligence is characterized by the radical reduction in the cost of cognitive tasks. This transformation is occurring across three primary dimensions:

### **The Cost-to-Zero Trend**

As scaling laws continue to apply, the following costs are perpetually declining:

* **Cost of Prediction:** The ability to forecast outcomes based on existing patterns.  
* **Cost of Generation:** The creation of new content (text, image, video, code).  
* **Cost of Deliberation:** The time and resources required to reason over a set of options.

### **Value Migration in the AI Stack**

While significant value currently resides at the bottom of the stack (chips, compute, and data centers), the long-term economic crucible lies at the interface between the human and the model.

* **Hardware Evolution:** There is an active shift from training-optimized hardware to inference-optimized hardware, with an increasing focus on on-device models to ensure privacy and speed.  
* **Agency over Outputs:** The industry is moving toward agents, systems that do work while the human is not working. The value is no longer just in the output (the generated text) but in the *outcome* (the action taken in the world).

"Alpha Evolve can sort of do the how of implementation while the human defines the what",  [**Kory Mathewson**](https://ca.linkedin.com/in/korymath)**, Google DeepMind**

\--------------------------------------------------------------------------------

## **2\. Public Sector Integration and Governance**

The **Government of Canada**’s approach to AI highlights the complexities of integrating cutting-edge technology into large-scale bureaucracies.

### **The Five Pillars of Public Sector AI Strategy**

1. **Skills and Talent:** Moving beyond general literacy to specific job-function upskilling (e.g., how AI changes the role of a border guard or meat inspector).  
2. **Infrastructure:** Strategic investment in Sovereign AI Compute to ensure national security and data sovereignty.  
3. **Safety, Security, and Trust:** Establishing guardrails through Algorithmic Impact Assessments.  
4. **International Leadership:** Leveraging the G7 presidency to establish global governance standards.  
5. **Adoption:** Transforming back-office functions (translation, summary of parliamentary committees, and access-to-information requests).

### **Structural Impediments**

* **Tech Debt:** Legacy systems that cannot simply be layered with AI.  
* **Policy Debt:** Antiquated data-sharing regulations that hinder innovation.  
* **The Car Funding Model:** The government tends to fund AI as a one-time purchase (like a car) rather than an ongoing, depreciating service that requires perpetual maintenance and updates.

\--------------------------------------------------------------------------------

## **3\. Specialized Industrial Applications**

### **Healthcare and the Healthcare OS**

The vision for healthcare is the creation of a Healthcare Operating System that is autonomous and ubiquitous.

* **Data Interoperability:** AI agents are now capable of screen-scraping and mapping data between different Electronic Medical Records (EMRs) without the need for traditional APIs, potentially breaking the silos maintained by private vendors.  
* **Clinical Diagnostics:** Models such as Med-Gemini are outperforming human doctors on clinical queries, while specialized tools like Luminetics Core can detect diabetic retinopathy at the point of care.  
* **Neural Interfaces:** Technologies like Neuralink and brain-decoding avatars are restoring voice and mobility to paralyzed patients by translating neural activity directly into speech and digital action.

### **Life Sciences and Biology**

AI is revolutionizing biology, but the field remains data-starved at certain levels.

* **The Structural Shift:** While AlphaFold has solved individual protein folding predictions, the industry is still struggling to predict protein-protein interaction networks and neighborhoods.  
* **The Dinosaur Risk:** Academic labs that fail to integrate machine learning are facing natural selection in an era where every Nobel Prize is increasingly powered by AI.

### **Game Design and Iterative Generation**

The use of Iterative Generators (rather than one-shot generators) allows for:

* **Procedural Content Generation (PCG):** Using Reinforcement Learning to ensure that levels are not only aesthetically pleasing but also functional (i.e., solvable for the player).  
* **Wave Function Collapse:** A constraint-solving algorithm used to extrapolate large, complex game worlds from small input patterns.

\--------------------------------------------------------------------------------

## **4\. Market Dynamics: AI Product vs. AI Company**

A critical distinction has emerged between companies that use AI as a feature and those built entirely around AI.

### **The Erosion of Technical Moats**

In the current environment, a technical lead can be erased overnight by a new model release from **OpenAI** or **Google**.

* **The Competitive Advantage:** Shifted toward Go-To-Market (GTM) strategy, community trust, and proprietary data sets.  
* **Wrappers with Staying Power:** A wrapper (an app built on top of a model) is only sustainable if it addresses a specific vertical better than a general model can, leveraging unique community network effects.

### **Transparency and Provenance**

As the internet becomes increasingly poisoned with synthetic data, the economic value of provenance (knowing the source of data) has skyrocketed.

* **SynthID:** Technologies that watermark generated content are essential for maintaining the integrity of data supply chains.  
* **The Trust Battery:** Companies must front-load value to build user trust before asking for the deep commitment of sharing proprietary business data.

| Component | Historical Advantage | AI-Era Advantage |
| :---- | :---- | :---- |
| **Technical Stack** | Proprietary algorithms | Speed of model switching/flexibility |
| **Sales Cycle** | Proof of Concept (PoC) | Transparency of Cognition / Safety Compliance |
| **Data Strategy** | Quantity of data | Quality of held-out or human-validated data |
| **Moat** | Feature set | Community, Trust, and Network Effects |

\--------------------------------------------------------------------------------

## **5\. Critical Future Horizons**

### **Transparency of Cognition**

As we approach more generalized intelligence, the demand for transparency of cognition grows. This involves:

* **Verifiability:** Being able to interrogate the intermediate reasoning steps an AI took to reach a decision.  
* **Anti-Fragility:** Designing systems that get stronger when they are incorrect by utilizing human-in-the-loop verification.

### **The Human Component**

Across all analyzed sectors, healthcare, government, and business, the consensus remains that the human is the most valuable component. AI is an augmentative tool that reduces toil and non-billable work, allowing humans to focus on empathy, ethics, and defining the what while the AI solves for the how.

"What if we were at AGI all along? No, I’m just kidding... but the human is the valuable component",  [**Kory Mathewson**](https://ca.linkedin.com/in/korymath)

# Summary Table

| Company | Founder/Speaker | Industry Focus | Application/Feature | Data Scale | Business Model | Target Customer |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| **BetterCart Analytics** | [Melanie Morrison](https://www.linkedin.com/in/melanie-morrison-bettercart/) | Grocery, Food & Beverage | Automated product matching using algorithms and ML for real-time pricing and competitive insights. | Over 55 million data observations per week. | SaaS and Enterprise (Dynamic pricing based on SKUs). | Retailers, SMB manufacturers, and F\&B brands. |
| **Bobo** | [Grant McDonald](https://www.linkedin.com/in/grant-j-mcdonald/) | Parenting | Distilling developmental data into insights via custom models and LLMs; connecting users to expert services. | Not in source | Commission on transactions and premium subscription. | Parents and families (children ages 0-6). |
| **Jobber** | [David Ferris](https://ca.linkedin.com/in/david-ferris-b31a19114) | Home Services | AI chatbots for queries, automated quoting/invoicing, and agentic voice interfaces for hands-off use. | Proprietary data from hundreds of thousands of SMB customers. | SaaS (Subscription). | Small business owners and tradespeople (SMBs). |
| **Cashew Research** | [Addy Graves](https://ca.linkedin.com/in/addy-graves-56547030) | Market Research / CPG | AI-guided software for research plans, survey customization, and synthesis via a proprietary respondent database. | 33 active customers; database recruited via social media. | Subscription (Volume-based $10,000–$ 70,000). | CPG brands (Food and Beverage). |
| **Bidblox** | [Lisa Mohapatra](https://www.linkedin.com/in/lisamohapatra/) | Construction | AI-first platform for pre-construction bid analysis, procurement workflows, and real-time pricing intelligence. | Projects up to 30-floor condominiums and GCs with $100M+ revenue. | SaaS (Feature-based pricing). | General Contractors, Subtrades, and Suppliers. |
| **Google DeepMind** | [Kory Mathewson](https://ca.linkedin.com/in/korymath) | General Creative / Media | Generative media models (VEO, Imagen, Gemini) for filmmaking, code generation, and creative ecosystems. | High-volume multimodal data (images, video, audio, text). | Subscription (G1), Enterprise, and Ad-supported. | Creatives, developers, and businesses. |
| **Samdesk** | [James Newfeld](https://ca.linkedin.com/in/jamesaneufeld) | Crisis Management / Events | Event detection classifiers processing real-time public data (X, Reddit) to spot crises like wildfires or crime. | 3 million breaking news articles produced annually. | SaaS (Contracts involving security reviews). | Government and Fortune 5,000 security teams. |
| **Nvidia** | [Kateryna Nekhomiazh](https://www.linkedin.com/in/iamkateryna/) | Business Solutions / Robotics | Cosmos World Foundation Models for physical AI simulation and synthetic data generation. | 20 million+ hours of video; 9,000+ trillion tokens. | Hardware (GPUs) and Software (CUDA, SDKs). | Developers, Fortune 5,000, and Robotics/AV firms. |
| **Boosted.ai** | [Joshua Pantony](https://ca.linkedin.com/in/joshua-pantony-266a3243) | Finance | Automates investment workflows, extracts financial models, and manages sales pipelines via document/email scanning. | Large-scale financial documents (e.g., 200-page 10ks). | SaaS / B2B Subscription. | Hedge funds, banks, and portfolio managers. |
| **Exo Imaging (Medo.ai)** | [Jacob Jaremko](https://ca.linkedin.com/in/jacob-jaremko-35854719) / [Abhilash RH](https://www.linkedin.com/in/abhilash-rh-06934964/) | Healthcare | AI-enabled handheld ultrasound for cardiac ejection fraction, lung artifact detection, and hip dysplasia classification. | Videos of approx. 800 frames for rotator cuff analysis. | Hardware and Software SaaS. | Emergency Departments, Nurses, and Physicians. |
| **Clinisys** | [Mehadi Sayed](https://www.linkedin.com/in/mehadi-sayed-87935b2/) | Healthcare | AI-driven EMR, pattern recognition for hospital readmission reduction, and pediatric stroke data analysis. | 5-10 years of historical patient records. | Enterprise Software and AI Solutions. | Hospitals, wellness companies, and clinical trials. |
| **City of Edmonton** | [Kris Andreychuk](https://ca.linkedin.com/in/kris-andreychuk-486350135) | Municipal Government | Wildfire forecasting (EmberWise), risk-based safety inspections, and pothole repair prioritization. | 500,000 annual inspections; 12,000 km of roadways. | Public Service | Edmontonians and Municipal Departments. |
| **AltaML** | [Chantal Ritcey](https://ca.linkedin.com/in/chantal-ritcey-03531250) | Public Sector / Government | Applied AI for wildfire prediction, enrollment forecasting, pavement defect detection, and labor now-casting. | 400+ use cases across 100+ sectors. | Service-based / Consultancy (GovLab). | Government of Alberta, Edmonton, and Calgary. |
| **Verge Agriculture** | [Goddard](https://www.linkedin.com/in/ggodardg/) | Agriculture | Interactive autonomy using satellite imagery for field delineation and route planning to optimize fuel and labor. | Over 34,000 acres of farmland across AB and SK. | SaaS (Per route / bundles / enterprise). | Farmers and OEMs. |
| **InstaDeep** | [Gurneck Singh](https://www.linkedin.com/in/gurneksingh) | Life Sciences / Genomics | Foundation models for DNA sequence reconstruction, genomic segmentation, and multi-modal trait identification. | 850 species; billions of base pairs. | Strategic Partnership / Acquisition (by BioNTech). | Biotech R\&D and Pharmaceutical companies. |
| **DCVC Bio** | [Kiersten Stead](https://www.linkedin.com/in/kstead) | Biotechnology | AI-driven discovery of new targets and antibody generation by analyzing billions of B cells. | 10 billion antibodies from 10 billion different B cells. | Venture-backed drug discovery. | Pharmaceutical companies and researchers. |
| **PCL Construction** | [Brian Gue](https://ca.linkedin.com/in/brian-gue-ab643b1) / [Mark Bryant](https://www.linkedin.com/in/bryantm/) | Construction | Automated cabling/wiring planning (Beline) and identifying discrepancies in CAD drawings and RFPs (Traverse). | Large project-specific data (CAD, RFPs, codes). | Internal use / Potential service. | Internal operations and project owners. |
| **Beacon Data Centers** | [Ken Hughes](https://ca.linkedin.com/in/honourable-ken-hughes-eca-icd-d-aab8a94) / [Ed Depalezieux](https://ca.linkedin.com/in/ed-depalezieux-251b841) | Energy / Infrastructure | High-load AI data center infrastructure utilizing grid-connected power and natural gas. | 400–4,500 Megawatts of power capacity. | Infrastructure as a Service. | Hyperscalers (Fortune 5,000). |
| **RoBIM Technologies** | [Bruce Alton](https://ca.linkedin.com/in/brucealton) | Construction Robotics | Modular robotic fabrication using simulation and AI for picking, placing, and fastening components. | Digital BIM models and robotic feedback loops. | Product sales / Pilot projects. | Commercial and residential construction firms. |
| **Correct-AI** | [Bruce Alton](https://ca.linkedin.com/in/brucealton) | Industrial Safety | Computer vision for collision avoidance by identifying humans vs. objects in heavy equipment blind spots. | Real-time processing across five continents. | Hardware / Software sales. | Industrial sites and heavy equipment operators. |
| Aiden (by **RBC**) | [Greg Mori](https://www.linkedin.com/in/greg-mori-5445b36/) | Capital Markets | Reinforcement learning agent for electronic trading (order execution) to achieve better pricing. | Traded over $100 billion in notional value. | In-house proprietary solution. | Institutional clients and traders. |
| Nomi Forecast (by **RBC**) | [Greg Mori](https://www.linkedin.com/in/greg-mori-5445b36/) | Personal Banking | Selective neural networks used to predict upcoming bills and cash flows based on transaction history. | 10 million plus client interactions. | Bank-integrated service. | Retail banking clients. |
| **Cityscan Technologies** | [Mustafa Gül](https://www.linkedin.com/in/mustafa-g%C3%BCl-5602097/) | Infrastructure | Computer vision for automated pavement assessment and LiDAR integration for structural monitoring. | Network-level assessment (entire municipalities). | SaaS / Platform. | Municipalities and Infrastructure owners. |
| **AutoCanada** | [Russ Fenske](https://ca.linkedin.com/in/russfenske) | Automotive | NLG for vehicle descriptions; STT and NLP for scoring sales calls based on best practices. | 80+ dealerships; 20,000 cars; 6,000 calls. | Not in source | Car Dealerships. |
| **G2V Optics** | Not in source | Horticulture | Precision LED lighting control and computer vision for plant growth optimization and spectral analysis. | High-frequency image data (every 5 minutes). | Not in source | Vertical Farming and Reforestation. |
| **Staircase Ventures** | [Janet Bannister](https://www.linkedin.com/in/janetbannister/) | Venture Capital | Investment in B2B software companies that are AI-first to achieve operational efficiency. | $34 million fund. | Venture Capital. | Canadian B2B Software Startups. |
| **Scribeberry** | [Zaahir Moloo](https://ca.linkedin.com/in/zaahir-moloo-40103758) | Healthcare | AI medical scribe for clinical documentation and automated form completion (e.g., disability tax credit). | Not in source | SaaS (Startup platform). | Physicians and healthcare professionals. |
| **pipikwan pêhtâkwan** | [Shani Gwin](https://www.linkedin.com/in/shanigwin/) | Public Relations | Generative AI plug-in (Wasigan Kisawatwin) to correct bias and misinformation about indigenous peoples. | Not in source | SaaS (B2B) and Free (Consumer). | Corporations, Media, and Government. |
| **Artificial Agency** | [Alex Kearney](https://ca.linkedin.com/in/alexandrakearney) / [Brian Tanner](https://www.linkedin.com/in/bttanner/) | Video Games | Behavior engine for 'living' NPCs and game directors that dynamically modify environments in real-time. | Not in source | B2B / Middleware. | Game Studios and Developers. |
| **Amplify & Elevate Innovation** | [Rebecca Bultsma](https://ca.linkedin.com/in/rebecca-bultsma) | Business / Education | AI training and integration using specialized GPTs and Notebook LM for knowledge management. | Not in source | Consulting and Training Services. | Educators and business organizations. |
| **FKA** | [Rob Jennings](https://ca.linkedin.com/in/robcjennings) | Business Leadership | Accelerating strategic document drafts and image recognition for data entry (screenshots to calendar). | Not in source | Consulting / Billable Hours. | Business Leaders. |
| **TBWA (DDB)** | [Howard Poon](https://ca.linkedin.com/in/howardpoon) | Creative Agency | Conversational brainstorming, source material synthesis via NotebookLM, and AI agents for storyboarding. | Not in source | Agency | Global CPG and Health clients. |
| **Syngenta** | [Gurneck Singh](https://www.linkedin.com/in/gurneksingh) | Agriculture | Foundation models in genomics for identifying novel crop traits and gene editing pivot points. | 48 edible plant species. | Not in source | Agricultural Research / Crop Producers. |
| **RWI Synthetics** | [Krista Davis](https://ca.linkedin.com/in/krista-davis-b712a4a7) | Business Solutions | Synthetic environments and visualization to model complex scenarios and analyze large data sets. | Huge data sets. | Not in source | Enterprise Clients. |
| **Learn Ed Inc.** | [Debra Somani](https://ca.linkedin.com/in/debrasomani) | Business Solutions | Strategic frameworks and advisory for AI-driven transformation and team management. | Not in source | Advisory / Keynote Speaking. | Businesses and Professionals. |
| **FEC Financial Advisory** | [Debra Somani](https://ca.linkedin.com/in/debrasomani) | Finance | Integrating AI to support business optimization and financial advisory services. | Not in source | Advisory / Consulting. | Businesses. |
| **Ask Polly** | Not in source | Market Research | Using AI capabilities to analyze social media data for brand identity and market research. | Not in source | Not in source | Brands and market researchers. |
| **Neuralink** | [Elon Musk](https://en.wikipedia.org/wiki/Elon_Musk) | Neurotechnology | Brain-computer interface (BCI) allowing paralyzed patients to control computers with their minds. | Not in source | Not in source | Patients with paralysis. |
| **Midjourney** | [Max Kreminski](https://mkremins.github.io/) | Creative AI | LLMs and diffusion models for world-building, storytelling, and rapid visual sketching. | Not in source | Not in source | Artists, Writers, and Hobbyists. |
| **Ontopical** | Not in source | Local Government | Unsupervised learning to group and summarize thousands of government meeting agendas and minutes. | Thousands of documents daily. | Not in source | Citizens and tracking businesses. |
| **RL Core Technologies** | [Martha White](https://www.linkedin.com/in/martha-white-49713a59/) | Utility Solutions | Reinforcement learning to optimize water treatment processes, reducing energy and chemical use. | Not in source | Not in source | Water treatment plants / Municipalities. |
| **Circle Cardiovascular** | Not in source | Healthcare | AI-automated workflow for cardiac MRI and diagnostic imaging to increase accuracy. | Not in source | Not in source | Cardiologists in 1,500 hospitals. |
| **SketchDeck.ai** | Not in source | Construction | CV and ML to automatically count structural steel elements and generate material takeoffs. | Not in source | Efficiency-based SaaS. | Estimators and structural engineers. |
| **Pursuit Zen** | Not in source | Business Solutions | LLM trained on past RFP data to automatically generate first drafts of new proposals. | Company historical RFP databases. | Not in source | Businesses bidding on contracts. |
| **QuoteToMe** | Not in source | Supply Chain | Machine vision to read supplier quotes/invoices and match them with purchase orders. | Not in source | SaaS | Construction and supply chain managers. |
| **Sensei Image Tech** | Not in source | Construction Safety | Computer vision in hard hats to translate crane hand signals into multi-language audio. | Not in source | Global product sales. | Crane operators and construction sites. |
| **ZGM** | [Carrie Robinson](https://ca.linkedin.com/in/carrie-denise-robinson) | Marketing | Generative AI for high-velocity content creation and Perplexity for deep market research. | Not in source | Agency / Billable Hours. | Not in source |
| **Compass** | Not in source | Criminal Justice | Risk assessment scores (recidivism prediction) using proprietary pattern matching algorithms. | Not in source | Proprietary Trade Secrets. | Governments and Parole Boards. |
| **Digital Diagnostics** | Not in source | Healthcare | Point-of-care AI tool for detecting diabetic retinopathy from retinal images. | Not in source | Not in source | Family doctors and health clinics. |
| **Visionary** | Not in source | Healthcare | AI Copilot combining EMR data, image data, and patient conversation for clinical results. | Not in source | Not in source | Ophthalmologists and optometrists. |
| **Ground Truth Ag** | Not in source | Agriculture | Automated grain grading using supervised learning and CV to detect damaged grains. | Not in source | Not in source | Grain shipping and storage. |
| **Xkey AiEstimation** | Not in source | Construction | Computer vision to read electrical drawings and count switches, receptacles, and fixtures. | Not in source | Not in source | Electrical contractors and estimators. |
| **Promise Robotics** | [Reza Nasseri](https://www.linkedin.com/in/reza-n-a7325916/) | Construction | Robotic factory system for off-site house fabrication and assembly. | Not in source | Turnkey factory model. | Home developers and const ruction firms. |

