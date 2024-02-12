# Product Recommendation System using Apache Spark and Apache Hadoop

## Introduction

Recommendation systems are indispensable in modern business environments due to the abundance of customer data, reviews, and product variety. They automate the real-time delivery of personalized product recommendations tailored to specific user preferences. 

This project focuses on developing a recommendation system utilizing Apache Spark and Apache Hadoop. It leverages collaborative filtering techniques to generate recommendations based on user-item interactions. Specifically, the system implements Alternating Least Squares (ALS) algorithm on Apache Spark for fast real-time data processing.

## Related Work

Previous studies have addressed challenges such as cold start issues in collaborative filtering methods. Efforts have been made to introduce hybrid models, which combine collaborative and content-based filtering approaches, to mitigate these issues. Our project builds upon these efforts by implementing ALS on Spark for product recommendations. Additionally, matrix factorization techniques are incorporated into the ALS algorithm to mitigate overfitting issues commonly encountered in recommendation systems.

## Implementation and Results

The recommendation system is implemented using collaborative filtering techniques, specifically ALS algorithm, on Apache Spark. Two main methods are explored:

1. **Content-Based Filtering**: Recommends products based on user preferences and item features. It creates user profiles reflecting user preferences and suggests similar items based on past interactions. However, it heavily relies on historical data and may struggle with cold start issues.

2. **Collaborative Filtering**: Recommends products based on the preferences of similar users. It identifies neighborhoods of similar users and suggests items based on their preferences. Collaborative filtering can handle cold start issues effectively and tailors recommendations to users.

The project utilizes ALS algorithm for matrix factorization in collaborative filtering. ALS is an optimization technique to perform matrix factorization and is commonly used in recommendation systems. By tuning hyperparameters and incorporating matrix factorization techniques, the system achieves improved prediction accuracy and mitigates overfitting issues.

## Environment Setup

The recommendation system is deployed on Google Cloud Platform using Google Cloud Dataproc service. Dataproc simplifies the deployment and management of Apache Spark and Apache Hadoop clusters, allowing easy configuration and management of big data projects. 

A cluster with one master node and three worker nodes is created on Google Cloud to run the recommendation system. Dataproc enables easy monitoring of system resources, making it an ideal choice for our project.

## Conclusion

The recommendation system developed in this project utilizes Apache Spark for high-speed data processing. By leveraging collaborative filtering techniques and matrix factorization, it delivers personalized product recommendations in real-time. The system is structured based on lambda architecture, enabling real-time recommendation visibility for users. Future enhancements may include integrating advanced methods such as deep collaborative filtering and convolutional neural network-based recommendation approaches.

## Contributions

- **Report Contributions**:
  - Introduction, Related Work, and Conclusion: Phanendra
  - Implementation and Results: Jaswanth
  - Conclusion and References: Abdul
- **Code Contributions**: Jaswanth, Phanendra, and Abdul

