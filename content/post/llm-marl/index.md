---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "LLMs for Multi-Agent Cooperation"
subtitle: ""
summary: ""
authors: []
tags: []
categories: ["LLM"]
date: 2025-05-23T13:46:11-05:00
lastmod: 2025-05-23T13:46:11-05:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  placement: 2
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---
<!-- # Large Language Models for Multi-Agent Cooperation: A Comprehensive Survey -->

The emergence of Large Language Models (LLMs) has catalyzed a paradigm shift in artificial intelligence, particularly in how we approach complex problem-solving through multi-agent systems. As we stand in May 2025, the field of LLM-based multi-agent cooperation has evolved from theoretical curiosity to practical reality, with implementations spanning software development, financial trading, robotics, and enterprise operations. This comprehensive survey examines the current state of this rapidly evolving field, synthesizing recent research, frameworks, and real-world applications.

## 1. Introduction to multi-agent cooperation with LLMs

LLM-based multi-agent systems represent a fundamental evolution in artificial intelligence, where multiple AI agents powered by large language models collaborate to solve complex tasks that exceed the capabilities of individual agents. Unlike traditional multi-agent systems that rely on predefined protocols and rigid communication structures, LLM-based systems leverage natural language as a universal medium for coordination, enabling unprecedented flexibility and emergent behaviors (Tran et al., 2025; Zhou et al., 2024).

The core innovation lies in transforming language models from passive text generators into **active, autonomous agents** capable of perception, reasoning, planning, and collaborative action. These agents can assume specialized roles, share knowledge dynamically, and adapt their strategies based on interaction outcomes (Guo et al., 2024). The field has experienced explosive growth, with research publications increasing exponentially each quarter since 2023, driven by the promise of solving complex real-world problems through collective AI intelligence.

What makes LLM-based multi-agent cooperation particularly compelling is its ability to mirror human collaborative patterns while potentially surpassing human limitations in scale, consistency, and processing speed. From virtual software companies where AI agents fulfill roles from CEO to programmer, to financial trading teams that combine fundamental and technical analysis, these systems are demonstrating new possibilities for automated problem-solving (Tran et al., 2025; SuperAnnotate, 2024).

## 2. Key concepts and terminology

### Core definitions shaping the field

**LLM-based Multi-Agent System (LLM-MAS)** refers to a computational system comprising multiple intelligent agents powered by large language models that can perceive, learn, reason, and act collaboratively to solve complex tasks collectively at scale (SuperAnnotate, 2024). This definition encompasses five essential components that characterize these systems: profile (how agents are created with personalized characteristics), perception (environmental information acquisition), self-action (memory, reasoning, and planning capabilities), mutual interaction (inter-agent communication), and evolution (self-reflection and progressive enhancement) (Zhou et al., 2024; Tran et al., 2025).

**Agentic AI** represents the application of LLMs as autonomous agents capable of goal-oriented behavior in dynamic environments. This concept moves beyond simple text generation to encompass planning, reasoning, and action-taking capabilities. The transition from "virtual assistants" to "virtual collaborators" marks a fundamental shift in how we conceptualize AI systems.

**Collaboration channels** serve as critical pathways enabling agents to work together, facilitating planning and coordination capabilities. These channels exhibit advanced behaviors including Theory of Mind reasoning, where agents develop models of other agents' beliefs, goals, and intentions (SuperAnnotate, 2024). The sophistication of these channels determines the system's ability to tackle complex, multi-faceted problems.

**Orchestration platforms** provide the core infrastructure managing interactions and information flow among agents. These platforms handle coordination, communication, planning, and learning across the multi-agent ecosystem, serving as the nervous system that enables collective intelligence to emerge from individual agent capabilities.

### Communication and coordination mechanisms

Multi-agent collaboration mechanisms are characterized across five key dimensions. **Actors** define the specific agents involved in collaboration, ranging from homogeneous teams to diverse, specialized groups. **Types** encompass cooperation (shared goals), competition (opposing objectives), and coopetition (mixed dynamics). **Structures** include peer-to-peer (decentralized), centralized (supervisor-based), and distributed architectures. **Strategies** range from role-based (specialized expertise) to model-based (AI-driven coordination) approaches. **Coordination protocols** specify the communication mechanisms and interaction patterns (Tran et al., 2025).

