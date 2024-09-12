# FitChart-Pro
# Size Chart Generator for Apparel Sellers

This project aims to generate accurate size charts for apparel sellers based on user body measurements, previous purchase history, and return/exchange data. The goal is to help sellers reduce size-related returns and exchanges by offering size recommendations with high confidence.

## Problem Overview

Apparel sellers often face the challenge of providing accurate size charts, especially when limited or inaccurate size data is available. This model solves the problem by:

- Utilizing a database of user body measurements (e.g., height, weight, chest, waist, hip).
- Analyzing users’ previous purchase history and return/exchange data.
- Clustering similar body types and associating them with successful purchases.
- Generating a comprehensive size chart (S, M, L, XL, etc.) with confidence scores for each measurement.
- Adapting to new data as it becomes available.

## Solution

This project uses **Random Forest** to predict the most accurate size recommendations based on the body measurements and historical purchase data. The model was trained and tested to improve size predictions, helping reduce returns and exchanges for sellers.

## Features

- **User Data Analysis:** Body measurements and previous purchase history are analyzed.
- **Size Clustering:** Users with similar body types are grouped to identify successful size purchases.
- **Dynamic Size Chart Generation:** A comprehensive size chart for each apparel item is generated.
- **Confidence Scores:** Each recommended size comes with confidence scores based on historical data.
- **Scalability:** The model is easily adaptable to new data from different brands or product lines.
- **Real-Time Updates:** Size charts are updated dynamically as more purchase data becomes available.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/size-chart-generator.git
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the model:
    ```bash
    python main.py
    ```

## Dataset

The project uses a dataset of body measurements and purchase history. You can modify the dataset to fit the needs of different apparel categories, such as tops, bottoms, and dresses.

## Model

The Random Forest algorithm is used for clustering users and predicting sizes. You can view the model code and configuration in `model.py`.

## Usage

1. Input user body measurements into the system.
2. Use historical purchase and return/exchange data to predict the most suitable size.
3. The model outputs a size recommendation along with confidence scores for each category (e.g., S, M, L, XL).

## Future Improvements

- Implementing deep learning models like Neural Networks for more accuracy.
- Introducing support for real-time size recommendations.
- Adding more categories like shoes or accessories.

## Link to the Project

You can access the complete project solution [here]((https://colab.research.google.com/drive/10fC9aqtSLEtKlk0LofRcfJ2C81oMUT1c?usp=sharing)).

## Judging Criteria

- **Accuracy:** Comparison of generated size charts with brands having known accurate data.
- **Category Handling:** Effective for different apparel categories (tops, bottoms, dresses, etc.).
- **Return Reduction:** Model's performance in reducing returns and exchanges.
- **Scalability:** Easy adaptability for new brands or product lines.
- **Efficiency:** Quick processing speed for generating and updating size charts.
