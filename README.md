# SecuRL
SecuRL – AI-Powered Cyber Threat Detection for 6G Networks SecuRL is a Reinforcement Learning-based cybersecurity framework that detects and mitigates threats in real time using Deep Q-Networks, a Cyber Knowledge Graph (CKG), and NASim. It adapts to evolving attacks, integrates real-time threat intelligence, and enables LLM-powered threat analysis.

Key Components & Methodology
Cyber Knowledge Graph (CKG) for Threat Intelligence
Why?
Traditional security systems rely on static rules, which are ineffective against rapidly evolving cyber threats. A dynamic knowledge graph enhances the model’s ability to understand and analyze vulnerabilities in real time.

What?
A Neo4j-powered Cyber Knowledge Graph (CKG) was built using data extracted from security databases, threat reports, and exploit sources. The graph maps relationships between attack vectors, vulnerabilities, and network components to provide structured threat intelligence.

How?

Data was collected using web scraping techniques (BeautifulSoup), structured using Graphker, and stored in Neo4j.
Queries are executed using Cypher, enabling real-time threat intelligence retrieval for the RL model.
Reinforcement Learning for Threat Detection (DQN Model)
Why?
Traditional threat detection methods rely on predefined rules and signature-based approaches, which are ineffective against zero-day attacks. Reinforcement Learning enables adaptive threat detection by continuously learning from attack scenarios.

What?
A Deep Q-Network (DQN) model was implemented to learn from network attack patterns and improve its detection capabilities over time. The model interacts with a simulated network environment and updates its knowledge dynamically.

How?

The model was trained using NASim (Network Attack Simulator) to recognize and respond to different types of cyber threats.
It interacts with the simulated environment, learns attack strategies, and updates its Q-values based on attack success or failure.
A reward-based learning mechanism optimizes the model’s ability to detect and mitigate threats effectively.
Integration of Large Language Models (LLM) for Automated Threat Querying
Why?
Security analysts require an intuitive method to interact with large-scale cybersecurity data and extract relevant threat intelligence efficiently.

What?
A Large Language Model (LLM)-powered interface was developed to allow users to query threat intelligence using natural language.

How?

User queries are converted into Cypher queries using LLMs (Groq & Gemini).
A Streamlit-based user interface was developed to facilitate seamless interaction with the Cyber Knowledge Graph.
The system enables security professionals to retrieve insights from large-scale threat data without requiring expertise in graph databases.

**Innovation & Impact**
The RL model continuously improves by learning from simulated attack scenarios.
Designed to operate in high-speed 6G networks without performance bottlenecks.
Moves beyond traditional signature-based detection by dynamically analyzing network behavior.
Security professionals can extract insights using an LLM-driven threat analysis system.
Achievements
**Secured first place** at the Software and System Security Bootcamp hosted by NITK Surathkal, in collaboration with Honeywell experts.
Recognized for developing a novel Reinforcement Learning-based cybersecurity framework tailored for next-generation networks.

**Future Enhancements**
Deploying the model in real-world network environments for further evaluation.
Enhancing adversarial training to improve robustness against evasive cyber attacks.
Optimizing the LLM-based querying system for faster and more precise threat analysis.
SecuRL represents a significant advancement in AI-driven cybersecurity, paving the way for self-learning threat detection systems in next-generation networks.
