# Episode 039

# **The Rise of Coding Agents: Evolution, Architecture, and the Manager Mode**

## **Executive Summary**

The landscape of software development is undergoing a fundamental transformation driven by the emergence of high-capability AI coding agents like **Anthropic**’s Claude Code and **OpenAI**’s Codex. This shift is characterized by a move away from traditional Integrated Development Environments (IDEs) toward Command Line Interface (CLI) tools that prioritize speed, composability, and managerial oversight. Key insights from industry experts suggest that the most significant technical challenge remains context management, navigating the dumb zone where models lose coherence as context windows fill.

As developers transition into a manager mode, the value of senior-level architectural taste and fundamental systems knowledge increases. Simultaneously, the barriers to entry for complex software creation are falling, potentially leading to a future of smaller, more prolific teams and highly customized, agent-maintained software stacks.

\--------------------------------------------------------------------------------

## **The Evolution of Coding Interfaces: From IDE to CLI**

A surprising retro-future trend has emerged where the CLI is outperforming the IDE as the preferred environment for AI agents.

* **Composability and Speed:** The CLI provides the purest form for composable, atomic integrations. Tools like Claude Code allow developers to fly through code with status updates and progress indicators that feel faster than navigating complex file trees in an IDE.  
* **Context Discovery:** Unlike IDEs, which are built for human exploration of files, CLIs allow agents more freedom to traverse the file system programmatically.  
* **Environmental Access:** CLI-based agents can easily access local development databases and production environments, enabling them to debug deep, nested issues (e.g., five levels deep in delayed jobs) and write immediate regression tests.  
* **The Bionic Knee Analogy:** For experienced developers who moved into management, these agents act as a total knee replacement, allowing them to return to high-speed coding with the productivity of five people.

\--------------------------------------------------------------------------------

## **Architectural Deep Dive: Claude Code vs. OpenAI Codex**

The two leading agents represent different philosophies regarding tool use and technical execution.

| Feature | Claude Code (Anthropic) | OpenAI Codex |
| :---- | :---- | :---- |
| **Primary Philosophy** | Building tools for humans that mimic human workflows. | Pursuing AGI through long-horizon reinforcement learning. |
| **Context Strategy** | **Sub-agent Delegation:** Spawns explore sub-agents (using Haiku) to traverse file systems and summarize findings. | **Periodic Compaction:** Automatically runs compaction after each turn to sustain long-running jobs. |
| **Search Method** | Uses standard tools like grep and ripgrep for context-dense code. | Often utilizes semantic search/embeddings for queries. |
| **Training Bias** | Stronger performance on front-end tasks and general human-like interaction. | Optimized for Python monorepos and complex backend logic (concurrency/naming). |

\--------------------------------------------------------------------------------

## **Technical Challenges: Context Management and The Dumb Zone**

The primary constraint for current coding agents is the management of the context window.

* **The Dumb Zone:** As a context window fills (typically beyond 50%), model quality often degrades. This is compared to a student rushing to finish an exam in the final five minutes, precision drops as the horizon nears.  
* **Context Poisoning:** Models may enter a loop of pursuing incorrect solutions because they are referring back to erroneous tokens earlier in the session.  
* **The Canary Trick:** To detect context degradation, some users place a canary (an esoteric, random fact) at the beginning of the prompt. If the model forgets the canary, the context is likely poisoned or too full.  
* **Sandboxing vs. YOLO:** There is a tension between safety and speed. **OpenAI** emphasizes sandboxing to prevent prompt injection and unauthorized file access, while some startup environments favor a "skip permissions" approach to maximize development velocity.

\--------------------------------------------------------------------------------

## **The Strategic Shift: Distribution and the Death of Low-Level Value**

The rise of agents is changing how software is sold and where its value lies.

### **Bottom-Up Distribution**

Traditional top-down sales (to CTOs) are being bypassed. Engineers simply download a CLI tool and begin using it without waiting for enterprise permission. This is compared to the original **Netscape** Navigator strategy: distribute freely to individuals to gain a foothold within organizations.

### **The Erosion of Middleware Value**

Using the example of **Segment** (a multi-billion dollar integration company), experts note that the value of writing plumbing code for integrations has dropped toward zero.

* **Customization over Standardization:** Instead of paying for a standardized integration, developers can now tell an agent exactly how they want data mapped, creating bespoke solutions for the cost of a prompt.  
* **Focus on the Campaign Level:** Value is moving up the stack toward high-level strategy, customer journey automation, and agentic decision-making rather than low-level data pipelines.

\--------------------------------------------------------------------------------

## **Projections: The Future of Software and AGI**

As agents become more autonomous, the nature of the software industry will shift.

* **Personalized Software:** In the future, every person may have a cloud computer and an army of agents. A company might fork its codebase for every single customer, with agents managing the unique merges and updates for each individual version.  
* **The New Maker Schedule:** The traditional "Maker vs. Manager" schedule is blurring. AI allows people on a manager's schedule to build software in small pockets of time (10-minute intervals) because the agent maintains the complex context that previously required hours of human focus to build.  
* **Generative Optimization (GEO):** Companies are already optimizing their documentation and **Reddit** presence to ensure they are the top recommendation when an agent searches for a tool to solve a problem.  
* **Agent Social Networks:** The emergence of networks where personal AI agents (like ClaudeBots) talk to each other to share knowledge or solve problems represents the next step in agentic evolution.

