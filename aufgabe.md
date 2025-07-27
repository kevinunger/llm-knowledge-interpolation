

LLM Reasoning for Interpolation of Knowledge Gaps in External Contexts for RAG
This project investigates how Large Language Models (LLMs) can address knowledge gaps in external contexts for Retrieval-Augmented Generation (RAG) tasks. In RAG, incomplete or irrelevant documents retrieved can limit the quality and completeness of generated responses, especially in long-form responses. This project aims to investigate LLM-based reasoning approaches to assess and improve the relevance and completeness of information retrieved from external sources. Additionally, it examines how LLMs can leverage their internal knowledge to fill in missing details, refine the retrieval process, and ultimately generate more comprehensive and high-quality responses. The goal is to develop methods that enable RAG systems to better handle incomplete or imperfect external contexts, improving their overall performance in generating detailed and accurate long-form responses.

Problem Description:
In RAG, relevant contexts are often not or only partially retrieved, which limits the quality and completeness of the LLM-generated responses. This is especially the case for long-form responses where relevant information may be scattered across several documents that all need to be retrieved.

RQ 1:
How can we use LLM-based reasoning to decide whether the information from the retrieved documents is relevant, correct , and complete to generate a comprehensive response to a query?

RQ 2:
Given the retrieved documents are irrelevant, incorrect, or incomplete for a query, how can we use LLM-based reasoning to interpolate the information using the internal, parametric knowledge of an LLM to add relevant context and enhance the completeness and quality of the generated response?

RQ 3:
Given the retrieved documents are irrelevant, incorrect, or incomplete for a query, how can we use LLM-based reasoning to choose a different retrieval approach that results in retrieving better external contexts that enhances the completeness and quality of the generated response?

RQ 4:
What are pros and cons for using additional retrieved, external knowledge vs. parametric, internal knowledge to interpolate knowledge gaps in external contexts for RAG?

Required skills & experiences:
Retrieval Augmented Generation, LLM prompting strategies, understanding of LLM reasoning models (e.g, DeepSeek-R1, OpenAI o1 and o3-mini, etc.), document retrieval and text embeddings (e.g, sentence embeddings etc.), vector databases (e.g, Weaviate, Pinecone, etc.).

Beneficial skills & experiences: LLM agents and tool use, graph databases (RDF graphs, Neo4j, etc.), LLM fine-tuning.
