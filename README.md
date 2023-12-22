# Game of Thrones Network Analysis

## Introduction
This project aims to perform an in-depth analysis of the Game of Thrones network using Apache GraphX, Neo4j, and Spark ML. The dataset used for this analysis is available [here](https://www.kaggle.com/code/mmmarchetti/game-of-thrones-network-analysis/input).
Here is an overview of the project architecture:
![image](https://github.com/rmakaoui/Project_GraphX_SparkML_neo4j/assets/101502312/727f6d92-84bc-412f-803c-813749520001)

## Project Overview
The project comprises several key steps:

1. **Read the Dataset:**
   - Use the provided [Game of Thrones dataset](https://www.kaggle.com/code/mmmarchetti/game-of-thrones-network-analysis/input).

2. **Connect Spark GraphX with Neo4j:**
   - Follow the instructions in the [Neo4j Spark Connector documentation](https://neo4j.com/docs/spark/current/) to establish a connection.

3. **Import Dataset into Neo4j:**
   - Use the Cypher query language to perform CRUD operations on the dataset in Neo4j.

4. **Apache Zeppelin with GraphX:**
   - Integrate Apache Zeppelin with GraphX.
   - Read data from Neo4j.
   - Conduct exploratory data analysis.
   - Execute five graph algorithms of your choice using [GraphX](https://spark.apache.org/graphx/).
   - Visualize the results.

5. **Create a Customizable Dashboard:**
   - Develop a customizable dashboard to visualize dataset information and the results of graph algorithms.

6. **Spark ML:**
   - Use Spark ML to apply machine learning algorithms to the dataset.

## Docker-Compose Configuration
Use the provided `docker-compose.yml` file to set up the cluster. The included services are:
- Zeppelin (Apache Zeppelin 0.10.0)
- Spark Master (Bitnami Spark 3.1.2)
- Neo4j (Bitnami Neo4j 5)

Make sure to configure volumes and ports accordingly.

## Running the Project
### Clone the Repository
```bash
# Clone the repository from GitHub
git clone https://github.com/rmakaoui/Project_GraphX_SparkML_neo4j.git
cd Project_GraphX_SparkML_neo4j
```
### Download the Game of Thrones dataset and place it in the appropriate location.
- [Game of Thrones Dataset](https://www.kaggle.com/code/mmmarchetti/game-of-thrones-network-analysis/input)
![image](https://github.com/rmakaoui/Project_GraphX_SparkML_neo4j/assets/101502312/c4e8a6af-e5f6-44fa-acd4-d94a3080fff0)

### Start the Project with Docker Compose
```bash
# Make sure to be in the project directory
cd Project_GraphX_SparkML_neo4j

# Start the services in the background with Docker Compose
docker-compose up -d
```

After running these commands, the Docker services (Zeppelin, Spark Master, Neo4j) will start, and you can access Apache Zeppelin at [http://localhost:8080](http://localhost:8080) in your browser.

6. Follow the steps outlined in the guide for data analysis, graph algorithms, and machine learning.

## References
- [Game of Thrones Dataset](https://www.kaggle.com/code/mmmarchetti/game-of-thrones-network-analysis/input)
- [Neo4j Spark Connector Documentation](https://neo4j.com/docs/spark/current/)
- [GraphX Documentation](https://spark.apache.org/graphx/)
