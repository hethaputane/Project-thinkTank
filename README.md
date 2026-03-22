# Big Data Movie Analysis (TMDB + IMDb)

## Overview
This project analyses a large-scale real-world dataset, “The Ultimate 1 Million Movies Dataset (TMDB + IMDb)”, containing approximately 989,000 movies (~720 MB). The aim is to compare traditional data processing using Pandas with distributed computing using Spark RDD (MapReduce).

## Objective
To analyse large-scale movie data using both Pandas and Spark RDD (MapReduce) in order to evaluate performance, scalability, and efficiency across different analytical tasks.

## Dataset
- Source: Kaggle  
- Size: ~720 MB  
- Records: ~989,000 movies  
- Attributes include:
  - Numerical: budget, revenue, popularity  
  - Categorical: genres, production companies  
  - Temporal: release dates  

The dataset demonstrates key big data characteristics:
- Volume: Large size leading to computationally expensive operations  
- Variety: Multiple data types requiring preprocessing  
- Velocity: Continuously updated dataset  

## Technologies Used
- Python  
- Pandas  
- Apache Spark (RDD API)  
- PySpark  
- Jupyter Notebook  

## System Specifications
- Local machine  
- 8GB RAM  
- Multi-core CPU  
- Spark running in local mode  

## Project Structure
The project is divided into eight components:
1. Data Preparation  
2. Genre Popularity Trends  
3. Financial Performance Analysis  
4. Trend and Shift Detection  
5. Genre–Box Office Analysis  
6. Multidimensional Analysis  
7. Validation and Benchmarking  
8. Directors/Cast Consistency  

Each team member completed two components.

## Methodology
- Data cleaning and preprocessing using Pandas  
- Queries implemented using:
  - Pandas (baseline)
  - Spark RDD (MapReduce model)  
- Performance evaluated based on execution time, memory usage, and scalability  

## Key Results
- Cast Genre Specialization: 42.85s → 7.59s (~5.6× faster)  
- Hit Probability: 2.88s → 1.09s (~2.6× faster)  
- Spark shows strong advantages for aggregation-heavy tasks  

## Key Insights
- Genre profitability varies significantly  
- Strong collaboration patterns exist between directors and cast  
- Popularity trends differ across genres and time  

## How to Run
1. Install dependencies:
   pip install pandas pyspark

2. Start Spark:
   from pyspark.sql import SparkSession
   spark = SparkSession.builder.master("local[*]").getOrCreate()

3. Run the provided scripts or notebooks  

## Repository
(https://github.com/hethaputane/Project-thinkTank)

## Authors
- Your Name  
- Teammate Names  

## License
This project is for academic purposes.
