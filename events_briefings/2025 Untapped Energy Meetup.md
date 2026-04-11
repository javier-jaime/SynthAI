# 2025 Untapped Energy Presentations

| Presentation Title | Presenter | Organization | Tech Topic | Key Tools or Technologies | Primary Use Case | Performance or Accuracy Metrics |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| Geospatial Data and GeoAI: The Coolest Data You Use | [Alonzo de la Cruz](https://ca.linkedin.com/in/geomatics1) | Suncor Energy | GeoAI / Geomatics | SQL, Python, Google Earth Engine, Picterra, ResNet-50 (CNN), Random Forest, Sentinel-2 | Mapping well pad footprints and dynamic wetlands (Prairie Potholes) for conservation. | 95% accuracy for Upland; 70% for Wetland; 83% success in well pad detection; 99% confidence. |
| AI-Ready or Just AI-Hopeful? | [Noel Thomas](https://ca.linkedin.com/in/noelfranthomas), [Eugene Paulia](https://ca.linkedin.com/in/eugene-paulia), [Sam Moses](https://ca.linkedin.com/in/samnmoses) | Grouplabs / Suncor / Cenovus | Data Quality / Data Governance | Norma, Python, Jupyter Notebook, Scikit-learn, KNN Imputer, Ridge Regression, Claude 3.7 | Improving model accuracy through data normalization and imputation; tracking occupancy/incidents. | 27% reduction in RMSE after pre-processing; 70% of AI projects fail due to data quality issues. |
| Stop Playing with AI \- Starting Planning For AI | [Tim Chan](https://ca.linkedin.com/in/timwhchan) | Untapped Energy | Agentic AI / AI Literacy | LLMs, SAP (ERP), Salesforce (CRM), Workday, GPU-bearing digital agents | Strategic business planning and upskilling employees from basic assistants to autonomous agents. | 10x to 100x productivity gain using advanced agents (vs 1-3x for basic assistants). |
| Dear Diary: Sensor Drama, Hourly | [Shayne Chidlaw](https://ca.linkedin.com/in/shayne-chidlaw-3a609211) | Chirality Research | Data Historians / Time Series Data | SCADA, PLC, SQL, Canary (Historian), Axiom (Visualization), Machine Learning | Converting disorganized well site sensor data into structured records for root cause analysis. | Standardized millions of inconsistent tags into a functional 7-parameter asset hierarchy. |
| Search Less, Land More \- The Smart AI Way to Job Hunt | [Sandra Rogoza](https://ca.linkedin.com/in/sandrarogoza) | LootzySoft | Job Search Strategies / Prompt Engineering | Python, PowerShell, Microsoft Copilot, ChatGPT, Data science chunking | Helping career transitioners navigate the Canadian job market by identifying titles and positions. | Zero hallucinations (reported via specific prompting techniques). |
| Scaling Large Language Models: Unlocking Enterprise Potential | [Farid Talebloo](https://ca.linkedin.com/in/ftalebloo) | Avenue Living | LLM Scaling / MLOps | AWS Secret Manager, Docker, LangChain, Streamlit, AWS ECS, AWS ECR, Fargate | Summarization, contract analysis, and fraud detection using scalable cloud architectures. | Not in source |
| Look Over Your Shoulders: What Students are Learning About AI | [Tim Chan](https://ca.linkedin.com/in/timwhchan) | University of Calgary / Mount Royal University | Generative AI Education / Vibe Coding | Perplexity, Elicit, Low-code/No-code tools | Academic research, data analysis, and developing applications via human-AI loops. | Not in source |
| How I Use Agentic AI To Get My Work Done | [Mark Perrin](https://ca.linkedin.com/in/msperrin) | TriAcc Group | Agentic AI / Scripting | Microsoft Copilot, ChatGPT, PowerShell, Visual Studio, Python, Blender, DAX, Power Query M, Rust | Automating administrative tasks (e.g., auditing 63 Microsoft Teams environments) and code generation. | Not in source |
| Will Your Boss Accept Your AI-Derived Recommendations? | [Yogi Schulz](https://ca.linkedin.com/in/yogischulz) | Corvelle Consulting | AI/ML Project Management | AI/ML models, Amazon, high volume/variety data | Communicating technical recommendations to senior management by focusing on business value. | Not in source |

Note: Where is Hossein Video?

# February 2025

# **AI Agents and Geospatial Intelligence in Technical Workflows**

## **Executive Summary**

The provided documents detail the increasing integration of artificial intelligence into technical work environments, specifically focusing on the use of agentic AI for programming and analytical GeoAI for geospatial data processing. A primary challenge addressed is the overwhelming volume of documentation and syntax associated with modern scripting languages, such as Python and PowerShell, where AI tools like **Microsoft** Copilot facilitate rapid problem-solving and automation. In the geospatial sector, the focus is on Analytical AI, which is used to extract insights from diverse data sources including satellite imagery, drone data, and point clouds. Key projects demonstrate that GeoAI can automate labor intensive tasks, such as identifying wellpad footprints or monitoring dynamic wetlands, leading to significant cost savings and improved accuracy. The effectiveness of these tools is fundamentally dependent on the quality and resolution of the source data, as AI cannot identify features not present in the original imagery.

## **AI Agents for Programming and Administrative Automation**

The use of AI agents serves as a critical support mechanism for professionals managing multiple programming and scripting languages. This is particularly relevant for individuals handling a wide variety of tools where remembering specific syntax is a significant challenge.

### **Documentation and Syntax Challenges**

Modern programming environments require familiarity with extensive documentation, which is often too vast for individual mastery.

* Python documentation consists of approximately 6,500 pages.  
* Blender documentation exceeds 4,000 pages.  
* PowerShell and Power Query M each have around 1,400 pages of documentation.  
* DAX documentation is roughly 1,100 pages.  
* Rust documentation is approximately 1,000 pages.

### **Practical Application: PowerShell and Microsoft Teams**

In a specific administrative scenario, AI was utilized to manage 63 **Microsoft** Teams environments. The task required identifying owners across all teams, many of which were not accessible via the standard user interface.

* **Initial Scripting:** **Microsoft** Copilot was used to generate an initial PowerShell script to list team owners.  
* **Iterative Problem-Solving:** When the script failed due to multi-factor authentication (MFA) requirements, the AI provided solutions for integrating the get credential function.  
* **Outcome:** The finalized script successfully gathered the required data and exported it to an Excel workbook, saving significant time compared to manual checking.

## **Fundamentals of Geospatial Data**

Geospatial data is defined as any time-based data related to a specific part of the earth. This data exists in several formats, each serving distinct analytical purposes.

### **Data Formats and Types**

* **Maps:** Digital or paper representations of the earth at a specific point in time.  
* **Tabular Text Data:** Tables containing location-based identifiers used to relate information to physical spots.  
* **Vector Data:** Points (representing buildings or addresses), lines (roads or railroads), and polygons (building footprints or areas).  
* **Raster Data:** Imagery composed of pixels, such as satellite or aerial photos.  
* **3D Models and Point Clouds:** Models composed of millions of points, each with three-dimensional coordinates, to represent physical reality.

### **The Science of Geodesy and Projections**

Accurate geospatial analysis requires an understanding of the earth's shape and how it is represented on flat surfaces.

* **Ellipsoids:** Mathematical models, such as WGS84 or North American Data 1927, account for the earth being an oval that is flatter at the poles and fatter at the equator.  
* **Projections:** These are methods of placing 3D surfaces onto 2D maps. This process inevitably distorts size, shape, or both.  
* **Specific Projections:** Examples include Mercator, Winkle, Lambert (often used for Alberta), and Spillhaus (centered on connected oceans).  
* **The Importance of Accuracy:** "If your data is in the wrong place inevitably your analysis is going to be flawed especially if you're using GeoAI."

## **Technological Evolution of Geospatial Collection**

The history of geospatial data is tied to the launch of Sputnik 1 in 1957, which led to the development of Global Navigation Satellite Systems (GNSS).

### **GNSS and Global Positioning**

The discovery that radio signals from Sputnik could be used to determine locations on earth led to the democratization of global coordinates.

* GPS was developed by the United States.  
* GLONASS was created by Russia.  
* Galileo is the European system.  
* BeiDou was developed by China.

### **Collection Hardware**

Modern geospatial data collection involves mounting sensors on moving vehicles.

* **Lasers:** Active pulses used to collect the precise position of objects, providing high spatial density.  
* **Cameras:** Passive sensors that capture parts of the electromagnetic spectrum.  
* **Platforms:** Satellites provide global coverage, planes offer high-resolution aerial imagery (30 cm pixels), and drones provide highly detailed local data (2 cm pixels).

## **Analytical GeoAI and Machine Learning**

Analytical GeoAI focuses on machine learning and deep learning to extract information from data, rather than generating new content. This is primarily achieved through computer vision.

### **Case Study: Wellpad Identification at Suncor Energy**

**Suncor Energy** utilized GeoAI to determine the true footprint of wellpads in Northeastern Alberta.

* **Platform:** The project used **Picterra**, an external deep learning platform.  
* **Model:** A convolutional neural network known as ResNet-50 was employed.  
* **Training Process:** The model was trained by manually digitizing wellpad outlines in specific training areas. Iterative training was required to teach the model what was not a wellpad to reduce false positives.  
* **Performance:** The model achieved 83% accuracy when checked against independent survey data. Confidence scores provided by the platform allowed for the filtering of results, with those above 95% confidence being highly accurate.

### **Case Study: Wetland Monitoring by ABMI**

The **Alberta Biodiversity Monitoring Institute** (**ABMI**) developed the Alberta Wetlands Index to track dynamic Prairie Pothole wetlands.

* **Tools:** The project utilized open satellite imagery from Sentinel-2 and the **Google** Earth Engine computing platform.  
* **Methodology:** A Random Forest machine learning model was used. This model consists of multiple decision trees (50 in this case), where each tree votes on whether a pixel is flooded or not, and the majority wins.  
* **Results:** The model showed 95% accuracy for uplands and 70% accuracy for wetlands. This was achieved using open data and open computing platforms, demonstrating that high-level GeoAI is accessible without massive corporate investment.

## **Economic and Operational Benefits of GeoAI**

The primary advantage of GeoAI is the reduction of manual tasks, which translates to cost and time savings.

| Benefit | Description |
| :---- | :---- |
| **Quantification** | GeoAI allows for the calculation of total area, extents, and the number of objects within a dataset. |
| **Change Detection** | By using time-series data, organizations can measure how physical features change over months or years. |
| **Pattern Recognition** | Models can identify trends in the data that may not be obvious to manual observers. |
| **Cost Reduction** | Automating the digitization of roads or footprints replaces labor-intensive manual clicking. For example, surveying thousands of wetlands manually would be economically impossible. |

## **Conclusion and Success Factors**

A successful GeoAI project requires a specific goal and data that matches the required resolution of that goal. "If you can't see it in the data the computer's not going to find it." Whether through deep learning platforms like **Picterra** or open-source methods involving **Google** Earth Engine, AI provides the means to understand physical reality more efficiently, aiding in logistics, travel, and environmental conservation.

# March 2025

# **Scaling Large Language Models: Unlocking Enterprise Potential**

## **Executive Summary**

The transition from rule-based Natural Language Processing (NLP) to deep neural network Large Language Models (LLMs) has transformed how enterprises approach automation and customer engagement. While early NLP required strict adherence to linguistic rules, LLMs mimic human communication through extensive training on diverse datasets. To unlock enterprise potential, organizations must move beyond simple chatbot integration toward hybrid models capable of human, like decision making. Successful deployment hinges on effective scaling, which involves balancing vertical and horizontal infrastructure growth while managing costs. Security remains a primary concern, necessitating the use of cloud based secret managers and containerized environments to protect sensitive data and ensure consistent performance. As these technologies evolve, the future of LLMs lies in multimodal capabilities that incorporate images, video, and sensory data.

## **The Evolution and Utility of Large Language Models**

The field of AI has moved from a literacy focused approach where developers functioned like teachers of grammar to a model based on deep neural networks. In previous iterations of NLP, systems relied on identifying parts of speech such as verbs, subjects, and adverbs to function. Modern LLMs, pioneered by models like GPT-1 and GPT-2, learn to act and talk like humans through training on massive datasets.

Enterprises currently leverage these models for several high, value applications:

* **Customer Support:** Providing 24/7 availability for customer care and maintaining records of interactions.  
* **Document Processing:** Utilizing auto, summarization, contract analysis, and legal insights to manage large volumes of text.  
* **Knowledge Management:** Enhancing search capabilities and organizing organizational knowledge by ingesting and documenting internal data.  
* **Industry, Specific Insights:** Applying models to fraud detection in finance, patient insights in healthcare, and personalized shopping in retail.

## **Scaling Strategies for Enterprise Applications**

Scaling is critical to maintaining customer satisfaction, as failing to provide available resources for high request volumes can result in lost business. Scaling requires a proactive decision between vertical and horizontal approaches.

| Scaling Type | Characteristics | Use Cases |
| :---- | :---- | :---- |
| **Vertical Scaling** | Adding more processors or memory to a single service or instance. | High, performance computing and databases. |
| **Horizontal Scaling** | Adding more individual systems or instances to distribute the workload. | AI inference and web applications. |

Horizontal scaling is generally preferred for enterprise AI because it improves fault tolerance, if one service fails, others continue to run. **AWS** provides tools such as Auto Scaling groups and load balancers to manage these distributed workloads. A hybrid version combining both methods is also an option for specific infrastructure needs.

## **Technical Architecture and Infrastructure**

A robust LLM application requires a fully packed design package to ensure reliability and security. The suggested technical stack, primarily utilizing **AWS** services, involves several integrated layers.

### **Security and Secret Management**

Hardcoding credentials or API keys directly into application code is a significant security risk. Enterprises should use a cloud, based secret manager, such as **AWS** Secrets Manager, **Microsoft** Azure Key Vault, or **Google** Secret Manager.

* **Automated Rotation:** Cloud services can automatically change credentials to maintain environment security.  
* **Access Control:** Permissions and auditing can be managed centrally without modifying the application code.  
* **Integration:** API keys for platforms like **OpenAI** are stored as encrypted values and retrieved by the application at runtime.

### **Containerization and Orchestration**

Using **Docker** allows LLMs to run consistently across different environments by isolating dependencies and preventing library conflicts.

* **Portability:** Containers are lightweight and can be expanded or versioned easily.  
* **Repository:** The **AWS** Elastic Container Registry (ECR) serves as a centralized, secure storage for container images.  
* **Service:** The **AWS** Elastic Container Service (ECS) manages the deployment of these containers. Using a serverless launch type like Fargate can reduce costs for systems that do not require constant uptime.

### **Model Orchestration and Interface**

To simplify the connection between the application and various models, developers use orchestrators like **LangChain**. This tool manages the complexities of connecting to models from **OpenAI** or **Hugging Face**. For the user interface, libraries like Streamlit allow for the rapid creation of web applications with minimal coding requirements, enabling features like text areas for summarization and progress indicators.

## **Risks, Guardrails, and Ethical Considerations**

Despite their capabilities, LLMs are not a complete human brain and lack true reasoning. They are prone to several risks that require enterprise, grade guardrails:

* **Hallucination:** LLM can simulate a fact and then rely on that fact and answer you back.  
* **Bias:** Models trained exclusively on specialized data, such as finance only datasets, may lack general knowledge and produce biased results.  
* **Privacy Violations:** Employees may inadvertently send sensitive organizational data to cloud, based LLMs, creating legal and security headaches.  
* **Jailbreaking:** Users may attempt to bypass model restrictions to force the AI to generate non, factual or inappropriate content.

## **Future Projections in AI Development**

The trajectory of LLM development suggests a shift toward multimodal systems. Future models will likely process more than just text, incorporating images, video, frequencies, and even sensory data like touch or taste.

Key future trends include:

* **Multimodal Integration:** Capabilities similar to GPT, 4o that allow users to upload images and ask questions about the visual content.  
* **On, Device Efficiency:** The development of smaller, more efficient models that can reside locally on user devices.  
* **Democratization:** Increasing global access to AI services, particularly for populations currently facing technological bans or lack of infrastructure.

# April 2025

# **Strategic AI Implementation: From Career Transition to Corporate Recommendation**

## **Executive Summary**

The provided documents examine two primary applications of Artificial Intelligence: streamlining the job search process through structured prompting and successfully presenting technical machine learning projects to corporate leadership. A specialized methodology known as data science chunking is utilized to eliminate AI hallucinations and identify hidden employment opportunities by expanding job title searches. In the corporate sphere, success is defined not by technical sophistication but by the ability to align AI initiatives with business value and corporate strategy. Data scientists are advised to avoid technical jargon, focusing instead on financial outcomes and the defensibility of their models across ten specific topic areas, including data quality, algorithm adequacy, and responsible AI practices.

## **AI-Driven Job Search Methodology**

The documents outline a highly effective strategy for navigating the Canadian employment landscape, particularly for newcomers or individuals in career transition. This approach leverages AI to move beyond traditional search methods and uncover companies that often fly under the radar of the general public.

### **The Data Science Chunking Technique**

To maintain absolute accuracy and prevent errors, a technique based on data science chunking is recommended. This method involves providing the AI model with focused, sequential pieces of information rather than overloading it in a single prompt.

* **Prevention of Hallucinations:** Overloading an AI with too much data causes the model to become scattered, leading to errors.  
* **Sequential Memory:** By feeding specific information in a sequence, the AI takes the data into memory more effectively.  
* **Persona Designation:** The process begins by assigning the AI specific professional personas, such as an expert in research, a human resources business partner, or a consultant with a grand level of expertise.

"I only give the AI model very focused pieces of information in a sequence because think of it this way: ‘Let's say you have a book that is a thousand pages in length I tell you to read that book in one minute and then give me a synopsis of what everything that you've learned in that book’. That is similar to when you overload the AI in one chat with too much information. It doesn't know where to look. It starts to become scattered and then that's when you have hallucinations or errors."

### **Broadening Career Horizons through Title Exploration**

A critical component of the AI-enhanced job search is identifying creative variations of job titles. Human resources departments often use diverse terminology for similar roles, which can limit the results of a standard search.

* **Title Variation:** For a candidate seeking a machine learning engineer role, the AI can identify equivalent positions such as AI developer, applied machine engineer, data scientist, machine learning scientist, or deep learning engineer.  
* **Local Market Insights:** Using these expanded titles allows candidates to find openings in specific locations like Calgary across various industries and work formats, including in-office, hybrid, or remote.  
* **Identification of Hidden Employers:** This method reveals numerous valid companies beyond traditional large entities like **Telus**, **ATB**, or major banks.

**Tool Accessibility and Platform Comparisons**

The analysis indicates that while paid accounts offer features like deep research, they are not strictly necessary for an effective job search. Free AI accounts return similar, high-quality results for identifying similar job titles and open positions at companies like **Clio** or **AltaML**.

## **Presenting AI/ML Projects to Senior Leadership**

A significant challenge for data scientists is the final stage of project delivery, where recommendations must be sold to management. Failure often occurs because technical experts focus on their technical prowess rather than business resonance.

### **The Managerial Communication Gap**

Senior executives often view Artificial Intelligence and Machine Learning as topics outside their domain. Presenting overly technical details or advanced algorithms can scare leadership and erode their confidence in the project. The audience often includes:

* Individuals openly uncomfortable with the technical topic.  
* Quiet, introspective, and hard-to-read stakeholders.  
* Openly skeptical or problematic characters.

To succeed, presenters must ignore technical pride and focus on business value, money, and follow-on project funding.

"Too often what I observe is that data scientists do just a brilliant job in working on the project and then they crash and burn on the goal line because they're not selling their recommendations in a way that management can understand them And my goal today is to help you understand how to present the great work that you've done in your AI/ML project in a way that will resonate with management and in a way that will get your recommendations accepted and funded and acted upon."

### **Evaluating Project Defensibility: The Ten Pillars**

To ensure recommendations are accepted, the project team must address ten critical topic areas that management is likely to raise.

1. **Accuracy of Business Opportunity:** Ensuring the project attacks a real business problem rather than just a symptom.  
2. **Data Sufficiency:** Evaluating the volume and variety of data, particularly the historical time periods used.  
3. **Data Quality:** Assessing the accuracy (lack of invalid values) and completeness (lack of nulls or missing rows) of the data.  
4. **Algorithm Adequacy:** Defending the choice of specific machine learning algorithms over others.  
5. **Model Adequacy:** Ensuring the model correctly targets the intended business situation without subtle deviations.  
6. **Congruity:** Verifying that the data and the model fit together properly to avoid dangerous or legally risky results.  
7. **Advancement of Corporate Strategy:** Confirming the project aligns with the broader business goals or pressing issues of the organization.  
8. **Understanding Data Elements:** Managing the risk of similar or cryptic column names in different data sources.  
9. **Team Competency:** Being candid about the team's expertise and the strategy for acquiring missing skills, such as using consultants or mentoring staff.  
10. **Responsible AI and Explainability:** Addressing ethics, fairness, bias, and privacy while ensuring end users can comprehend and trust the results.

"The algorithms are available to build AI/ML models vary widely in scope complexity and indeed quality So the confidence you can have in your recommendation is dependent on the adequacy of these algorithms."

## **Handling Executive Inquiries**

The manner in which a team responds to questions from senior leadership determines the ultimate acceptance of the project.

### **Responses that Erode Confidence**

* **Blank Stairs:** Failing to address a topic indicates the issue was not considered during planning.  
* **Technical Jargon:** Providing lengthy, jargon-filled answers suggests a lack of critical communication skills.  
* **Generalized Comparisons:** Claiming an approach is the same as another well-known organization fails to account for unique business contexts.

### **Responses that Build Confidence**

* **Thoughtful Planning:** Providing answers based on the ten pillars of project defensibility.  
* **Transparency Regarding Risk:** Being upfront about uncertainties, unanticipated consequences, or potential business implications.  
* **Back Pocket Slides:** Having supplemental material ready to answer specific, anticipated questions.  
* **Defining Scope:** Reminding leadership of the project's limitations and what it was not designed to solve, which prevents over-excitement or scope creep.

"Responding accurately and confidently to the questions for the topics I've presented will cause your boss to accept your recommendations. And the bottom line is that's how we achieve success as an AI/ML project team."

# May 2025

# June 2025

# **From AI Experimentation to Strategic Implementation**

## **Executive Summary**

Current industry trends reveal a significant divide between organizations that play with Artificial Intelligence and those that plan for it. While basic generative AI use (e.g., writing cover letters or enhancing photos) offers modest productivity gains of 1x to 3x, the transition to Agentic AI, where autonomous agents handle complex, multi-step deliverables, promises transformative productivity increases of 10x to 100x.

However, the path to these gains is fraught with high failure rates. Approximately 85% of corporate AI projects fail, with 70% of those failures attributed to poor data quality and integration issues. This briefing outlines the critical need for internal AI literacy, the foundational role of data governance, and the technical necessity of robust data pre-processing to ensure AI systems achieve their strategic objectives.

\--------------------------------------------------------------------------------

## **1\. The Strategic Shift: Playing vs. Planning for AI**

The current landscape is dominated by AI hopeful users who utilize tools for minor tasks. True organizational AI readiness requires moving beyond superficial applications toward a strategic, agentic framework.

### **The Productivity Spectrum**

The impact of AI is categorized by the level of autonomy and complexity involved:

* **Assistants and Co-pilots:** Used for chatbots, search, and text generation. These tools provide a 1x to 3x productivity boost.  
* **Agentic AI:** Advanced tools capable of sophisticated research, reasoning, and coding. These agents work autonomously for extended periods (15 minutes or longer) and can provide a 10x to 100x productivity boost.

### **The Risk of Vendor Dependency**

Many organizations believe they have integrated AI because their existing SaaS providers (**SAP**, **Salesforce**, **Workday**) have added automated or predictive features. This approach carries significant risks:

* **Lack of Upskilling:** It does not meaningfully improve the AI literacy of the company’s employees.  
* **Vendor Lock-in:** It makes organizations entirely dependent on external vendors for their AI capabilities.  
* **Strategic Stagnation:** Companies fail to develop the internal skills necessary to win in their specific market.

### **The Future of the Workforce**

Regardless of job titles, the next generation of employees will essentially be in coding roles. This does not imply constant keyboard work, but rather the ability to:

* Understand how AI tools function to troubleshoot undesired outcomes.  
* Discern which AI startups and products are viable and which will fail.  
* Lead hybrid teams consisting of "flesh-bearing employees" and "GPU-bearing digital agents."

\--------------------------------------------------------------------------------

## **2\. Data Quality: The Cornerstone of AI Success**

AI systems are only as effective as the data they ingest. Global data indicates that 5% of annual revenue is lost due to poor data quality in AI systems.

### **The Components of Bad Data**

Errors in AI outcomes typically stem from three real-world problems:

1. **Bias:** Flawed sampling methods.  
2. **Variance:** High variance caused by insufficient data volume.  
3. **Noise:** Inaccuracies resulting from limitations in measurement devices.

### **Challenges for Human-Only Management**

Humans can no longer manage data quality effectively due to:

* **Volume:** Petabytes of data cause manual processes to time out.  
* **Variety:** Rapidly changing schemas and data types break traditional pipelines.  
* **Drift:** Data quality tends to degrade over time, requiring constant monitoring.

\--------------------------------------------------------------------------------

## **3\. Case Studies: The Impact of Data Preparation**

The difference between AI failure and success is often found in the initial investment in data cleaning and standardization.

| Organization | Investment/Scope | Outcome | Root Cause |
| :---- | :---- | :---- | :---- |
| **IBM Watson (Oncology)** | $4 Billion | Project shut down after recommending harmful treatments. | Trained on textbook perfect data, failed when exposed to messy, real-world hospital data. |
| **Global Food Manufacturer** | $20 Billion | Supply chain optimization failed within one year. | Less than 10% of the budget spent on cleaning, overlooked seasonal spikes and outliers. |
| **HCA Healthcare** | 185 Hospitals | Saved 8,000+ lives, 18-hour lead time on sepsis detection. | Standardized 700+ different names for the same lab test (lactic acid) using domain experts. |

### **Key Insight: The Black Box Problem**

A significant factor in the **IBM** Watson failure was the black box nature of its algorithm. Doctors were given treatment recommendations without the reasoning behind them, leading to a lack of trust and rapid abandonment of the tool.

\--------------------------------------------------------------------------------

## **4\. Technical Efficacy: The Norma Case Study**

A technical demonstration comparing a baseline regression model to one with basic pre-processing revealed a 27% improvement in model performance.

### **Pre-processing Techniques and Results**

The demonstration utilized the **Zillow** housing market dataset (25,000 rows, 20 features) to predict sales prices.

| Step | Action Taken | Impact |
| :---- | :---- | :---- |
| **Handling Nulls** | Used K-Nearest Neighbors (KNN) imputer to fill gaps based on similar data clusters. | Prevented data loss from dropping rows and avoided bias from zero values. |
| **Anomaly Removal** | Dropped extreme outliers (e.g., apartments with 15+ rooms or build years before 1200). | Improved model stability and normality of residuals. |
| **Feature Engineering** | Created new ratios: Living Efficiency, Average Room Size, and Amenity Score. | Provided the model with higher-context indicators of value. |
| **Scaling & Encoding** | Applied Standard Scaler and One-Hot Encoding for categorical data. | Ensured numerical consistency across features. |

**The Result:** The error score (RMSE) dropped by 27%, representing hundreds of thousands of dollars in improved prediction accuracy for a single model.

\--------------------------------------------------------------------------------

## **5\. Emerging Solutions: AI-Powered Data Governance**

New tools, such as the Norma product, are leveraging AI to automate the data cleaning process that previously took data scientists hours or days to complete manually.

### **Core Features of AI-Ready Data Tools**

* **Automated Cataloging:** AI fills out column descriptions and identifies data types.  
* **Task-Aware Cleaning:** Adjusting data manipulation based on the end goal (e.g., training a model vs. reporting).  
* **SQL Generation:** Using Large Language Models (LLMs) like **Anthropic**’s Claude to translate natural language into complex SQL queries, enabling non-technical users to analyze data objectively.  
* **Change Tracking:** Implementation of versioning/revisions to prevent data loss and allow for the reversal of AI-driven errors.  
* **Anonymization:** Ensuring data privacy by scrubbing sensitive information before it is sent to external LLMs for processing.

### **Conclusion**

To move from AI hopeful to AI ready, organizations must prioritize data literacy and strategic planning. The goal is to build an "AI Strategic Roadmap" and an "AI Competency Maturity Inventory," ensuring the foundation of the company's data is clean, standardized, and ready to support the 100x productivity gains promised by the age of Agentic AI.