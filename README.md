# Machine Learning Experiments: Engine Condition & Predictive Maintenance

This repository collects machine-learning experiments and supporting datasets for exploring engine-condition classification and predictive maintenance. It includes a Jupyter notebook, CSV data, a Random Forest spreadsheet, and a Power BI report.

## What's included
- `AutomotiveEngine.ipynb` — notebook experiments training and evaluating Random Forest classifiers on engine sensor readings.
- `engine_data.csv` — engine sensor dataset used by the notebook.
- `predictive-maintenance-dataset.csv` — additional predictive-maintenance data for analysis.
- `RandomForest.xlsx` — spreadsheet associated with the Random Forest work.
- `Charts.pbix` — Power BI report for interactive data exploration.

## Notebook workflow
The notebook loads the engine CSV with pandas, removes rows containing missing values, and uses sensor measurements such as engine RPM, lubricant pressure, fuel pressure, coolant pressure and temperatures as model inputs. The target is the `Engine Condition` column. It demonstrates train/test evaluation and comparisons across Random Forest configurations, with accuracy and cross-validation calculations.

## Requirements
- Python 3.9+ recommended
- Jupyter Notebook or JupyterLab
- pandas
- scikit-learn
- A compatible Power BI Desktop installation to open `Charts.pbix`

## Run the notebook
```bash
git clone https://github.com/Saikabilane/ML_model.git
cd ML_model
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux: source .venv/bin/activate
python -m pip install pandas scikit-learn notebook
jupyter notebook AutomotiveEngine.ipynb
```

Run the cells from top to bottom. Keep the CSV files in the repository root, or update the notebook's paths if you move them.

## Interpreting results
Model accuracy depends on the dataset, preprocessing, feature selection and train/test split. Results in the notebook are experimental and should not be treated as validated real-world maintenance predictions without further testing, leakage checks and evaluation on representative data.

## License
No license file is currently included; contact the repository owner for reuse permission.
