# 🎬 Personalized-Movie-Recommendation-System-Neo4j-Graph-Database-Knowledge-Graph-LLM-AI-Agents 
This repository contains a **personalized movie recommendation system** that leverages **Neo4j knowledge graphs, LangChain LLMs, and AI agents**. It extracts movie relationships (genres, keywords, cast, crew, etc.) from a dataset, stores them in a **Neo4j graph database**, and uses **LLM-based reasoning** to suggest similar movies based on shared attributes.

## 🚀 Features  
✅ **Knowledge Graph Integration**: Uses **Neo4j** to store and query movie relationships.  
✅ **AI-Powered Recommendations**: Utilizes **LangChain LLMs** for natural language query processing.  
✅ **Query Refinement**: Refines vague user inputs for better movie suggestions.  
✅ **Graphical User Interface (GUI)**: Built using **Gradio** for user interaction.  
✅ **Evaluation Metrics**: Measures system accuracy with **precision, recall, and F1-score**.  

## 📂 Dataset  
The system processes the **TMDb 5000 Movies dataset** and integrates information about:  
🎭 **Genres**  
🔑 **Keywords**  
🎬 **Cast & Crew**  
🏢 **Production Companies**  
🌍 **Production Countries**  

## 🛠 Installation  
To run this system, install the required dependencies:  
```bash
pip install langchain langchain_community neo4j gradio
```

## 🔗 Neo4j Database Setup  
Connect to a **Neo4j Sandbox** or local database using the credentials:  
```python
uri = "neo4j+s://your-database-uri"
username = "neo4j"
password = "your-password"
driver = GraphDatabase.driver(uri, auth=(username, password))
```

## 🤖 LLM Integration  
The system utilizes **Meta-Llama-3-8B-Instruct** from **Hugging Face** for AI-powered recommendations. It constructs movie similarity queries and generates results using **LangChain LLM agents**.  

## 🎨 GUI for Movie Search  
A **Gradio-based** interface allows users to input a movie title and receive recommendations:  
```python
interface = gr.Interface(fn=get_similar_movies, inputs="text", outputs="text", title="Movie Recommendation System")
interface.launch()
```

## 📊 Evaluation  
The system is evaluated using **genre-based ground truth** and the following metrics:  
✔ **Precision**  
✔ **Recall**  
✔ **F1-score**  

## 💡 How It Works  
1️⃣ Loads the **TMDb dataset** and extracts relevant information.  
2️⃣ Stores **movies and relationships** in a **Neo4j knowledge graph**.  
3️⃣ Uses an **LLM-based agent** to generate movie recommendations.  
4️⃣ Provides a **user-friendly interface** for interaction.  
5️⃣ Evaluates recommendations using **precision, recall, and F1-score**.  

## 🛠 Future Enhancements  
- 🔍 Improve query understanding using **retrieval-augmented generation (RAG)**.  
- 🎞️ Incorporate **user watch history** for personalized recommendations.  
- 🤖 Experiment with **other LLM models** for better reasoning.  

## 🏁 Run the System  
Clone this repository and execute the Python script to start the movie recommendation system!
