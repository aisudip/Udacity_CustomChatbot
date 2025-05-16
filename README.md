# Udacity_CustomChatbot
This custom chatbot addresses ChatGPT’s shortcomings that arise from its inability, in its native form, to support queries about events beyond 2021. For example, if asked “Who is the president of the USA?”, it would respond with “Joe Biden,” because it is unaware that an election took place in November 2024 and that Donald Trump assumed the presidency on January 20, 2025. To bridge this gap, the Wikipedia 2025 database has been integrated to cover events in 2025. By enhancing this capability, the chatbot can now respond to queries about current events more accurately.

This has been achieved with the following steps

1. Load '2025' current events database from Wikipedia into Pandas dataframe and clean it for further processing.
2. Generate embeddings for the above database that has been loaded. The embeddings is generated for model 'text-embedding-ada-002'.
3. Create a function to calculate distance for a query and sort by relevance
4. Create a function to generate prompt keeping in view the maximum number of tokens
5. Create a custom query completion function that returns the answer by integrating context related to current events
6. Test custom chatbot with questions

