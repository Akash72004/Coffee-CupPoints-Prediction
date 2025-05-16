# Introduction
This project aims to solve a real-world problem for coffee buyers, café owners, and producers by providing a data-driven way to assess coffee quality. In the specialty coffee industry, pricing and perception heavily depend on a score known as the Total Cup Points. This score, usually out of 100, is a professional rating that combines multiple sensory attributes like aroma, flavor, sweetness, acidity, and aftertaste. By predicting this score using machine learning, the project helps users make informed decisions about which coffee to buy, sell, or serve.

# Dataset and Features
The dataset used in this project contains information on Arabica coffee beans, sourced from professional grading reports. Key features include Aroma, Flavor, Aftertaste, Sweetness, Acidity, Category, Harvest Year, and others, all of which contribute to the Total Cup Points. This diverse set of attributes offers a rich ground for building a predictive model capable of learning how different factors influence perceived coffee quality.

# Objective
The objective of the project was to develop a machine learning model that can predict the Total Cup Points of coffee samples based on measurable characteristics. The process involved several stages—data cleaning, feature engineering, exploratory analysis, model training, and evaluation. Beyond model accuracy, the goal was also to make the solution practically usable through a real-time deployment interface.

# Model Building and Evaluation
Multiple regression models were developed and tested using Scikit-learn, including Linear Regression, Ridge Regression, Random Forest Regressor, and Gradient Boosting Regressor. The models were evaluated using Mean Absolute Error (MAE) and standard deviation via cross-validation to ensure robust performance. While Linear and Ridge Regression both performed well, Ridge Regression was selected due to its optimal trade-off between accuracy and generalization, showing the lowest MAE with consistent results across folds.
![Image](https://github.com/user-attachments/assets/57c1ff5a-0243-4144-964c-e6e96c965c54)

# Deployment with Flask
To make the model accessible and user-friendly, the final Ridge Regression model was deployed using Flask, a lightweight Python web framework. The backend was connected to a simple React-based frontend, where users can input features like aroma, flavor, and harvest year, and receive a real-time prediction of the coffee's Total Cup Points. This real-time prediction tool turns the machine learning model into a practical asset for business use.

![Image](https://github.com/user-attachments/assets/f6d77d60-e4ed-4714-9b04-dca1fe173ec4)

# Real-World Applications
This project can be particularly useful for several user groups. Coffee buyers can use the tool to assess bean quality before purchasing. Café owners can forecast how a particular bean might perform in terms of customer satisfaction and pricing. Producers and growers can experiment with changes in growing practices—such as improving sweetness or harvest timing—to see how these affect the predicted cup score. In essence, the project bridges data science and consumer experience in the coffee industry.