The field distinguishes between several communication paradigms. **Memory-based** communication involves shared knowledge repositories accessible to all agents. **Report-based** systems use status updates and progress communication. **Relay** mechanisms enable information passing between agents in sequential workflows. **Debate** protocols facilitate argumentative exchanges for consensus building (Zhou et al., 2024). These paradigms can be implemented across various network topologies including bus, star, ring, and tree configurations, each optimized for different coordination requirements.

## 3. Main approaches and methodologies for LLM-based multi-agent cooperation

### Architectural paradigms defining the field

The field has converged on several dominant architectural patterns. **Centralized coordination** employs a supervisor agent that manages and directs specialized worker agents, exemplified by AutoGen's supervisor architecture and LangGraph's supervisor tool-calling pattern (Analytics Vidhya, 2024). This approach provides clear control and coordination but can create bottlenecks. **Decentralized systems** enable peer-to-peer communication without central authority, as seen in CAMEL's role-playing framework, offering greater resilience but increased coordination complexity. **Hierarchical architectures** implement multi-level supervision where supervisors manage other supervisors, supported by frameworks like LangGraph's hierarchical teams and MegaAgent's system-level parallelism.

Structural approaches vary based on use case requirements. **Network architectures** allow every agent to communicate with every other agent, maximizing information flow but potentially creating communication overhead. **Assembly line structures** implement sequential processing where agents work in predefined stages, epitomized by MetaGPT's software development pipeline. **Role-based teams** assign agents specific professional roles with associated capabilities and responsibilities, as implemented in CrewAI and MetaGPT. **Graph-based workflows** treat agents as nodes in directed graphs with edge-controlled communication, providing maximum flexibility for complex processes (Tran et al., 2025).

### Theoretical frameworks guiding development

The **Extended Coevolutionary (EC) Theory** provides a dynamic framework incorporating coevolutionary dynamics where agents evolve strategies based on interactions, adaptive learning from environmental feedback, and LLM-based strategy recommendations. This framework accounts for heterogeneous agent modeling with diverse capabilities, risk preferences, and learning styles, moving beyond static game theory models (Giannakis et al., 2023).

The **CAMEL framework** (Communicative Agents for Mind Exploration) introduces a foundational approach using role-playing methodology. Agents assume specific roles through inception prompting, facilitating autonomous cooperation and task completion. This framework has proven particularly valuable for studying collaborative behaviors and generating conversational data for analysis while addressing common challenges like role flipping and conversation termination (Li et al., 2023).

The **Multi-LLM-Agent System (MLAS)** framework addresses the evolution from single-agent to multi-agent systems, highlighting advantages including higher task-solving performance potential, greater system flexibility, proprietary data preservation for participating entities, and feasibility of monetization. The framework implements layered protocol architectures for diverse agent interactions with dynamic protocol selection based on task requirements (Zhang et al., 2024).

## 4. Current state-of-the-art techniques and frameworks

### Leading frameworks shaping the ecosystem

**Microsoft AutoGen** stands as a conversational multi-agent framework built on an actor model with asynchronous messaging. Its AutoGen Core provides low-level control while AutoGen AgentChat offers high-level APIs for rapid prototyping. Key features include Docker-based code execution for security, flexible conversation patterns, human-in-the-loop support, and enhanced LLM inference with caching (Wu et al., 2023). AutoGen excels in research and code generation scenarios but requires significant coding expertise for production deployment.

**MetaGPT** revolutionizes software development automation through its assembly line paradigm. Following the philosophy "Code = SOP(Team)", it materializes standard operating procedures into LLM teams with specialized roles including Product Manager, Architect, Project Manager, Engineer, and QA Engineer. The framework's innovation lies in structured communication interfaces, publish-subscribe message filtering, and executable feedback for code generation, enabling one-line requirements to generate complete software projects (Hong et al., 2023).

