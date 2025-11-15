# AI-Powered Task Management System

This project implements an AI-driven system designed to enhance traditional task management by incorporating **Priority Prediction**, **Forecasting**, **Workload Balancing**, and a comprehensive **Accuracy Dashboard**.

## Features

* **Priority Prediction:** Uses machine learning to automatically assign a priority (`Low`, `Medium`, `High`) to new tasks based on their text content.
* **Workload Balancing:** Analyzes current and forecasted load to suggest actions for balancing tasks among assigned users (e.g., `delegate_tasks` or `take_more_tasks`).
* **Task Forecasting:** Leverages Time Series models like **Prophet** and **ARIMA** (if available) to predict future task volume.
* **Model Accuracy Dashboard:** Visualizes the performance of the Task Completion (Status) and Priority Prediction models.

## Technologies

The project relies on a mix of machine learning and data science tools:

* **Core Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`
* **NLP/Feature Engineering:** **TF-IDF Vectorizer** for converting task text (`task_name`, `description`) into numerical features.
* **Machine Learning Models:** **RandomForestClassifier** (primary), with optional support for **XGBoost** for classification.
* **Forecasting Models:** **Prophet** and **ARIMA** from `statsmodels`.

## Files in this Repository

| File | Description |
| :--- | :--- |
| `Untitled39.ipynb` | The main Jupyter Notebook containing all the project logic, including data loading, preprocessing, feature engineering, model training, forecasting, and workload balancing logic. |
| `main` | A simplified Python script likely used to execute the core task management logic. |
| `synthetic_task_dataset.csv` | The sample dataset used for training and analysis, containing columns like `task_id`, `task_name`, `priority`, `status`, and `deadline`. |

## Getting Started

### Prerequisites

You will need Python 3 and the following major packages (some optional):

* `pandas`
* `scikit-learn`
* `matplotlib`
* `seaborn`
* `xgboost` (Optional)
* `statsmodels` (Optional)
* `prophet` (Optional)

### Running the System

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/munshid-mhd/ai-task-managment-system](https://github.com/munshid-mhd/ai-task-managment-system)
    cd ai-task-managment-system
    ```
2.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt # Assuming you have a requirements file
    # OR manually install the necessary libraries
    ```
3.  **Execute the Notebook:** Open and run the `Untitled39.ipynb` notebook in a Jupyter environment to execute the full pipeline, including data loading, model training, forecasting, and reporting.
