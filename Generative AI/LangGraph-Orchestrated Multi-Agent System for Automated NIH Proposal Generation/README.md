# LangGraph-Orchestrated Multi-Agent System for Automated NIH Proposal Generation

This project extends an existing LangChain-based research assistant by integrating LangGraph to orchestrate a multi-step, agent-driven workflow for NIH proposal generation. Rather than redesigning the system from scratch, LangGraph is used to structure, control, and iterate over already-implemented components such as document ingestion, retrieval, summarization, idea generation, proposal drafting, and evaluation.

The workflow begins by ingesting and embedding a NOFO document, followed by large-scale analysis and categorization of prior research papers. These outputs feed into an LLM-driven idea generation stage. LangGraph then manages the stateful proposal loop, coordinating a proposal-writing agent and a reviewer agent that iteratively refine the draft until it meets predefined quality thresholds aligned with NIH evaluation criteria.

By introducing LangGraph, the project gains:

Explicit control over execution flow (generation → evaluation → revision)

Clear separation of agent responsibilities

Deterministic stopping conditions and human-in-the-loop checkpoints

Easier extensibility for future agents (e.g., budget reviewers, compliance checkers)

Overall, LangGraph serves as the coordination layer that turns an existing collection of LLM tools into a robust, modular, and evaluatable end-to-end system for automated NIH proposal drafting.