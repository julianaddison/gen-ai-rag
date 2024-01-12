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

# References
1. Combining LangChain and Weaviate [Link](https://weaviate.io/blog/combining-langchain-and-weaviate)

1. LangChain Vectorstores: Weaviate [Link](https://python.langchain.com/docs/integrations/vectorstores/weaviate#prerequisites)

1. Data used in Demo: InsuranceQA Corpus [Link](https://github.com/shuzi/insuranceQA/tree/master)

1. Retrieval-Augmented-Generation from theory to LangChain implementation [Link](https://towardsdatascience.com/retrieval-augmented-generation-rag-from-theory-to-langchain-implementation-4e9bd5f6a4f2).

1. Question Answering in Weaviate with OpenAI Q&A module [Link](https://github.com/openai/openai-cookbook/blob/main/examples/vector_databases/weaviate/question-answering-with-weaviate-and-openai.ipynb)

1. Building an Interactive Streaming Chatbot with Langchain, Transformers, and Gradio [Link](https://medium.com/@shrinath.suresh/building-an-interactive-streaming-chatbot-with-langchain-transformers-and-gradio-93b97378353e)

1. Creating Your Own Chatbot: A Beginner-Friendly Tutorial with OpenAI, LangChain, Gradio, and Wikipedia [Link](https://medium.com/@kristenkehrer/creating-your-own-chatbot-a-beginner-friendly-tutorial-with-openai-langchain-gradio-and-8440c96fc9b4)

1. Getting Started with Weaviate: A Beginner’s Guide to Search with Vector Databases [Link](https://towardsdatascience.com/getting-started-with-weaviate-a-beginners-guide-to-search-with-vector-databases-14bbb9285839)

