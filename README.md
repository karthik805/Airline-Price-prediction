# Flight Price Prediction Application

## Overview

This application predicts flight prices using machine learning techniques. It involves data preprocessing, feature engineering, exploratory data analysis (EDA), and model training. The project utilizes various libraries and tools to analyze flight data and build a prediction model.

## Tools and Libraries

- **Python**: The primary programming language used for this project.
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical computations.
- **Matplotlib & Seaborn**: For data visualization.
- **Scikit-learn**: For machine learning algorithms and preprocessing.
- **XlsxWriter & Openpyxl**: For Excel file handling.
- **ydata_profiling**: For generating EDA reports.
- **Cufflinks & Chart Studio**: For interactive visualizations.
- **Django**: For building RESTful APIs (optional, if using for deployment).
- **Flask**: For serving the model (if applicable).

## Getting Started

### Prerequisites

- Python 3.x
- Pip (Python package installer)

### Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/flight-price-prediction.git
cd flight-price-prediction
```

Install the required packages:

```bash
pip install -r requirements.txt
```

### Files

- `Data_Train.xlsx`: Training dataset.
- `Test_set.xlsx`: Test dataset.
- `data_handling.py`: Script for loading and saving datasets.
- `preprocessing.py`: Contains custom data transformers for preprocessing.
- `training_pipeline.py`: Script for training the model.
- `predict.py`: Script for generating predictions using the trained model.
- `config.py`: Configuration settings for file paths and model parameters.
- `version`: File indicating the model version.

### Data Preparation

1. **Load Data**: Read the training and test datasets using Pandas.
2. **Handle Missing Values**: Remove or impute missing values.
3. **Feature Engineering**:
    - Convert date columns to datetime format.
    - Extract features like day and month from dates.
    - Split and transform time and duration columns.
4. **Categorical Encoding**: Apply One-Hot Encoding to categorical variables.

### Exploratory Data Analysis (EDA)

1. **Generate EDA Report**: Use `ydata_profiling` to generate an automated EDA report.
2. **Visualizations**: Use Matplotlib, Seaborn, and Cufflinks to create various plots:
   - Distribution of flight prices.
   - Price analysis based on airlines, stops, source, and destination.
   - Correlation heatmap.

### Model Training

1. **Preprocessing**: Apply preprocessing steps using `preprocessing.py`.
2. **Model Training**: Fit the model using the training dataset in `training_pipeline.py`.
3. **Save Model**: Save the trained model using `data_handling.py`.

### Prediction

1. **Load Model**: Load the trained model using `predict.py`.
2. **Make Predictions**: Apply the model to the test dataset and generate predictions.

### Running the Application

To train the model, run:

```bash
python training_pipeline.py
```

To generate predictions, run:

```bash
python predict.py
```

### Notes

- Ensure that the dataset paths in `config.py` are correctly set.
- Update the version file (`version`) when making changes to the model.

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Contact

For any questions or issues, please contact:

- **Name**: B.S Karthik 
- **Email**: karthik.uk@outlook.in
