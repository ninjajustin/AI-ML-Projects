# Integrating LangGraph into an AI Email Assistant

In this assignment, I enhanced an existing AI email assistant by integrating LangGraph to better structure and manage the email processing workflow. The project focused on supporting a busy software engineering manager by automatically prioritizing, summarizing, and drafting responses to emails using the Yesterbox approach, which processes the previous day’s emails first.

Instead of relying on a single, linear LLM pipeline, I used LangGraph to define multiple AI agents, each responsible for a specific task such as email categorization, summarization, response drafting, and executive-level reporting. This made the workflow more modular, easier to understand, and simpler to extend or reuse in other contexts.

By refactoring the notebook to reduce prompt complexity and centralize agent logic, the system became cleaner and more maintainable while still producing actionable summaries and professional response drafts for high-priority emails. Overall, integrating LangGraph improved the clarity, control flow, and scalability of the existing project, demonstrating how agent-based orchestration can strengthen real-world AI applications.