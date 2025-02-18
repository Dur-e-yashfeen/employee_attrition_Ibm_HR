# Employee Attrition Analysis

## Overview
This repository contains data, code, and reports related to the analysis of employee attrition. The goal of this project is to understand the factors that contribute to employee attrition and to build predictive models to identify employees who are at risk of leaving the company.

## Repository Structure
The repository is organized into the following directories:

- `datasets/`: Contains the datasets used for the analysis.
- `notebooks/`: Contains Jupyter notebooks with the data analysis and model building steps.
- `scripts/`: Contains Python scripts used for data processing and analysis.
- `reports/`: Contains reports and visualizations generated from the analysis.

## Files
- `datasets/employee_attrition.csv`: The main dataset used for the analysis.
- `notebooks/EDA.ipynb`: Jupyter notebook with exploratory data analysis (EDA).
- `notebooks/Model_Building.ipynb`: Jupyter notebook with model building and evaluation steps.
- `scripts/data_processing.py`: Python script for data cleaning and preprocessing.
- `scripts/train_model.py`: Python script for training the predictive model.
- `reports/Attrition_Report.pdf`: Final report summarizing the findings and results of the analysis.

## Getting Started

### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook
- Required Python packages (listed in `requirements.txt`)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your_username/employee-attrition.git
   cd employee-attrition
   ```

2. Create a virtual environment and activate it:
   ```bash
   python3 -m venv env
   source env/bin/activate  # On Windows, use `env\Scripts\activate`
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

### Usage
1. To perform exploratory data analysis, open `notebooks/EDA.ipynb` in Jupyter Notebook and run the cells.
2. To build and evaluate the predictive model, open `notebooks/Model_Building.ipynb` in Jupyter Notebook and run the cells.
3. To generate the final report, run the `scripts/train_model.py` script and refer to the `reports/Attrition_Report.pdf`.

## Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments
- The dataset used in this project is sourced from [Kaggle](https://www.kaggle.com/).
- Special thanks to the data science community for their valuable resources and contributions.
