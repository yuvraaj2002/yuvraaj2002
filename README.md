# Yuvraj Singh

AI engineer. I ship production LLM systems: agents, RAG and retrieval, document AI, and voice AI. Python and AWS. Based in India.

[Portfolio](https://master.d24o598po2jt0p.amplifyapp.com/) · [LinkedIn](https://www.linkedin.com/in/yuvraaj-singh/) · [X](https://x.com/yuvraajsinghh1) · [Writing](https://github.com/yuvraaj2002/engineering-blogs)

## Experience

### AIML Engineer, Relecura Technologies

Oct 2025 – Present · Employee of the Month

Patent-intelligence platform. Python, Django REST, AWS, Amazon Bedrock, Gemini, Claude.

- Built an explainable classification API that fuses dense-vector and BM25 retrieval (Reciprocal Rank Fusion) with schema-constrained LLM reranking. Reached 87.8% top-1 and 98.2% top-3 accuracy at taxonomy-branch level, up from a 62% baseline, on 5,000 client-labelled patents across 84 categories. Processes up to 100,000 publications per job.
- Built a serverless citation-extraction pipeline on AWS Step Functions that extracts, normalizes, and highlights citations in large patent PDFs. Gemini structured output for extraction, Claude tool use for each citation's bounding boxes, RapidOCR only on citation-bearing pages, large PDFs fanned out into 70-page batches.
- Shipped a private LiteLLM gateway to production: one OpenAI-compatible API over four Amazon Bedrock models (Mistral Large 3, DeepSeek V3.2, NVIDIA Nemotron, Claude Sonnet as fallback), with virtual keys, per-model rate limits, and spend tracking.

### AI Engineer (Contract), Independent Consulting

Mar 2025 – Aug 2026

Production AI agents and LLM products for healthcare, legal, and pharmacy clients. Owned architecture, backend, frontend, and deployment.

- **Voice-AI patient outreach for a US healthcare pharmacy** (Jul 2025 – Aug 2026). Multi-agent voice platform (Retell outbound, inbound, and processing agents) that handled 80,000+ calls, running 14-day, 7-call/6-SMS outreach for ~6,600 patients and 650+ concurrent sequences, with do-not-call compliance and race-safe enrollment. LangGraph QC agents that transcribe, diarize, and score recorded calls (94%+ average QC score), and an MCP server with 29 tools giving Claude live call, QC, and cost data.
- **Bilingual legal assistant for a legal firm** (Jul 2026 – Aug 2026). Answers questions in English or Spanish from the firm's own library, citing the exact sources (RAG on Bedrock with Claude, Cohere, and Qdrant). A pipeline reads large unordered legal PDFs, puts pages back in order, and flags conflicts for staff approval, then turns approved records into ready-to-send notices. Web app in Next.js, FastAPI, PostgreSQL, and S3, backed by 176 automated tests.
- **Multilingual, multimodal advisor for a pharmacy retailer** (Mar 2025 – Aug 2026). Customers talk by text, voice, or video in Italian, English, or French, and the advisor recommends catalog products. Video path picks the clearest frame, Gemini assesses the skin, and those findings become product recommendations. Multilingual RAG: query expansion, OpenAI embeddings in ChromaDB, Jina reranking (top 5 of 15), Groq Llama 3.3 70B answers, and Whisper transcription.

### Process Associate, MaxVal IP Services

Sep 2024 – Oct 2025

Mapped daily patent-analyst workflows on the USPTO platform. Built automations pairing Playwright with vision-based AI agents for document-layout understanding and structured extraction. Saved 18–20 hours per week and processed hundreds of documents in one-third of the manual time.

### Research Intern, Samsung PRISM

Samsung R&D Institute · Feb 2024 – Jul 2024

Built a computer-vision project using YOLO object detection to identify personal documents in images and automatically mask their sensitive information.

## Selected work

[**Tracehound**](https://github.com/yuvraaj2002/Tracehound/tree/main) — what I'm building now. Evidence-first multi-agent investigation for on-call engineers. Given an alert, a LangGraph workflow triages it, then specialist agents read logs (Loki), metrics (Prometheus), traces (Tempo), and deploys (GitHub). A hypothesis step returns candidate root causes, and every claim cites evidence. FastAPI, PostgreSQL, and a React UI. Pinned scenario files cover the seeded path.

[**InjectGuard**](https://github.com/yuvraaj2002/InjectGuard) — lab for building, attacking, and measuring prompt-injection defenses on a RAG and tool-using agent. The agent is a synthetic banking-ops assistant: keyword search over policy docs, and mock tools for transfers and refunds. In the repo: a local Llama Prompt Guard 2 classifier, an isolation path (planner, quarantine model, and answer model on Groq), and an eval runner. Synthetic data only.

[**FlowDesk**](https://github.com/yuvraaj2002/FlowDesk) — support copilot for a fictional SaaS CRM. The target is cited answers, live account tools, writes that run only after human approval, and reproducible evals. The path that runs today is a React UI, FastAPI, and local Ollama. Qdrant and the seed corpus are in the repo; chat calls the model directly.

[**Engineering blogs**](https://github.com/yuvraaj2002/engineering-blogs) — notes on AI security and guardrails. The first post is on why prompt injection can't be fully solved, and what you can still contain.

## Stack

- **Agents and models:** LangGraph, MCP, tool use, Retell, ElevenLabs, Claude, Amazon Bedrock, OpenAI, Gemini, Groq, Cohere, Jina, LiteLLM, Ollama
- **Retrieval and documents:** dense and BM25, Reciprocal Rank Fusion, reranking, Qdrant, ChromaDB, OCR, structured outputs, evals
- **Application:** Python, FastAPI, Django, Celery, Playwright, React, TypeScript, Next.js, pytest, Vitest
- **Data and AWS:** PostgreSQL, MySQL, Redis, S3, ECS, Lambda, Step Functions, SQS, EventBridge, RDS, Docker

Bachelor's, Artificial Intelligence and Machine Learning, Chandigarh University, 2021–2025.

Microsoft Learn Student Ambassador, Apr 2023 – Jan 2025. Delivered ML and Python workshops to 150+ students globally, with a 95% satisfaction rate.
