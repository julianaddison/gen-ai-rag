# PolicyPal
PolicyPal is a demo chatbot experience to redefine the way users engage with insurance. Say goodbye to complicated forms and confusing jargon – with PolicyPal, obtaining insurance information becomes as easy as having a conversation. This demo utilizes Retrieval-Augmented Generation (RAG) on an open-source [insurance Q&A corpus](https://github.com/shuzi/insuranceQA/tree/master) with real-world user questions on various insurance domains.

## Tech Stack
In this Google Collab notebook, a RAG pipeline in Python is implemented using OpenAI's LLM in combination with a Weaviate vector database and an OpenAI embedding model. LangChain is used for orchestration with Gradio's ChatBot module used as a simple web user interface.

## Prerequisites
You will need to have the following before continuing:

- **OpenAI API key**: We will generate embeddings from text via OpenAI's inference service. The Ada model (version 2) costs $0.0001 per 1,000 tokens. For this demo, the embedding of a subset of the InsuranceCorpus was $0.23.
- **Weaviate API key and cluster URL**: Run a Weaviate instance as a managed service using Weaviate Cloud Services (WCS). The free trial plan provides a sandbox for 14 days. No payment information is required. The sandbox expires after the trial period but a new free trial sandbox can be created anytime. Refer to the Setup section in this article for more information.
Store the keys and url in Google Collab Secrets. Refer to this article on how to store the keys.

Store the keys and url in Google Collab Secrets. Refer to this [article](https://medium.com/@parthdasawant/how-to-use-secrets-in-google-colab-450c38e3ec75) on how to store the keys.