**LangGraph** provides graph-based state machines where agents function as nodes and edges control flow. This event-driven system supports flexible state management with user-defined schemas, cycles for iterative processes, built-in checkpointing, and command-based dynamic control flow (LangChain, 2024). LangGraph excels when fine-grained execution control and complex workflow visualization are paramount, though it presents a steeper learning curve.

**CrewAI** focuses on role-based design with agents possessing specific roles, goals, and skills. Built on LangChain's ecosystem, it offers hierarchical team structures, process-driven collaboration, and business-focused automation with low-code visual tools through CrewAI Studio. The framework has achieved significant commercial success with adoption by Oracle, Deloitte, and Accenture, demonstrating 5.76x faster execution than LangGraph in certain tasks (Moura, 2024).

### Advanced coordination techniques

Modern systems implement sophisticated memory synchronization mechanisms. **A-Mem (Agentic Memory)** provides dynamic memory structuring inspired by the Zettelkasten method (Zhang et al., 2025). **Hierarchical memory** systems implement multi-level storage with short-term, long-term, and external knowledge components (LangChain, 2024). **Memory sharing** enables real-time storage and retrieval across agent networks, crucial for maintaining consistency in distributed systems (Liu et al., 2024).

Planning and task decomposition have evolved beyond simple sequential processing. **Chain of Thought (CoT)** enables sequential reasoning steps, while **Tree of Thoughts (ToT)** allows multi-path reasoning exploration. **Graph of Thought** implements graph-structured reasoning for robust decision-making, and **RAP (Reasoning via Planning)** uses world model simulation for plan evaluation before execution (Guo et al., 2024).

Communication optimization techniques include **attentional communication** where agents learn when communication is necessary, **message filtering** using subscription-based relevance determination, and structured **communication protocols** with built-in error handling and recovery mechanisms (SmythOS, 2024; LangChain, 2024).

## 5. Applications and use cases

### Software development automation

**ChatDev** represents a complete virtual software company with specialized AI agents fulfilling roles from CEO to Art Designer. Following a waterfall model through designing, coding, testing, and documenting phases, ChatDev generates software containing 39-359 lines of code (averaging 131.26 lines). The system uses "chat chain" architecture for collaborative task decomposition and "communicative dehallucination" to reduce coding errors (Qian et al., 2023). Multi-agent approaches consistently produce more complete software with fewer errors compared to single-agent systems.

**AgileGen and Think-on-Process (ToP)** advance beyond static workflows to create tailored process instances based on project requirements. Using Gherkin language for testable requirements, these systems bridge the gap between user needs and code implementation, demonstrating the evolution toward more adaptive development processes (Rasheed et al., 2024).

### Financial services transformation

The **TradingAgents** framework mimics real trading firms with specialized agents including fundamental analysts, sentiment analysts, technical analysts, and traders with varying risk profiles. Teams comprise bull and bear researchers, risk management specialists, and fund managers communicating through structured protocols combining reports with natural language dialogue. All decisions include detailed reasoning and tool usage explanations, demonstrating significant improvements in cumulative returns, Sharpe ratio optimization, and maximum drawdown reduction (Li et al., 2024).

**Multi-agent crypto portfolio management** systems employ expert training modules and intrateam/interteam collaboration based on confidence levels. These systems have outperformed single-agent models and market benchmarks in classification, asset pricing, and portfolio performance from November 2023 to September 2024, showcasing the power of specialized agent collaboration in financial markets (Wang et al., 2025).

### Enterprise and business operations

Microsoft's deployment of AutoGen at Novo Nordisk exemplifies enterprise adoption, where the data science department uses the framework to reduce barriers to technical data analytics and enable broader community insights (Microsoft Research, 2023). The "Business-in-a-Box" concept from Azure AI demonstrates comprehensive automation across marketing, HR, procurement, technology, and invoice auditing departments, allowing human workers to focus on specializations while GenAI scales across the organization.

Real-world implementations show measurable benefits. An SEO team case study demonstrated **40% reduction in project time** while maintaining quality through specialist collaboration, with agents handling keyword research, content optimization, and backlink analysis. Document processing systems using LangGraph and CrewAI automate ticket auditing and forwarding through intelligent text analysis and routing.

## 6. Challenges and limitations

### Performance gaps between promise and reality

