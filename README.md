# transportaion-of-cyanobacteria-and-cyano-toxins
# Cyanobacteria Forecasting Pipeline

## Project Overview

This project develops a robust data pipeline and machine learning models to **forecast cyanobacteria and cyanotoxins in the Raritan River Basin**. By analyzing historical environmental data from sources like USGS, this pipeline provides predictive insights into water quality, enabling proactive management and early warning systems. The goal is to enhance environmental monitoring and support data-driven decision-making for public health and ecological preservation.

This initiative moves beyond simple data collection to deliver actionable intelligence, optimizing existing algorithms for efficiency and performance on large-scale environmental datasets.

## Features

* **Automated Data Collection & Transformation:** Fetches, cleans, and transforms raw environmental time-series data (e.g., from USGS).
* **Machine Learning Forecasting:** Trains and evaluates multiple ML models (LSTM, Prophet, XGBoost) for accurate time-series predictions of cyanobacteria levels.
* **Feature Importance Analysis:** Identifies key environmental variables influencing cyanobacteria growth, providing actionable insights.
* **Performance Optimization:** Optimizes data processing and model inference for efficiency on large datasets.
* **Predictive Insights:** Generates actionable forecasts for environmental monitoring and public health.

## Technologies Used

* **Programming Language:** Python
* **Machine Learning Frameworks:** scikit-learn, TensorFlow / Keras (for LSTM), Prophet (Facebook's forecasting library), XGBoost
* **Data Manipulation:** Pandas, NumPy
* **Data Sources:** USGS (example)
* **Version Control:** Git

## How to Run Locally

Follow these steps to set up and run the Cyanobacteria Forecasting Pipeline on your local machine.

### Prerequisites

* Python 3.8+
* Git

### Setup Instructions

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Swetha-Kambham/cyanobacteria-forecasting-pipeline.git](https://github.com/Swetha-Kambham/cyanobacteria-forecasting-pipeline.git)
    cd cyanobacteria-forecasting-pipeline
    ```
2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    # On macOS/Linux:
    source venv/bin/activate
    # On Windows:
    .\venv\Scripts\activate
    ```
3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    *(Note: `requirements.txt` should contain all necessary libraries like `pandas`, `numpy`, `scikit-learn`, `tensorflow`, `prophet`, `xgboost`)*

### Running the Pipeline

1.  **Configure Data Sources:**
    * Ensure your data collection scripts (if external to the repo) are set up to pull data into the expected format/location.
    * *(If `data_collection.py` exists):* Run the data collection script:
        ```bash
        python data_collection.py
        ```
2.  **Execute the Forecasting Pipeline:**
    ```bash
    python main_forecasting_pipeline.py
    ```
    *(Note: Replace `main_forecasting_pipeline.py` with the actual name of your main script that runs the data processing, model training, and forecasting.)*

This script will perform data loading, cleaning, model training, and generate forecasts. Results (e.g., forecast plots, performance metrics) will be saved to a designated `output/` directory.

## Project Structure (Example)
