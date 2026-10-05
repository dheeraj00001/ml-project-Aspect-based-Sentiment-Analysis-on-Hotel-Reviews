# Aspect-Based Sentiment Analysis on Hotel Reviews

## Setup and Running the Project

### 1. Clone the Repository

```bash
git clone https://github.com/dheeraj00001/ml-project-Aspect-based-Sentiment-Analysis-on-Hotel-Reviews
cd <REPOSITORY_FOLDER>
```

### 2. Install the Required Python Packages

Install the required dependencies using pip:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn lightgbm torch transformers jupyter
```

### 3. Project Structure

Make sure the repository contains the following files:

```text
.
├── main.ipynb
├── train_aspects.csv
├── dev_aspects.csv
├── test_aspects.csv
├── README.md
```

The CSV files are already included in the repository and are loaded directly by `main.ipynb`.

### 4. Run Using Google Colab

Google Colab is recommended for running the notebook, especially for the transformer-based models.

1. Open `main.ipynb` in Google Colab.
2. If available, select a GPU runtime:

   **Runtime → Change runtime type → T4 GPU**
3. Make sure `train_aspects.csv`, `dev_aspects.csv`, and `test_aspects.csv` are available in the same working directory as the notebook.
4. Run the notebook cells from top to bottom.

The notebook performs the complete workflow, including data loading, preprocessing, model training, evaluation, model comparison, and sentiment prediction.

### 5. Run Locally Using Jupyter Notebook

From the project directory, start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
main.ipynb
```

Then run the notebook cells sequentially from top to bottom.

A GPU is recommended for the DistilBERT and OpenJEV-0.8B sections.

### 6. Dataset Files

The project uses three pre-split CSV files:

- `train_aspects.csv` — training data
- `dev_aspects.csv` — development/validation data
- `test_aspects.csv` — held-out test data

No separate dataset download is required because the datasets are included in the repository.

### 7. Expected Output

Running `main.ipynb` produces:

- Data inspection and exploratory analysis
- Classical machine-learning model results
- DistilBERT training and evaluation results
- OpenJEV-0.8B zero-shot evaluation results
- Test-set performance metrics
- Model comparison
- Visualizations such as evaluation plots/confusion matrices
- Sentiment predictions for hotel-review examples

### 8. Notes

- Run the notebook cells in order because later cells depend on variables and models created earlier.
- Internet access may be required when loading pretrained transformer models for the first time.
- GPU execution is recommended for transformer-based sections to reduce runtime.
