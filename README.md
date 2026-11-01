<div align="center">

<img src="./assets/hero.svg" alt="Amjath Hussain S - AI Engineer. Building agentic AI systems, RAG applications and LLM-powered solutions." width="100%">

</div>

<br>

<img src="./assets/h-about.svg" alt="About" width="100%">

I'm a final-year B.Tech student in Artificial Intelligence and Data Science (Class of 2027), and I build LLM applications that go beyond a demo: retrieval that is evaluated, agents that are guarded, and pipelines that return structured, validated output.

My focus is agentic AI and retrieval-augmented systems, especially natural-language interfaces to data. These are agents that plan, call tools, remember context, and ask for human approval before doing anything risky.

National finalist at the Cognizant TechnoVerse Hackathon 2026, and Microsoft-certified in Azure AI app and agent development and in Fabric analytics.

<br>

<img src="./assets/h-build.svg" alt="What I Build" width="100%">

<img src="./assets/build.svg" alt="Agentic AI systems, RAG applications, LLM-powered solutions, and intelligent automation" width="100%">

<br>

<img src="./assets/h-projects.svg" alt="Featured Projects" width="100%">

<a href="https://github.com/amjathhussain31/Data-Agent"><img src="./assets/p1.svg" alt="DataMind Agent - National Finalist. Conversational analytics: plain English to SQL, summaries and charts." width="100%"></a>

