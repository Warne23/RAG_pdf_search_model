# Retrieval-Augmented Generation (RAG) Based Search Tool
![image](https://github.com/Warne23/RAG_pdf_search_model/assets/101012996/e15493c3-e38a-4006-ade6-a52fbd18efdb)
## Requirements
- Langchain
- Llama index
- Transformers
- Pypdfs
- LlamaCPP

## Steps
- Upload the PDFs to a directory and read them.
- Build a RAG model using the Llama Cpu. We are using the 7B parameter 5-bit Mistral llm. [Link to Model](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.1-GGUF/blob/main/mistral-7b-instruct-v0.1.Q5_K_S.gguf)
- Set the temperature, context window, and number of  gpu layers you want to use.
- Convert the Documents to Vectors using a pre-trained model from Hugging face
[Link to Model](https://huggingface.co/thenlper/gte-large)
- Encapsulate the embedded model, and the LLM and specify the chunk size
- Build the Vector Index database containing the encapsulated model
- Run a query engine to take the input prompts
- Our model is ready.

- You can reduce the chunk size or reduce the context window to fasten the process.
You can also use different llms like Google Gemma or Meta’s Llama2.(I tried google Gemma but Mistral was performing better)