Recent empirical findings reveal significant challenges in realizing theoretical potential. ChatDev achieves only **33.3% correctness** on programming tasks in the ProgramDev benchmark. AppWorld shows an **86.7% failure rate** on cross-app test cases (UC Berkeley Sky Lab, 2025). Many multi-agent frameworks demonstrate minimal performance gains over single-agent systems, highlighting the gap between architectural sophistication and practical outcomes.

The **MAST (Multi-Agent System Failure) Taxonomy**, developed through analysis of 7 popular frameworks across 200+ tasks, identifies 14 unique failure modes organized into three categories. **Specification issues** include poor task decomposition, inadequate role definition, and unclear objective specification. **Inter-agent misalignment** encompasses communication breakdowns, inconsistent goal understanding, memory management failures, and coordination protocol violations. **Task verification** problems manifest as incorrect output verification (13.48% of observed failures), incomplete verification processes, and insufficient quality control mechanisms (Cemri et al., 2025).

### Technical and operational limitations

**Context limitations** restrict information tracking capabilities, preventing agents from maintaining comprehensive state across extended interactions. **Long-term planning** difficulties emerge when adapting to unexpected problems, as agents struggle with dynamic replanning. **Knowledge drift** leads to amplification and propagation of errors through agent chains. Unlike humans who naturally filter information, LLMs exhibit **cognitive bias expansion**, amplifying errors rather than correcting them (Label Your Data, 2025).

**Scalability challenges** become acute as agent populations grow. LLMs are resource-hungry with astronomical compute requirements, and inference costs balloon with concurrent requests. Systems require sophisticated load-balancing across multiple LLM providers, with caching, quantization, and optimizations becoming essential for viable deployment (Chen et al., 2024).

**Production deployment challenges** include the fundamental trade-off between deterministic behavior and agent autonomy. Organizations lose fine-grained control in autonomous systems while struggling to reason about overall system behavior. Enforcing constraints while maintaining autonomy remains an unsolved challenge, complicated by difficulties in validating outputs and ensuring correctness at scale (ZenML, 2024).

## 7. Recent research papers and developments (2023-2025)

### Groundbreaking surveys and frameworks

**"Multi-Agent Collaboration Mechanisms: A Survey of LLMs"** (Tran et al., 2025) provides the most recent comprehensive survey, introducing an extensible framework characterizing collaboration mechanisms across five dimensions. The work explores applications in 5G/6G networks, Industry 5.0, question answering, and social settings, establishing a new standard for understanding multi-agent collaboration patterns (Tran et al., 2025).

**"Why Do Multi-Agent LLM Systems Fail?"** (Cemri et al., 2025) represents a watershed moment in the field, providing the first empirically grounded failure taxonomy. Through analysis of 7 frameworks across 200+ tasks with expert human annotators, the research achieves a Cohen's Kappa score of 0.88 for inter-annotator agreement and validates an LLM-as-a-Judge pipeline for scalable evaluation. This systematic identification of failure modes provides a clear roadmap for improvement (Cemri et al., 2025).

### Industry protocol standardization

**Google's A2A (Agent-to-Agent) Protocol** establishes an open standard for universal agent interoperability with enterprise-grade authentication and authorization. Supporting long-running tasks and multimodal interactions, A2A is designed for large-scale multi-agent system deployment across organizational boundaries (Google Developers Blog, 2025).

**Anthropic's Model Context Protocol (MCP)** creates a standard for connecting AI assistants to data sources through two-way connections. With OpenAI announcing support and thousands of integrations already available, MCP is rapidly becoming the de facto standard for agent-data interactions, signaling industry convergence on common protocols (Anthropic, 2024; TechCrunch, 2025).

### Emerging evaluation standards

The field has developed sophisticated benchmarks including **SWT-Bench** for test generation, **ProductQA** for question answering evaluation, and extended versions of **GAIA** and **MMLU** for multi-agent scenarios. New metrics assess collaboration through cooperation and coordination rates, trust scores for agent reliability, consensus metrics after multi-round negotiation, and communication efficiency including protocol compliance and temporal synchronization (Dibia, 2024).

## 8. Future directions and open research questions