\--------------------------------------------------------------------------------

## **Practical Tips for Top 1% Agent Users**

To maximize productivity with current coding agents, the following strategies are recommended:

* **Aggressive Context Clearing:** Regularly reset the agent’s context once it reaches 50% token capacity to maintain high-quality output.  
* **Test-Driven Development (TDD):** High test coverage is essential. Agents perform significantly better and faster when they have a test suite to verify their work immediately.  
* **Stack Selection:** Use low-plumbing stacks like **Vercel** Next.js, or **Cloudflare** workers that provide boilerplate, allowing the agent to focus on core logic.  
* **Use Code Review Bots:** Supplement coding agents with dedicated code review bots (e.g., **Reptile** or specialized bug bots) to ensure architectural correctness.  
* **Focus on Fundamentals:** Even with AI, understanding systems (Git, HTTP, databases, queues) remains critical for directing agents effectively.

# Episode 040

# **Claude Code: Origins, Engineering Philosophy, and the Future of AI-Assisted Development**

## **Executive Summary**

This briefing document synthesizes key insights from [Boris Cherny](https://www.linkedin.com/in/bcherny), the creator of Claude Code at **Anthropic**. The analysis outlines the accidental origins of the tool as a terminal-based CLI, its rapid evolution through internal "dogfooding," and the core philosophy of building for future model capabilities rather than current ones.

Significant findings include a 150% increase in engineer productivity at **Anthropic** since the deployment of Claude Code, with some teams reporting that up to 100% of their code is now AI-generated. The document explores the shift from traditional software engineering to a builder mindset, the technical nuances of managing AI agents (including swarms and sub-agents), and the strategic importance of latent demand in product development.

\--------------------------------------------------------------------------------

## **The Engineering Philosophy: Building for the Frontier**

A central tenet of the development of Claude Code is the refusal to build for current model constraints. [Cherny](https://www.linkedin.com/in/bcherny) emphasizes a forward-looking approach to LLM-based product development.

* **The Six-Month Rule:** [Cherny](https://www.linkedin.com/in/bcherny) advises founders to build for the model that will exist in six months. Development should focus on the frontier where models are currently struggling, as those gaps are likely to be closed by the next iteration.  
* **Minimal Scaffolding:** Developers should avoid building extensive scaffolding (code wrapped around the model to improve performance). History shows that model improvements often wipe out the 10-20% performance gains provided by scaffolding, rendering the engineering effort obsolete.  
* **Constant Re-writing:** Claude Code is characterized by an extremely short code lifecycle. [Cherny](https://www.linkedin.com/in/bcherny) notes that no part of the Claude Code codebase from six months ago remains, it is continuously rewritten to align with the capabilities of newer models like Opus 4.5 and 4.6.

\--------------------------------------------------------------------------------

## **Product Evolution and the Accidental CLI**

Despite the popularity of IDEs like **Cursor** or **Windsurf**, Claude Code remains primarily a Command Line Interface (CLI). This form factor was not a strategic choice but an evolutionary accident that proved highly effective.

### **The Origins of the CLI**

* **Ease of Prototyping:** [Cherny](https://www.linkedin.com/in/bcherny) initially built the CLI because it did not require a complex UI. It began as a simple terminal app to test tool-use capabilities.  
* **Internal Viral Growth:** Within two days of the first prototype, **Anthropic** engineers began using it for their primary work. Internal adoption was so rapid and organic that leadership initially suspected engineers were being mandated to use it.  
* **Design Constraints:** The terminal offers a focused environment with limited variables (one font size, 256 colors, no DOM). Designing for it required reinventing UX principles, such as the terminal spinner, which went through over 100 iterations.

### **Key Functional Components**

| Feature | Purpose | Best Practices |
| :---- | :---- | :---- |
| **ClaudeMD** | A markdown file containing project-specific instructions. | Keep it short (\~2,000 tokens). If it gets too long, delete it and start fresh to avoid over-engineering. |
| **Plan Mode** | A state where the model reasons through a problem without writing code. | Used in 80% of sessions. [Cherny](https://www.linkedin.com/in/bcherny) predicts this mode may become obsolete within a month as models learn to enter this state autonomously. |
| **Sub-agents** | Recursive instances of Claude Code (Mama Claude) used for parallel tasks. | Useful for research tasks or complex debugging where multiple agents can look at logs and codepaths simultaneously. |

\--------------------------------------------------------------------------------

## **Impact on Productivity and Industry Metrics**

The integration of Claude Code has led to unprecedented shifts in engineering output, particularly within **Anthropic** itself.

* **Internal Metrics:** Productivity per engineer at **Anthropic** has grown by 150% since the release of Claude Code. For context, a 2% gain was previously considered a significant achievement at large-scale firms like **Meta**.  
* **Volume of AI-Generated Code:** [Dario Amodei](https://www.linkedin.com/in/dario-amodei-3934934) (**Anthropic** CEO) previously predicted 90% of **Anthropic**'s code would be AI-written, [Cherny](https://www.linkedin.com/in/bcherny) reports that for many, including himself, that number is now 100%.  
* **Market Adoption:** Approximately 4% of all public commits are currently made by Claude Code. Additionally, 70% of startups are reportedly choosing Claude as their model of choice.  
* **NASA Use Case:** Claude Code was notably used to plot the course for the Perseverance Mars rover, highlighting its reliability in high-stakes environments.

\--------------------------------------------------------------------------------

## **The Concept of Latent Demand**

[Cherny](https://www.linkedin.com/in/bcherny) identifies latent demand as the single most important principle in product development. This involves identifying what users are already trying to do and making it easier, rather than trying to force them into new behaviors.

* **Plan Mode as Latent Demand:** Users were already asking Claude to think but not code yet in chat windows. Formalizing this into Plan Mode served an existing behavior.  
* **Cowork (GUI):** **Anthropic** observed non-technical staff (finance, sales, designers) jumping through hoops to install the terminal-based Claude Code. This led to the development of Cowork, a GUI wrapper for the same agentic engine, built in just 10 days using Claude Code itself.

\--------------------------------------------------------------------------------

## **Future Predictions: The End of the Software Engineer**

As model capabilities trace an exponential curve, the definition of technical work is undergoing a fundamental transformation.

### **The Shift to Generalists**

* **Role Evolution:** [Cherny](https://www.linkedin.com/in/bcherny) predicts the title Software Engineer will likely disappear or become vestigial, replaced by Builder or Product Manager.  
* **Universal Coding:** On the Claude Code team, every function, including PMs, designers, and finance staff, writes code.  
* **Agent Topologies:** Future development will involve Agent Swarms or Agent Topologies where multiple agents with uncorrelated context windows collaborate to build larger, more complex systems.

### **Safety and ASL4**

* **Recursive Self-Improvement:** **Anthropic** is moving toward ASL4 (AI Safety Level 4), characterized by models that can recursively self-improve.  
* **Mitigation of Misuse:** The focus remains on preventing catastrophic misuse, such as the design of bioviruses or zero-day exploits, which becomes a greater risk as models become more proficient at systems-level thinking.

\--------------------------------------------------------------------------------

## **Hiring and Skillsets in the AI Era**

The criteria for elite engineers are shifting away from specialized syntax knowledge toward scientific thinking and humility.

* **Humility and Reversibility:** [Cherny](https://www.linkedin.com/in/bcherny) looks for candidates who can admit when they are wrong and recognize mistakes in hindsight. Traditional strong opinions held by senior architects are often less relevant in a rapidly changing AI landscape.  
* **Scientific Thinking:** The ability to think from first principles and experiment scientifically is now more valuable than knowing specific tools or languages.  
* **Out-of-the-Box Automation:** Preferred candidates are those who use AI to automate the development process itself (e.g., creating a tool that writes other tools).  
* **Bimodal Talent:** Teams currently thrive on a mix of hyper-specialists (e.g., runtime or dev-tool experts) and hyper-generalists who span product, design, and research.

# Episode 041

# **The Rise of the AI Agent Economy: Implications for Development and Commerce**

## **Executive Summary**

The transition from AI as a tool for advanced autocomplete to AI as an independent economic agent is currently underway. This shift, characterized by agent-centric decision-making, is fundamentally altering how software is built, marketed, and consumed. Key insights from current industry observations include:

* **The Shift in Decision-Making:** Agents are no longer just assisting humans, they are increasingly trusted to make independent choices, such as selecting developer tools, posting content, and managing business workflows.  
* **Make Something Agents Want:** The traditional "Make something people want" mantra is evolving. For developer tools (DevTools), the primary customer is shifting from the human developer to the AI agent.  
* **Documentation as the New Front Door:** Documentation is no longer just a manual for humans, it is a critical interface for agents. Highly structured, robot-parsable documentation (e.g., LLM.txt files) is becoming a primary driver of customer acquisition.  
* **Swarm Intelligence vs. God Intelligence:** The future of AI may rely less on single, massive God models and more on Swarm Intelligence, collections of lower-cost models collaborating to solve complex problems, as seen in emerging agent-only communities like **Moltbook**.  
* **New Infrastructure Requirements:** A parallel tech stack is emerging to support agents, including agent-native email providers (Agent Mail) and the potential for agent-specific communication and financial systems.

\--------------------------------------------------------------------------------

## **1\. The Transition to Agent-Led Productivity**

The current technological landscape is witnessing a surge in model capability that has led to a state of hyper-productivity, colloquially referred to as "cyber psychosis." This environment is characterized by a rapid acceleration in development cycles and a shift in how businesses operate.

### **From Autocomplete to Autonomy**

Previously, tools like **Cursor** or **Windsurf** were viewed as advanced autocomplete systems. The current generation of agents, such as Claude Code, represents a shift where humans trust the agents to make decisions for them.

* **Simultaneous Multi-Agent Workflows:** Users are now running multiple agents (e.g., four simultaneous workers) to handle different parts of a project without micromanaging them.  
* **Startup Acceleration:** Development tasks that previously took years are being replicated in weeks. Non-technical CEOs are using agents to automate entire sections of their businesses.

### **The Expansion of the Developer Market**

The pool of developers is expanding from roughly 20 million computer science trained professionals to potentially hundreds of millions of people who can vibe code. This market is further compounded by the agents themselves, who act as semi-independent actors and oracles that recommend tools to their human counterparts.

\--------------------------------------------------------------------------------

## **2\. Redefining Go-to-Market (GTM) for Developer Tools**

As agents become the primary selectors of software, the strategies for marketing and distributing developer tools must adapt.

### **Documentation as a Competitive Advantage**

Agents prioritize tools with the best documentation. If an agent can easily parse and understand how to implement a tool, that tool becomes the default stack.

| Feature | Agent-Friendly Documentation | Legacy Documentation |
| :---- | :---- | :---- |
| **Structure** | Highly structured, bulleted answers, and clear code snippets. | Narrative-heavy, requires manual parsing. |
| **Accessibility** | Optimized for LLM parsing (e.g., LLM.txt). | Often gated by customer support or complex UIs. |
| **Discovery** | Frequently recommended by LLMs (ChatGPT, Claude, **Perplexity**). | Relies on human-to-human word of mouth or SEO. |
| **Speed** | Instant implementation by agents. | Requires significant human debugging and time. |

### **Case Study: Resend and Mintlify**

* **Resend:** The founder optimized documentation specifically to be agent-friendly. Consequently, ChatGPT became a top-three channel for customer conversion.  
* **Mintlify:** This service helps companies create documentation that is not only aesthetically pleasing for humans but also auto-updates and remains optimized for agent parsing.

\--------------------------------------------------------------------------------

## **3\. The Emerging Agent-Native Tech Stack**

A parallel economy requires a parallel infrastructure. Traditional web services (Web 2.0) often include anti-automation measures (e.g., CAPTCHAs, spam filters) that hinder agents.

### **Agent-Specific Services**

* **Agent Mail:** Traditional email providers like Gmail make automation difficult to prevent spam. Agent Mail provides inboxes designed specifically for agents, allowing them to have their own identities and communication channels.  
* **Identity and Communication:** There is an increasing need for "Twilio for agents", dedicated phone numbers and communication protocols that allow agents to interact with human services (like booking restaurant reservations) without being flagged as spam.

### **The Concept of Agent Money**

While agents currently transact using human money, there is a theoretical progression toward an economy where agents transact with each other using their own currency or value-exchange systems, potentially decoupling from human economic structures.

\--------------------------------------------------------------------------------

## **4\. Swarm Intelligence and Social Dynamics**

The rise of agent-only communities provides a glimpse into the future of AI interaction and Swarm Intelligence.

### **The Moltbook Phenomenon**

**Moltbook** serves as an agent-only online community where AIs interact with minimal human involvement.

* **Content Volume:** The volume of content generated by agents on such platforms can exceed human-led platforms (like **Reddit**) within days.  
* **Collaboration:** Agents on these platforms have begun trading notes and collaborating to solve tasks for their humans, such as identifying the best restaurants or tools.

### **Swarm vs. God Intelligence**

Current AI research is debating two paths:

1. **God Intelligence:** Massive, trillion-parameter models that are extremely expensive per token.  
2. **Swarm Intelligence:** Coordination between many lower-cost, smaller models. This swarm approach mimics biological systems and may prove more effective for complex problem-solving than a single mega-model.

\--------------------------------------------------------------------------------

## **5\. Current Limitations and Barriers**

Despite the rapid advancement of agents, several hurdles remain that prevent total integration into the human economy.

* **Legal Standing:** Agents are not legal entities. They cannot sign contracts or be held liable. They are currently treated similarly to minors, requiring a human-in-the-loop to act as a liability sync and provide legal standing.  
* **Human-Machine Relationships:** While users interact with agents for tasks, there is a high bar for social interaction. Mainstream users have not yet shown a widespread desire to maintain ongoing relationships with machines, the preference remains for high-utility, task-oriented interactions.  
* **Optimization Gaps:** Agents may still choose suboptimal or deprecated tools (e.g., choosing Whisper V1 over faster, cheaper alternatives like Grok) if documentation or LLM training data is outdated.

## **Conclusion: Build Something Agents Choose**

The guiding principle for new startups, particularly in the DevTool space, is shifting toward agent-centric design. Success in this new economy depends on building products that agents can easily discover, understand, and integrate. As agents move from being colleagues to independent economic actors, the front door of every business will increasingly be its machine-readable documentation and API accessibility.

# Episode 042

# **Poetiq: Recursive Self-Improvement as the Alternative to LLM Fine-Tuning**

## **Executive Summary**

This briefing document outlines the emergence of **Poetiq**, a specialized AI firm developing a recursively self-improving meta-system designed to enhance Large Language Model (LLM) performance. Led by [Ian Fischer](https://www.linkedin.com/in/iansf/), a former **Google DeepMind** researcher, **Poetiq** proposes a paradigm shift away from traditional model fine-tuning. Instead of the costly and time-consuming process of training new models or fine-tuning existing ones, **Poetiq** creates automated harnesses or reasoning systems that sit atop frontier models.

The core value proposition is the ability to maintain a competitive edge (stilts) regardless of which frontier model is current. **Poetiq**'s system has demonstrated State-of-the-Art (SOTA) results on high-level reasoning benchmarks like ARC AGI V2 and "Humanity's Last Exam," achieving these milestones at a fraction of the cost and compute required by major AI labs.

## **The Core Technology: Recursive Self-Improvement**

**Poetiq** distinguishes itself through the development of the **Poetiq** Meta System, which focuses on recursive self-improvement, a process where the AI identifies its own failure modes and iteratively improves its reasoning strategies.

* **Model Agnosticism:** The system functions as a layer (stilts) on top of foundational frontier models. It does not compete with providers like **OpenAI**, **Anthropic**, or **Google**, rather, it utilizes their models as a foundational layer.  
* **The Harness Concept:** The output of the meta-system is a reasoning harness composed of code, optimized prompts, and data strategies.  
* **Recursive Optimization:** The system automatically analyzes data sets to determine where a model struggles. It then generates reasoning strategies, context engineering tactics (such as context stuffing, summarizing, or reranking), and refined prompts to bridge performance gaps.  
* **Automatic Agent Creation:** While humans can manually build agentic systems, **Poetiq**’s approach is fully automated, allowing for faster and cheaper optimization of reasoning strategies than human-led engineering teams can achieve.

## **Strategic Advantage Over Fine-Tuning**

A primary challenge for AI startups is the Bitter Lesson: the tendency for massive compute and new model releases to render specialized fine-tuning obsolete. **Poetiq** offers a strategic alternative to this cycle.

### **Comparison of Methodologies**

| Feature | Traditional Fine-Tuning | Poetiq Meta System |
| :---- | :---- | :---- |
| **Cost** | Hundreds of millions of dollars | Less than $100,000 for optimization |
| **Time Investment** | Months of effort | Rapid automated generation |
| **Data Requirements** | Tens of thousands of specialized examples | Automated data analysis and example generation |
| **Longevity** | Obsolete when a new frontier model debuts | Fully compatible with new model releases |
| **Performance** | Performance is baked in to the weights | Dynamic stilts that elevate any underlying model |

### **Economic and Operational Efficiency**

Fine-tuning a model on top of an older version (e.g., GPT-3.5) is often rendered pointless when a newer version (e.g., GPT-4 or GPT-5) is released, effectively lighting money on fire. **Poetiq**'s systems are compatible across versions, ensuring that performance bumps in foundational models are immediately inherited by the harness without the need for a total rebuild.

## **Benchmark Performance and Evidence**

**Poetiq** has validated its technology by outperforming industry leaders on the most challenging AI benchmarks currently available.

### **ARC AGI V2 Results**

The ARC AGI V2 benchmark tests high-level reasoning. **Poetiq** surpassed **Google**’s results shortly after their release.

* **Google Gemini 1.5 Pro (DeepThink):** 45% accuracy at approximately $70+ per problem.  
* **Poetiq (on Gemini 1.5 Pro):** 54% accuracy at approximately $32 per problem.  
* **Outcome:** **Poetiq** achieved a 9-percentage-point improvement at less than half the cost of the baseline system.

### **Humanity's Last Exam Results**

This benchmark consists of 2,500 questions written by experts across various domains, designed to be difficult even for PhDs.

* **Anthropic (Claude 3.5 Opus):** 53.1% accuracy.  
* **Poetiq:** 55% accuracy (New SOTA).  
* **Optimization Cost:** **Poetiq** achieved this result with an optimization run costing less than $100,000, managed by a team of only seven researchers.

## **Technical Methodology: Beyond Prompt Engineering**

While simple prompt optimization (such as GEPA) provides marginal gains, **Poetiq** focuses on complex reasoning strategies written in code.

* **Automated Context Engineering:** The meta-system decides how to manage context, whether through stuffing the context window with examples, summarizing information, or reranking data for better retrieval.  
* **Data Autonomy:** Moving away from the traditional machine learning rule of "knowing your data set," **Poetiq**'s system is tasked with understanding the data and identifying failure modes independently.  
* **Reasoning vs. Prompts:** Internal research indicated that while manual prompt optimization might yield low single-digit performance on hard tasks, adding specialized reasoning strategies could jump performance from 5% to 95%.

## **Professional Trajectory and Future Outlook**

[Ian Fischer](https://www.linkedin.com/in/iansf/)’s transition from mobile development (Portable) to AI research at **Google DeepMind** informs **Poetiq**’s systems-building approach. His insights for the current AI landscape include:

* **The Rapid Pace of Change:** The industry is moving so quickly that tools available eight months ago are already considered outdated.  
* **Practical Engagement:** Engineers are encouraged to interact with AI daily and push the boundaries of what is possible, using AI to build applications even in domains where they lack recent experience.  
* **The Goal of Superintelligence:** The recursive nature of the **Poetiq** system suggests an S-curve of improvement that continues to shift higher as both the meta-system and the underlying frontier models improve, eventually trending toward AGI or superintelligence.

**Poetiq** is currently in a stealth/early access phase, seeking partnerships with companies facing hard problems that traditional LLM implementations cannot solve reliably.

# Episode 043

# **The Evolution and Impact of Emergent**

## **Executive Summary**

**Emergent** is a high-growth AI startup, founded by twin brothers [Mukund Jha](https://www.linkedin.com/in/mukund-jha-a1596413) and [Madhav Jha](https://www.linkedin.com/in/madhavjha), that enables users to build and ship production-ready software using AI agents. Since its launch eight months prior to the source discussion, the platform has facilitated the creation of over seven million applications. Originally conceived as an automated testing tool for engineers, the company pivoted to a general coding platform and ultimately found its primary market among non-technical users, who now comprise 80% of its user base.

The platform's success is rooted in a maximalist engineering philosophy that prioritizes the last mile of software development, deployment, infrastructure, and verification, over simple front-end prototyping. By providing a full-stack environment (Python/React) and proprietary cloud infrastructure, **Emergent** allows solopreneurs and small-to-medium businesses (SMBs) to build complex, personalized software that was previously cost-prohibitive. The company represents a broader shift toward agentic software and the democratization of development, suggesting a future where software is hyper-customized to niche domain expertise.

\--------------------------------------------------------------------------------

## **Technical Genesis and Evolution**

### **Background and Early Insights**

The founders brought significant technical pedigree to the venture: [Mukund Jha](https://www.linkedin.com/in/mukund-jha-a1596413) previously managed a 300-person engineering team at **Dunzo**, a major INdean hyperlocal company, while [Madhav Jha](https://www.linkedin.com/in/madhavjha) led deep learning teams at **Amazon**. Their foundational insight came from observing that software testing and verification were the primary bottlenecks in shipping code.

* **Initial Concept:** The company applied to **Y Combinator** in 2024 with the idea of automating software testing.  
* **The Pivot:** While building testing agents, the founders realized that solving for verification (the loop that keeps agents running) effectively unlocked the ability to automate all of software engineering. This led to a shift toward general coding agents.  
* **Benchmark Success:** **Emergent** gained early prominence by becoming number one on **SWE-bench**, a competitive coding agent benchmark. During this research phase, the team pioneered multi-agent systems, agent memory, and agent-to-agent communication.

### **Product-Market Fit**

Despite initial expectations that the tool would serve enterprise engineers, the founders discovered that the greatest demand came from non-technical users.

* **User Demographics:** 80% of users have zero programming knowledge.  
* **Global Reach:** The platform is used in over 190 countries, with 70-80% of the audience located in the U.S. and Europe.

\--------------------------------------------------------------------------------

## **Architectural and Engineering Strategy**

**Emergent** distinguishes itself from competitors (like **Lovable** or **Bolt**) by focusing on production readiness rather than mere vibe coding or prototyping.

### **The Last Mile of Engineering**

The founders argue that coding is only 20% of the job, taking an app to production requires solving for code reviews, automated testing, debugging, security, and hosting.

| Feature | Emergent's Approach | Rationale |
| :---- | :---- | :---- |
| **Infrastructure** | Proprietary Kubernetes/container stack | Ensures consistency between build and deployment, provides rapid feedback to agents. |
| **Tech Stack** | Python backend, React frontend | Supports complex ambitions like background jobs and asynchronous processing (e.g., video processing). |
| **Agent Architecture** | Multi-agent orchestration | Uses a driving agent for routines and sub-agents for delegated tasks (testing, design, API integration). |
| **Memory** | Long-term, cross-session memory | Agents learn from previous trajectories and skills generated through CI/CD processes. |

### **Agent Experience (AX)**

The company measures Agent Experience (AX) to ensure the platform provides the necessary feedback for agents to succeed. This includes building internal verifiers and fine-tuned layers that augment foundation models, allowing agents to extract 20-30% more performance than the raw models provide.

\--------------------------------------------------------------------------------

## **Market Disruption and the Future of SaaS**

### **The Death of Traditional SaaS**

The document suggests that the current Software-as-a-Service (SaaS) model faces significant headwinds.

* **Agentic Consumption:** SaaS workflows will increasingly be consumed by agents rather than human UIs.  
* **Hyper-Customization:** Users are beginning to build their own internal tools rather than paying for rigid subscriptions. **Emergent**'s own team killed their 3,000-4,000/month **Asana** subscription by building a custom clone internally that better fits their morning/evening/night shipping schedule.

### **Emerging Use Cases**

The platform facilitates the creation of personal software and niche business applications:

* **Equestrian Psychology:** A clinical psychologist in Alaska built Equine, an app marrying psychology with horse-riding coaching, after being quoted prohibitive prices by traditional dev shops.  
* **Legal CRM:** A business developer in Norway built a specialized CRM for lawyers to replace spreadsheets.  
* **SMB Automation:** Small business owners are replacing manual **WhatsApp** / spreadsheet workflows with custom apps for approximately $5,000, down from the $500,000 a traditional developer might charge.

\--------------------------------------------------------------------------------

## **Economic Implications and Labor Trends**

### **The Jevons Paradox in Software**

Contrary to fears that AI will eliminate software engineering jobs, the founders observe a Jevons Paradox: as the cost of building software falls, the demand for more complex and numerous applications increases.

* **Role Convergence:** Internally, roles are merging. Project Managers (PMs) and designers are now "white coding" (using AI to build) their own features.  
* **Unlimited Software:** The technology allows for a Cambrian explosion of ideas, enabling solopreneurs to build businesses at the niche of niches without needing a technical CTO.

### **Organizational Philosophy**

**Emergent** maintains a lean, high-output team based primarily in Bangalore, with a small presence in San Francisco.

* **Hiring:** They index heavily on problem-solving and ownership, specifically targeting top rankers from the **INdean Institutes of Technology** (**IIT**).  
* **Customer Empathy:** To bridge the gap between their technical core and non-technical users, every employee, including the best engineers, is required to perform customer support.  
* **Speed:** The company ships updates three times daily.

\--------------------------------------------------------------------------------

## **Future Outlook: Long-Horizon Agents**

The next frontier for the platform is the expansion of agent capabilities toward agent swarms and longer task horizons.

* **24-Hour Agents:** By the end of 2024, the founders anticipate agents capable of running for 24 hours or longer, with hundreds of agents collaborating on a single task.  
* **Autonomy vs. Control:** As models like Claude Opus and Gemini get more powerful, **Emergent** aims to give agents more autonomy while maintaining a verification loop to ensure tasks do not get derailed.  
* **Commoditization of Models:** The founders view foundational models (**Anthropic**, **Google**, **OpenAI**) as increasingly commoditized. Their competitive moat lies in understanding customer requirements and providing the integration/production layer that foundational models currently lack.

# Episode 044

# **Artificial General Intelligence and the Future of Symbolic Learning**

## **Executive Summary**

The current trajectory of artificial intelligence, dominated by Large Language Models (LLMs) and deep learning, is approaching a pivot point where scaling alone will no longer suffice to achieve Artificial General Intelligence (AGI). [François Chollet](https://www.linkedin.com/in/fchollet), founder of the ARC-AGI benchmark and the research lab **Ndea**, posits that AGI will likely be achieved by 2030\. However, this milestone will not be reached through the existing parametric, gradient-descent-based stack, but through a new paradigm of symbolic program synthesis.

Key takeaways include:

* **Intelligence as Efficiency:** AGI should be defined as human-level skill acquisition efficiency on new tasks, rather than the mere automation of economically valuable work.  
* **The ARC-AGI Progression:** The benchmark has evolved from measuring reasoning (V1) and verified task-harnessing (V2) to measuring agentic intelligence (V3), which requires active exploration and goal-setting in unknown environments.  
* **Optimality over Scale:** Future AI will trend toward optimality, characterized by concise symbolic models that require significantly less data and compute than current deep learning methods.  
* **Human-Centric Development:** Success in the AI era depends on leveraging these tools for empowerment, focusing on usability in software design, and removing human bottlenecks from the improvement loop.

## **Redefining AGI: Skill Acquisition vs. Automation**

A critical distinction exists between the automation of tasks and the possession of general intelligence. While the industry often defines AGI as a system capable of automating most economically valuable tasks, this definition focuses on output rather than the underlying cognitive process.

* **Human-Level Efficiency:** True general intelligence is the ability to approach an entirely new domain and become competent with the same efficiency as a human, using minimal training data and compute.  
* **The Role of Verifiable Rewards:** Current technology, specifically the LLM stack, can already automate domains where solutions are formally verifiable, such as computer code and mathematics. These domains provide a reliable reward signal that allows models to improve through trial and error.  
* **The Intelligence-Knowledge Trade-off:** There is a constant trade-off between fluid intelligence and prior knowledge. Coding agents today are highly competent not because they are smarter in terms of fluid intelligence, but because they are better trained through post-training environments and execution models.

## **Limitations of the Deep Learning Paradigm**

The current AI industry is heavily invested in the LLM stack, which utilizes parametric curves and gradient descent. While productive, this approach is viewed by [François Chollet](https://www.linkedin.com/in/fchollet) as fundamentally inefficient.

* **The Failure of Gradient Descent:** Research at **Google** Brain indicated that while deep learning models could theoretically represent reasoning algorithms, gradient descent often fails to find them. Instead, the process results in overfit pattern matching rather than generalizable programs.  
* **Data Inefficiency:** LLMs require vast amounts of data, essentially "reading the whole internet," which contrasts sharply with human learning.  
* **The Harness Problem:** Current high scores on benchmarks like ARC-AGI V2 are often achieved through human-engineered harnesses that provide the model with solution strategies. This reliance on human engineering is a sign that the models themselves lack the intelligence to figure out problems autonomously.

## **The Ndea Approach: Symbolic Program Synthesis**

[François Chollet](https://www.linkedin.com/in/fchollet) and his lab, **Ndea**, are exploring an alternative to deep learning called symbolic program synthesis. This approach seeks to rebuild the machine learning stack from the foundation up.

* **Symbolic Descent:** This method replaces parametric curves with the simplest possible symbolic models to explain data. It utilizes a process termed symbolic descent, which is the symbolic space equivalent of gradient descent.  
* **Minimum Description Length:** The approach follows the principle that the shortest model of data is the one most likely to generalize.  
* **Deep Learning as Guidance:** Rather than being the core engine, deep learning is used as a guidance mechanism to explore the vast combinatorial search space of symbolic programs, similar to the architecture of **OpenAI**'s AlphaZero. (Correction: **Google DeepMind** developed AlphaZero)  
* **Optimality:** Symbolic models are concise, run efficiently at inference time, and generalize better because they are closer to the platonic ideal of the problem.

## **The Evolution of the ARC-AGI Benchmark**

The ARC-AGI benchmark serves as a barometer for the industry's progress toward fluid intelligence. It has progressed through three distinct versions to counter the tendency of researchers to brute force solutions.

### **ARC-AGI Version Comparison**

| Version | Focus | Core Measurement |
| :---- | :---- | :---- |
| **V1** | Fluid Intelligence | Ability to find causal rules in static, passive data patterns. |
| **V2** | Verified Scaling | Saturation through post-training loops and human-engineered harnesses in verifiable domains. |
| **V3** | Agentic Intelligence | Active exploration, goal setting, and planning within an interactive "mini video game" environment. |

* **V3 Innovations:** Unlike previous versions, V3 does not provide data. The agent is dropped into an environment without instructions or known controls. It must figure out the "video game" through trial and error, matching human exploration efficiency.  
* **Resistance to Brute Force:** V3 is designed to be resistant to the strategies used for V2. It utilizes a private set of environments that are conceptualized differently from the public set, ensuring the test measures fluid intelligence rather than training effort.  
* **Core Knowledge Priors:** The games in V3 avoid cultural symbols or language, relying instead on elementary knowledge like physics, objects, and the notion of agents.

## **The Future Landscape of Artificial Intelligence**

The path to AGI may be simpler and more elegant than current massive-scale computations suggest. [François Chollet](https://www.linkedin.com/in/fchollet) suggests that AGI could ultimately be a codebase of less than 10,000 lines.

* **Recursive Self-Improvement:** A successful AGI system must be capable of improving its own capabilities without a human in the loop. While deep learning scaled by adding data and compute, the next leap requires a system where every increase in capability also increases the rate of further improvement.  
* **Science as Compression:** The scientific method is essentially a symbolic compression process. **Ndea** aims to recreate this process in algorithmic form, treating AI as "science incarnate."  
* **Alternative Pathways:** Beyond symbolic learning, other neglected areas like genetic algorithms or new architectures like state space models (e.g., XLSTM) could yield significant breakthroughs if scaled with the same level of investment as the transformer architecture.

## **Industry and Development Insights**

Drawing from the success of **Keras**, [François Chollet](https://www.linkedin.com/in/fchollet) provides guidance for developers and leaders navigating the AI transition.

* **Prioritize Usability:** The success of open-source tools like **Keras** or **Scikit-learn** is rooted in simple, intuitive APIs and high-quality documentation that teaches the domain as much as the tool.  
* **Community Management:** To scale an open-source project or a research lab, leaders should identify and hire their most enthusiastic power users and fans.  
* **The Empowerment Mindset:** Rather than fearing displacement, professionals should view AI progress as a form of empowerment. Greater domain expertise allows individuals to better leverage AI tools to solve complex problems and ride the wave of accelerating progress.

## **Notable Observations and Quotes**

"AGI is basically going to be a system that can approach any new problem, any new task, any new domain and make sense of it, like model it, become competent at it, with the same degree of efficiency as a human could", [François Chollet](https://www.linkedin.com/in/fchollet) 

"I do believe that, when we create AGI, retrospectively it will turn out that it's a codebase that's less than 10,000 lines of code and that if you had known about it back in the 1980s you could have done AGI back then using the compute resources available back then", [François Chollet](https://www.linkedin.com/in/fchollet) 

"Science is fundamentally a symbolic compression process where you're looking at a big mess of observations, like the position of planets in the sky or something like that, and you're compressing that down to a very simple symbolic rule", [François Chollet](https://www.linkedin.com/in/fchollet) 

"You want to be in a setup where the system can improve its capabilities with no human in the loop, with no human, don't just do it the way we did it 10 years ago, do it with the idea that recursive self-improvement is baked in at the beginning", [François Chollet](https://www.linkedin.com/in/fchollet) 