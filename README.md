# Graph Database Question Answering System

A sophisticated question-answering system built on top of Neo4j graph database, utilizing LangChain and Groq for natural language processing.

## 🌟 Features

- Graph-based movie database integration with Neo4j
- Natural language question answering about movies, actors, and directors
- Integration with Groq's language models
- Cypher query generation from natural language questions
- Comprehensive movie dataset including titles, actors, directors, and genres

## 🛠️ Technologies Used

- Neo4j Graph Database
- LangChain
- Groq API
- Python 3.12
- Jupyter Notebook

## 📋 Prerequisites

- Python 3.12 or higher
- Neo4j database instance
- Groq API key
- Required Python packages:
  - langchain
  - langchain-groq
  - python-dotenv
  - neo4j

## 🚀 Setup and Installation

1. Clone the repository:
```bash
git clone https://github.com/0Xuser100/Neo4j_Build-a-Question-Answering-application-over-a-Graph-Database.git
```

2. Install required packages:
```bash
pip install langchain langchain-groq python-dotenv neo4j
```

3. Create a `.env` file with your credentials:
```env
NEO4J_URI="your-neo4j-uri"
NEO4J_USERNAME="your-username"
NEO4J_PASSWORD="your-password"
GROQ_API_KEY="your-groq-api-key"
```

## 💡 Usage

1. Start by importing the required libraries and setting up the environment variables
2. Initialize the Neo4j graph connection
3. Load the movie dataset into the graph database
4. Create the question-answering chain using LangChain and Groq
5. Ask questions about movies, actors, and directors!

Example queries:
```python
# Ask about movie directors
response = chain.invoke({"query": "Who was the director of the movie Casino?"})

# Query about movie actors
response = chain.invoke({"query": "Who were the actors of the movie Casino?"})

# Get statistics
response = chain.invoke({"query": "How many artists are there?"})
```

## 📊 Dataset

The movie dataset includes:
- Movie titles
- Release dates
- IMDB ratings
- Directors
- Actors
- Genres

## 🔍 Sample Queries and Results

```python
Q: "Who was the director of the movie Casino?"
A: "Martin Scorsese"

Q: "Who were the actors of the movie Casino?"
A: "Robert De Niro, Joe Pesci, Sharon Stone, and James Woods"

Q: "How many artists are there?"
A: "There are 1240 artists"
```

## 🏗️ Project Structure

```
.
├── .env                    # Environment variables
├── README.md              # Project documentation
└── movie_qa.ipynb         # Jupyter notebook with implementation
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Neo4j for the graph database platform
- LangChain for the amazing framework
- Groq for providing the language model API
- Movie dataset contributors