- **Problem:** business users depend on analysts and SQL to answer simple data questions.
- **Built:** upload a CSV, ask in plain English, and get the generated SQL, a written summary and an interactive chart.
- **Architecture:** `Guardrails` → `Router (SQL / RAG / hybrid)` → `Memory` → `Schema-aware SQL` → `SQL firewall + human approval` → `DuckDB on S3` → `Summary` → `Chart`. It is a 12-node LangGraph supervisor, with 8 tools exposed over MCP behind a FastAPI gateway and a documented 31-test suite.
- **Repository:** [amjathhussain31/Data-Agent](https://github.com/amjathhussain31/Data-Agent)

<a href="https://github.com/amjathhussain31/local-sql-agent"><img src="./assets/p2.svg" alt="SQL Agent. ReAct agent grounded in the schema and a business glossary." width="100%"></a>

- **Problem:** generated SQL is only as good as the model's grasp of the schema and the business vocabulary.
- **Built:** a conversational analytics agent for SQLite, PostgreSQL and MySQL that answers, explains the result and draws the chart.
- **Architecture:** `Question` → `LangChain ReAct agent` → tools for `schema lookup`, `glossary RAG (FAISS)`, `SQL execution`, `insights` and `charts` → `Answer`. Short- and long-term memory, input and output guardrails, and Langfuse tracing sit around the loop.
- **Repository:** [amjathhussain31/local-sql-agent](https://github.com/amjathhussain31/local-sql-agent)

<a href="https://github.com/amjathhussain31/RFP-Intelligence-Extractor"><img src="./assets/p3.svg" alt="RFP Intelligence Extractor. RFP packages to 20 validated fields, addenda-aware." width="100%"></a>

- **Problem:** RFP packages mix long PDFs, portal pages and addenda, and a later addendum can silently change a deadline or requirement.
- **Built:** a pipeline that turns an RFP package into validated JSON with 20 fields, such as due date, bid bond and payment terms.
- **Architecture:** `PDF / HTML parsing` → `cleaning` → `metadata-tagged chunks` → `FAISS retrieval per field` → `addendum override` → `LLM extraction` → `Pydantic validation`. Fields the documents do not support come back as `null`, and 12 tests are documented.
- **Repository:** [amjathhussain31/RFP-Intelligence-Extractor](https://github.com/amjathhussain31/RFP-Intelligence-Extractor)

<a href="https://github.com/amjathhussain31/Week-2-RAG-Chatbot"><img src="./assets/p4.svg" alt="RAG Chatbot with Evaluation. Document Q&A that measures its own quality with RAGAS." width="100%"></a>

- **Problem:** language models hallucinate on private documents, and "it seems to work" is not a quality bar.
- **Built:** a PDF question-answering chatbot with session memory and switchable open models (Mistral 7B, LLaMA 2), evaluated with RAGAS.
- **Architecture:** `Loader` → `Splitter` → `Embeddings` → `FAISS retriever` → `Chain + memory` → `RAGAS evaluator`. In the sample run in the README, faithfulness and answer relevancy scored 1.00 and context recall 0.60, and the repository lists the retrieval limits it found.
- **Repository:** [amjathhussain31/Week-2-RAG-Chatbot](https://github.com/amjathhussain31/Week-2-RAG-Chatbot)

<a href="https://github.com/amjathhussain31/Week-3-Domain-Aware-Agent"><img src="./assets/p5.svg" alt="Domain-Aware ReAct Agent. Local agent with guardrails, a workflow graph and dual memory." width="100%"></a>

- **Problem:** an agent that can call tools also needs boundaries, memory and a way to show its reasoning.
- **Built:** a fully local conversational agent that blocks out-of-domain or unsafe requests, remembers users across sessions, and shows a live tool trace.
- **Architecture:** `Input validation` → `Guardrail rails` → `Graph routing` → `ReAct agent` → `Optional human approval` → `Output formatter`. Memory has two layers, the last six interactions plus a long-term JSON store, and the agent has six tools.
- **Repository:** [amjathhussain31/Week-3-Domain-Aware-Agent](https://github.com/amjathhussain31/Week-3-Domain-Aware-Agent)

<a href="https://github.com/amjathhussain31/Week-1-Presidio-Summer-Internship-26"><img src="./assets/p6.svg" alt="PDF Question Answering. End-to-end RAG over a PDF with a persistent vector store." width="100%"></a>

- **Problem:** answering questions from a PDF with answers grounded in its content rather than the model's memory.
- **Built:** a notebook-based RAG application with a persistent vector store.
- **Architecture:** `PDF loading` → `Chunking` → `Sentence-transformer embeddings` → `ChromaDB` → `Top-chunk retrieval` → `Local LLM answer`.
- **Repository:** [amjathhussain31/Week-1-Presidio-Summer-Internship-26](https://github.com/amjathhussain31/Week-1-Presidio-Summer-Internship-26)

<br>

<img src="./assets/h-expertise.svg" alt="Technical Expertise" width="100%">

| Area | What I work with |
|---|---|
| <img src="./assets/e-ai.svg" width="26" align="absmiddle" alt=""> **AI Engineering** | Evaluation-driven development (RAGAS), input and output guardrails, tracing and observability (Langfuse, CloudWatch), structured outputs validated with Pydantic |
| <img src="./assets/e-agent.svg" width="26" align="absmiddle" alt=""> **Agentic AI Systems** | LangGraph supervisor workflows, ReAct agents, tool calling, Model Context Protocol servers, short- and long-term memory, human-in-the-loop approval |
| <img src="./assets/e-rag.svg" width="26" align="absmiddle" alt=""> **RAG & Knowledge Retrieval** | Chunking strategies, sentence-transformer embeddings, FAISS and ChromaDB, query routing across SQL, documents and hybrid, per-field context budgeting |
| <img src="./assets/e-llm.svg" width="26" align="absmiddle" alt=""> **LLM Application Development** | AWS Bedrock, Gemini, Groq and local models through Ollama, LangChain, natural language to SQL, Streamlit interfaces |
| <img src="./assets/e-backend.svg" width="26" align="absmiddle" alt=""> **Backend Engineering** | FastAPI and REST APIs, PostgreSQL, MySQL, DynamoDB, DuckDB, testing with pytest |
| <img src="./assets/e-cloud.svg" width="26" align="absmiddle" alt=""> **Cloud Technologies** | AWS (Bedrock, S3, DynamoDB, CloudWatch, EC2), Microsoft Azure, IBM Cloud |

<br>

<img src="./assets/h-stack.svg" alt="Technology Stack" width="100%">

<img src="./assets/stack.svg" alt="Scrolling list of technologies: Python, Java, C++, SQL, LangChain, LangGraph, RAG, MCP, FastAPI, PostgreSQL, MySQL, DynamoDB, FAISS, ChromaDB, AWS, Azure, IBM Cloud, Pandas, NumPy, Power BI" width="100%">

**Programming** &nbsp; `Python` `Java` `C++` `SQL`
**AI / ML** &nbsp; `Machine Learning` `Deep Learning` `NLP` `Generative AI`
**LLM engineering** &nbsp; `LangChain` `LangGraph` `RAG` `Agentic AI` `MCP` `RAGAS` `Langfuse`
**Backend** &nbsp; `FastAPI` `REST APIs`
**Databases** &nbsp; `PostgreSQL` `MySQL` `DynamoDB` &nbsp;·&nbsp; **Vector** &nbsp; `FAISS` `ChromaDB`
**Cloud** &nbsp; `AWS` `Microsoft Azure` `IBM Cloud`
**Data and analytics** &nbsp; `Pandas` `NumPy` `Matplotlib` `Power BI`
**Tools** &nbsp; `Git` `GitHub` `VS Code` `Postman` `Jupyter`

<br>

<img src="./assets/h-achievements.svg" alt="Achievements" width="100%">

<a href="https://github.com/amjathhussain31/Data-Agent"><img src="./assets/ach1.svg" alt="National Finalist, Cognizant TechnoVerse Hackathon 2026, with DataMind Agent" width="100%"></a>

<a href="https://app.notion.com/p/ajayr07/Presidio-Summer-Internship-26-31fbd94ad5e280b69acfc842ce0bb018"><img src="./assets/ach2.svg" alt="Presidio GenAI Foundations Internship" width="100%"></a>

<details>
<summary>Presidio weekly deliverables and hands-on practice</summary>

| Week | Work | Repository |
|---|---|---|
| 1 - GenAI Foundations | RAG practice | [Rag-Practice](https://github.com/amjathhussain31/Rag-Practice) |
| 1 - GenAI Foundations | Deliverable: Simple RAG application (PDF question answering) | [Week-1-Presidio-Summer-Internship-26](https://github.com/amjathhussain31/Week-1-Presidio-Summer-Internship-26) |
| 2 - Prompting and LangChain | LangChain sequential practice | [LangChain-Practice](https://github.com/amjathhussain31/LangChain-Practice) |
| 2 - Prompting and LangChain | Multimodal chatbot (text and images) | [Multimodal-Chatbot-Practice](https://github.com/amjathhussain31/Multimodal-Chatbot-Practice) |
| 2 - Prompting and LangChain | Streamlit chatbot interface | [Streamlit-Practice](https://github.com/amjathhussain31/Streamlit-Practice) |
| 2 - Prompting and LangChain | Mini task: RAG chatbot with FAISS and RAGAS | [Week-2-RAG-Chatbot](https://github.com/amjathhussain31/Week-2-RAG-Chatbot) |
| 3 - Agentic AI | Agent practice: reasoning, tools and memory | [agent-practice](https://github.com/amjathhussain31/agent-practice) |
| 3 - Agentic AI | Mini task: domain-aware ReAct agent | [Week-3-Domain-Aware-Agent](https://github.com/amjathhussain31/Week-3-Domain-Aware-Agent) |

</details>

<img src="./assets/cert1.svg" alt="Microsoft Certified: Fabric Analytics Engineer Associate (DP-600), earned August 2026, valid until August 2027" width="100%">

<img src="./assets/cert2.svg" alt="Microsoft Certified: Azure AI Apps and Agents Developer Associate, earned August 2026, valid until August 2027" width="100%">

<br>

<img src="./assets/h-connect.svg" alt="Connect With Me" width="100%">

<p align="center">
  <a href="https://www.linkedin.com/in/amjath-hussain-s/"><img src="./assets/c-linkedin.svg" alt="LinkedIn" width="230"></a>
  <a href="mailto:amjathhussain.ah@gmail.com"><img src="./assets/c-email.svg" alt="Email: amjathhussain.ah@gmail.com" width="230"></a>
  <a href="https://github.com/amjathhussain31"><img src="./assets/c-github.svg" alt="GitHub" width="230"></a>
</p>

<img src="./assets/footer.svg" alt="" width="100%">
