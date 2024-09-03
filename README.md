# Knowlegegrph_langchain
1. Installation of required libraries: LangChain, Neo4j, and related packages.
2. Configuration of Neo4j database connection:
  Neo4j URI, username, and password are set.
  These credentials are also set as environment variables.
3. Initialization of Neo4j graph connection using LangChain's Neo4jGraph.
4. Setup of a language model:
 Using Groq API with the "Gemma2-9b-It" model.
5.Creation of a sample document about Mark Zuckerberg.
6. Use of LLMGraphTransformer to convert the document into graph format.
7. Exploration of the generated graph documents, including nodes and relationships.
8. Preparation of a Cypher query to load movie data into the Neo4j database:
 The query is designed to create Movie nodes with properties like id, released date, title, and IMDb rating.
 It also creates Person nodes for directors and actors, and Genre nodes.
 Relationships are established between movies and people (DIRECTED, ACTED_IN) and between movies and genres (IN_GENRE).
9. Execution of the movie data loading query using the graph.query() method.

The notebook demonstrates the process of setting up a graph database, integrating it with a language model, and preparing to populate it with movie-related data.