### Immediate research priorities

**Reliability and robustness** top the research agenda, with focus on addressing the 14 failure modes identified in MAST, developing more robust coordination mechanisms, and improving task verification and quality control. The field requires comprehensive multi-agent evaluation suites, standardized metrics for collaboration assessment, and long-term tracking of system performance to measure progress objectively (Li et al., 2025).

**Scalability solutions** must address performance maintenance as agent count increases, requiring new architectures and optimization techniques. **Emergent behavior** research seeks to understand and control collective intelligence emergence, predicting beneficial behaviors while preventing harmful ones. **Human-AI collaboration** research explores optimal integration of human oversight in multi-agent workflows, balancing automation with human judgment (UC Berkeley Sky Lab, 2025).

### Long-term research horizons

**Interoperability** remains a critical challenge, requiring standardization of communication protocols across different frameworks and organizations. **Security and safety** concerns include addressing vulnerabilities in distributed agent systems, preventing adversarial attacks, and ensuring ethical behavior under all conditions. **Collective intelligence theory** needs development to understand how intelligence emerges from agent interactions and how to foster beneficial emergent behaviors systematically (Chen et al., 2024).

Industry predictions suggest transformative changes ahead. Anthropic CEO Dario Amodei predicts models "gradually get better than us at almost everything" within 2-3 years. OpenAI has committed to building AGI during the current administration (2025-2029) (Axios, 2025). Over 80% of enterprise workloads are expected to use AI-driven systems by 2026 according to Gartner, with multi-agent systems serving as collective intelligence platforms.

## 9. Practical implementation considerations

### Framework selection guidelines

**Choose AutoGen** when fine-grained control and robust error handling are essential, particularly for research applications and scenarios requiring containerized code execution. Its strength lies in conversational patterns and human-in-the-loop capabilities, though it demands significant technical expertise (Datagrom, 2024; Getting Started AI, 2024).

**Choose MetaGPT** for software development automation where structured workflows and role-based collaboration mirror human development teams. Its assembly line approach excels at transforming requirements into complete software projects but remains domain-specific.

**Choose LangGraph** when complex state management and workflow visualization are paramount. Its graph-based approach provides maximum flexibility for intricate processes, though the learning curve is steep and documentation gaps persist (Datagrom, 2024; Relari, 2024).

**Choose CrewAI** for rapid business automation with minimal technical overhead. Its intuitive role-based design and extensive documentation make it ideal for teams seeking quick deployment, though dependency on LangChain may limit flexibility (Datagrom, 2024; Relari, 2024; OyeLabs, 2024).

### Architecture best practices

Successful implementations follow clear design principles. **Role definition** must be explicit with well-defined capabilities and constraints. **Communication patterns** should match task requirements - sequential for simple chains, hierarchical for complex coordination, decentralized for resilience, and hybrid for flexibility. **Error handling** requires circuit breakers, retry mechanisms, and graceful degradation. **Human oversight** remains critical for high-stakes decisions and system monitoring (Chen et al., 2025).

Technical requirements for success include efficient resource allocation, dynamic task control mechanisms, robust inter-agent communication protocols, and comprehensive monitoring systems. Organizations must ensure adequate technical expertise, realistic expectations about capabilities, and proper change management for successful adoption (IntegrAI, 2024; LangChain, 2024).

## 10. Comparison of different approaches

### Architectural trade-offs

**Centralized architectures** offer better coordination and easier debugging but suffer from single points of failure and potential bottlenecks. **Decentralized systems** provide greater resilience and scalability but face coordination complexity and potential inconsistencies. **Hierarchical approaches** balance control and distribution but add complexity in level management (IntegrAI, 2024).

**Communication patterns** present distinct trade-offs. Shared scratchpads enable seamless information access but risk context pollution. Independent contexts maintain clean separation but complicate information sharing. Publish-subscribe systems reduce noise through filtering but may miss relevant information. Direct handoffs provide clear control transfer but limit parallel processing (LangChain, 2024).

### Performance characteristics

