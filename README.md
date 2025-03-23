# Personalized-Movie-Recommendation-System-Neo4j-Graph-Database-Knowledge-Graph-LLM-AI-Agents 
This project is a knowledge graph-based movie recommendation system that integrates Neo4j, LLMs, and AI agents to provide personalized movie recommendations. It processes movie datasets, builds a structured knowledge graph, and utilizes LLM-powered AI agents to generate recommendations.  

Features:  

    Loads and processes movie data from CSV files  
    Connects to a Neo4j graph database to store and query movie-related knowledge  
    Builds a knowledge graph with relationships between movies, genres, cast, crew, and production companies  
    Utilizes a custom LLM model to generate responses based on movie attributes  
    Retrieves similar movies using AI-driven search techniques  
    Provides a graphical user interface for users to interact with the recommendation system  
    Evaluates recommendations using precision, recall, and F1-score  

Installation:

    Run the following commands to install the required dependencies:  
    pip install langchain  
    pip install langchain_community  
    pip install neo4j  
    pip install gradio  

Data Processing:  

    The system loads movie data from CSV files and merges them to create a structured dataset. A test dataset containing 20 movies is extracted for processing.  

Knowledge Graph Construction:

    The system connects to a Neo4j database and creates nodes and relationships for movies, genres, keywords, cast, crew, production companies, and countries. The knowledge graph serves as a foundation for  querying and retrieving related movie information.  

LLM Integration: 

    A custom LLM model is implemented to process user queries and provide movie recommendations. The model interacts with an external API to generate responses.  

AI Agents and Query Processing:  

    The AI agents refine user queries, retrieve knowledge from Neo4j, and use structured prompts to generate movie recommendations. The system considers factors like shared genres, cast, and keywords to find similar movies.  

Graphical User Interface:

    The system includes an interactive GUI built with Gradio, allowing users to input a movie title and receive recommendations in real time.  

Recommendation System Evaluation:

    The recommendations are evaluated using precision, recall, and F1-score, comparing the generated results with genre-based ground truth data.  

Usage:  

    Load the movie dataset and merge it  
    Connect to the Neo4j database  
    Create the knowledge graph  
    Use AI agents to process queries and generate recommendations  
    Interact with the system via the GUI  
    Evaluate the recommendation performance  

This project demonstrates the integration of knowledge graphs and AI models for an advanced recommendation system.
