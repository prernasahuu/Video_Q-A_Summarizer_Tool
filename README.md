#Q-ABot-RAGpipeline
##Objective:
To build a Question and Answer Bot that will help to generate response to query on the basis of given Context. In this project, I have used word embeddings using the msmarco-MiniLM-L-6-v3 model and integrated it with the ChromsDB vector database to build a robust RAG pipeline. The input for the bot was taken as Video("context"), allowing the model to understand context and provide domain specific and top ranked answers to the query efficiently.

###RAG (Retrival Augumented Generation):
Retrieval-augmented generation (RAG) is a technique for enhancing the accuracy and reliability of generative AI models with facts fetched from external sources.
In a RAG workflow, a user submits a question, and the system first retrieves the most relevant documents using vector similarity search, leveraging tools like FAISS or ChromaDB. These documents are then passed to a generative model, which synthesizes an answer grounded in the retrieved information, leading to more accurate and fact-based responses. This hybrid approach improves the generative model's performance by reducing hallucinations (when the model generates incorrect or fabricated information) and enhancing the relevance of the answers. 
###About Vector Database: 
ChromaDB is a vector database designed to efficiently store and retrieve high-dimensional vector embeddings, making it an excellent tool for building Q&A bots. In a Q&A system, user questions and potential answers are typically converted into embeddings using language models like MiniLM or BERT. These embeddings are numerical representations of text that capture the meaning and context, allowing the system to perform semantic searches. ChromaDB stores these embeddings and performs fast, scalable similarity searches to find the most relevant answer based on the input question.
###Word Embedding Model:
The MiniLMv6 (Mini Language Model version 6) is a compact transformer-based language model designed for efficient natural language processing tasks. It is part of Microsoft's family of models optimized for tasks like text embedding, similarity search, and more. MiniLMv6 model is used for both the user's query and pre-written context in the database that are transformed into embeddings (vector representations) that capture their semantic meaning. The system compares the query's embedding to the pre-embedded context using cosine/dot product/Euclidean Distance similarity, measuring how close the vectors are to each other in terms of meaning. The answers with the highest similarity scores are ranked and retrieved as the most relevant and spcidfic answer to the query. This approach enables efficient and accurate retrieval of answers based on the meaning of the query, rather than just keyword matching.
###Wishper:
Whisper is an automatic speech recognition (ASR) model developed by OpenAI, designed to transcribe speech into text. When used in conjunction with tools like a Q&A bot, Whisper can transcribe audio or video into text, which can then be processed by the system to provide relevant answers or actions
###OpenAI:
The OpenAI library gives access to GPT models, like GPT-3 and GPT-4, which can be used for generating responses to user queries in a Q&A bot.You can leverage the natural language understanding and generation abilities of GPT to answer complex questions, generate summaries, or explain concepts in simple terms.

##Results:
As it consumes alot of time for students or any person, to go through the whole context, so as to find out an answer to the specific query. Hence, this education based tool,provides relaxation in time comsumption and manual efforts, with the atmost flexibility.