Framework performance varies significantly by use case. **AutoGen** excels in iterative problem-solving and code generation but requires substantial setup. **MetaGPT** delivers complete software projects efficiently but lacks flexibility outside development contexts. **LangGraph** handles complex workflows with fine control but demands expertise. **CrewAI** enables rapid deployment with good performance but may hit limitations in complex scenarios (Getting Started AI, 2024; Oxylabs, 2024).

Memory and context management approaches differ substantially. Vector-based retrieval provides semantic search capabilities but requires embedding infrastructure. Hierarchical storage enables sophisticated retention policies but adds complexity. Dynamic filtering improves relevance but may miss edge cases. The choice depends on specific application requirements and resource constraints (Gao et al., 2024; UC Berkeley Sky Lab, 2025).

## Conclusion

Large Language Model-based multi-agent cooperation stands at a critical juncture in 2025. While theoretical foundations are solid and frameworks proliferate, empirical evidence reveals significant gaps between promise and performance. The systematic identification of failure modes through research like MAST provides clear direction for improvement, while emerging protocols like A2A and MCP signal industry maturation.

Success in this field requires careful balance - between autonomy and control, flexibility and structure, innovation and reliability. Organizations must choose frameworks aligned with their specific needs, implement robust architectures with appropriate oversight, and maintain realistic expectations about current capabilities. The rapid pace of development suggests that addressing current limitations will unlock transformative potential across industries.

As we look toward an AI-augmented future, multi-agent systems represent not just a technical evolution but a fundamental shift in how we approach complex problem-solving. The next few years will determine whether these systems achieve their transformative potential or remain primarily academic curiosities. For researchers and practitioners willing to navigate current challenges, the opportunity to shape this future has never been greater.

## References

Analytics Vidhya. (2024). Building a Multi-Agent System with CAMEL AI. Retrieved from https://www.analyticsvidhya.com/blog/2024/12/multi-agent-system-with-camel-ai/

Anthropic. (2024). Model Context Protocol Documentation. Retrieved from https://www.anthropic.com/mcp

Axios. (2025). OpenAI, Anthropic, Google again promise "artificial general intelligence" in "a few years". Retrieved from https://www.axios.com/2025/02/20/ai-agi-timeline-promises-openai-anthropic-deepmind

Cemri, M., et al. (2025). Why Do Multi-Agent LLM Systems Fail? arXiv preprint arXiv:2503.13657.

Chen, L., et al. (2024). LLM Multi-Agent Systems: Challenges and Open Problems. arXiv preprint arXiv:2402.03578.

Chen, Y., et al. (2025). Multi-Agent Design: Optimizing Agents with Better Prompts and Topologies. arXiv preprint arXiv:2502.02533.

Datagrom. (2024). Top 3 Trending Agentic AI Frameworks: LangGraph vs AutoGen vs Crew AI. Retrieved from https://www.datagrom.com/data-science-machine-learning-ai-blog/langgraph-vs-autogen-vs-crewai-comparison-agentic-ai-frameworks

Dibia, V. (2024). Multi-Agent LLM Applications: A Review of Current Research, Tools, and Challenges. Victor Dibia Newsletter.

Gao, Z., et al. (2024). A Survey on the Memory Mechanism of Large Language Model based Agents. arXiv preprint arXiv:2404.13501.

Getting Started AI. (2024). Let's compare AutoGen, crewAI, LangGraph and OpenAI Swarm. Retrieved from https://www.gettingstarted.ai/best-multi-agent-ai-framework/

Giannakis, G., et al. (2023). Emergent Cooperation and Strategy Adaptation in Multi-Agent Systems: An Extended Coevolutionary Theory with LLMs. Electronics, 12(12), 2722.

Google Developers Blog. (2025). Agent Development Kit: Making it easy to build multi-agent applications. Retrieved from https://developers.googleblog.com/en/agent-development-kit-easy-to-build-multi-agent-applications/

Guo, T., et al. (2024). Large Language Model based Multi-Agents: A Survey of Progress and Challenges. arXiv preprint arXiv:2402.01680.

Hong, S., et al. (2023). MetaGPT: Meta Programming for Multi-Agent Collaborative Framework. arXiv preprint arXiv:2308.00352.

