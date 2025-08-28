# Sonar Detection

This project uses machine learning to classify sonar signals as either "Rock" (R) or "Mine" (M) using a logistic regression model.

## Files
- `core/Train.ipynb`: Jupyter notebook containing the data loading, preprocessing, model training, and evaluation steps.
- `core/sonar_data.csv`: Dataset containing sonar signal readings and their corresponding labels.
- `requirments.txt`: List of required Python packages.

## Getting Started
1. **Install dependencies**
   ```bash
   pip install -r requirments.txt
   ```
2. **Run the notebook**
   - Open `core/Train.ipynb` in Jupyter Notebook or JupyterLab.
   - Follow the cells to load data, preprocess, train, and evaluate the model.

## Usage
- The notebook demonstrates:
  - Loading the sonar dataset
  - Splitting data into training and test sets
  - Training a logistic regression model
  - Evaluating model accuracy
  - Making predictions on new input data

## Example Prediction
To predict with new data:
```python
input_data = (0.0203, 0.0121, ..., 0.0016)  # 60 features
# Convert to numpy array and reshape for prediction
input_data_np = np.array(input_data).reshape(1, -1)
prediction = model.predict(input_data_np)
```

## License
This project is for educational purposes.