# RAG_example

This is a sample code focusing on creating basic RAG that would extract relevant information from the document of interest and generate response based on the most similar chunks using GPT model.
The code was used for the txt document 'Healthy Nutrition Guidelines' that was taken from [this public website](https://www.healthline.com/nutrition/how-to-eat-healthy-guide#bottom-line). 

A brief note on the selected specifications:
* Sentence transformer model: all-MiniLM-L6-v2
* FAISS (Facebook AI Similarity Search) to create vector database to organize and store vectors for efficient similarity search (using L2 distance)
* Langchain for Recursive Spliting (chunk_size=250, chunk_overlap=50): splits data at different levels until the chunks of appropriate size.