IntegrAI. (2024). Multi-Agent AI Coordination. Retrieved from https://integrail.ai/blog/multi-agent-ai-coordination

Label Your Data. (2025). Multi Agent LLM: Key Frameworks & Applications in 2025. Retrieved from https://labelyourdata.com/articles/multi-agent-llm

LangChain. (2024). LangGraph Documentation. Retrieved from https://langchain-ai.github.io/langgraph/

Li, G., et al. (2023). CAMEL: Communicative Agents for "Mind" Exploration of Large Language Model Society. arXiv preprint arXiv:2303.17760.

Li, S., et al. (2024). TradingAgents: Multi-Agents LLM Financial Trading Framework. arXiv preprint arXiv:2412.20138.

Li, Y., et al. (2025). Position: Towards a Responsible LLM-empowered Multi-Agent Systems. arXiv preprint arXiv:2502.01714.

Liu, S., et al. (2024). Memory Sharing for Large Language Model based Agents. arXiv preprint arXiv:2404.09982.

Microsoft Research. (2023). AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation. Retrieved from https://www.microsoft.com/en-us/research/publication/autogen-enabling-next-gen-llm-applications-via-multi-agent-conversation-framework/

Moura, J. (2024). CrewAI Documentation. Retrieved from https://github.com/crewAIInc/crewAI

OyeLabs. (2024). LangGraph vs CrewAI vs OpenAI Swarm: Which AI Agent Framework to Choose? Retrieved from https://oyelabs.com/langgraph-vs-crewai-vs-openai-swarm-ai-agent-framework/

Oxylabs. (2024). CrewAI vs. AutoGen: Comparing AI Agent Frameworks. Retrieved from https://oxylabs.io/blog/crewai-vs-autogen

Qian, C., et al. (2023). ChatDev: Communicative Agents for Software Development. arXiv preprint arXiv:2307.07924.

Rasheed, M., et al. (2024). LLM-Based Multi-Agent Systems for Software Engineering: Literature Review, Vision and the Road Ahead. arXiv preprint arXiv:2404.04834.

Relari. (2024). Choosing the Right AI Agent Framework: LangGraph vs CrewAI vs OpenAI Swarm. Retrieved from https://www.relari.ai/blog/ai-agent-framework-comparison-langgraph-crewai-openai-swarm

SmythOS. (2024). Agent Communication in Multi-Agent Systems: Enhancing Coordination and Efficiency in Complex Networks. Retrieved from https://smythos.com/ai-agents/multi-agent-systems/agent-communication-in-multi-agent-systems/

SuperAnnotate. (2024). Multi-agent LLMs in 2024 [+frameworks]. Retrieved from https://www.superannotate.com/blog/multi-agent-llms

TechCrunch. (2025). OpenAI adopts rival Anthropic's standard for connecting AI models to data. Retrieved from https://techcrunch.com/2025/03/26/openai-adopts-rival-anthropics-standard-for-connecting-ai-models-to-data/

Tran, N., et al. (2025). Multi-Agent Collaboration Mechanisms: A Survey of LLMs. arXiv preprint arXiv:2501.06322.

UC Berkeley Sky Lab. (2025). MAST – Multi-Agent System Testing. Retrieved from https://sky.cs.berkeley.edu/project/mast/

Wang, J., et al. (2025). LLM-Powered Multi-Agent System for Automated Crypto Portfolio Management. arXiv preprint arXiv:2501.00826.

Wu, Q., et al. (2023). AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation Framework. arXiv preprint arXiv:2308.16449.

ZenML. (2024). LLM Agents in Production: Architectures, Challenges, and Best Practices. Retrieved from https://www.zenml.io/blog/llm-agents-in-production-architectures-challenges-and-best-practices

Zhang, L., et al. (2024). Multi-LLM-Agent Systems: Techniques and Business Perspectives. arXiv preprint arXiv:2411.14033.

Zhang, Y., et al. (2025). A-Mem: Agentic Memory for LLM Agents. arXiv preprint arXiv:2502.12110.

Zhou, Y., et al. (2024). A survey on LLM-based multi-agent systems: workflow, infrastructure, and challenges. Vicinagearth, 1(1), 9.