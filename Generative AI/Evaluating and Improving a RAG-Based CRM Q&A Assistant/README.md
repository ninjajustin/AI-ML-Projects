# Evaluating and Improving a RAG-Based CRM Q&A Assistant

In this assignment, I worked with a provided Python notebook to analyze and improve a Retrieval-Augmented Generation (RAG) question-answering assistant built on Salesforce CRM documents. By running and modifying the notebook, I examined how the assistant retrieves relevant documents and uses them to generate answers to user queries.

I first evaluated the assistant’s baseline behavior, reviewing the default prompt, its initial responses, and scoring their relevance and completeness. I then iteratively applied prompt engineering techniques to improve formatting, transparency, and trustworthiness, including adding source citations and generating executive-style summaries across multiple documents.

Next, I analyzed the retrieval pipeline, inspecting the relevance of retrieved documents and considering how factors like chunk size and embeddings affect retrieval quality. I also explored hallucination risks by asking questions not covered in the dataset and proposing prompt-based and pipeline-based strategies to reduce incorrect or fabricated answers.

Overall, this assignment strengthened my understanding of how prompt design, retrieval quality, and guardrails interact in enterprise RAG systems, and highlighted the tradeoffs between clarity, completeness, and accuracy when preparing an AI assistant for real-world deployment.