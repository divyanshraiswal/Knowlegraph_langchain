# Knowlegegrph_langchain
Installation of required libraries: LangChain, Neo4j, and related packages.
Configuration of Neo4j database connection:

Neo4j URI, username, and password are set.
These credentials are also set as environment variables.


Initialization of Neo4j graph connection using LangChain's Neo4jGraph.
Setup of a language model:

Using Groq API with the "Gemma2-9b-It" model.


Creation of a sample document about Mark Zuckerberg.
Use of LLMGraphTransformer to convert the document into graph format.
Exploration of the generated graph documents, including nodes and relationships.
Preparation of a Cypher query to load movie data into the Neo4j database:

The query is designed to create Movie nodes with properties like id, released date, title, and IMDb rating.
It also creates Person nodes for directors and actors, and Genre nodes.
Relationships are established between movies and people (DIRECTED, ACTED_IN) and between movies and genres (IN_GENRE).


Execution of the movie data loading query using the graph.query() method.

The notebook demonstrates the process of setting up a graph database, integrating it with a language model, and preparing to populate it with movie-related data.
