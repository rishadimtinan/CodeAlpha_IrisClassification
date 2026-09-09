# Iris Flower Classification 

This is my first project for the CodeAlpha Data Science Internship. The goal was pretty simple on paper — build a model that can look at a flower's measurements and figure out which of the three Iris species it belongs to (Setosa, Versicolor, or Virginica). But it turned out to be a great way to actually get hands-on with the full ML workflow, from raw data to a working model.

## What's in this project

I used the classic Iris dataset (150 samples, 4 features: sepal length, sepal width, petal length, petal width) and walked through it step by step:

- **Explored the data** — checked for missing values, looked at the distribution of each species (turns out it's perfectly balanced, 50 samples each)
- **Visualized it** — plotted Petal Length vs Petal Width, which honestly told me most of what I needed to know before even training anything. Setosa is completely separate from the other two, while Versicolor and Virginica overlap a little
- **Split the data** — 80% for training, 20% for testing
- **Trained a model** — went with K-Nearest Neighbors (KNN) since it's simple and works really well on a dataset like this
- **Evaluated it** — accuracy, precision, recall, f1-score, and a confusion matrix to see exactly where (if anywhere) it was getting confused

## Results

The model hit **100% accuracy** on the test set — all 30 test samples classified correctly, no mix-ups at all. That's not too surprising once you see the scatter plot; the petal measurements alone make the species pretty easy to tell apart.

## Tools used

- Python
- Pandas & NumPy
- Matplotlib & Seaborn (for visualization)
- Scikit-learn (for the model and evaluation metrics)

## Files

- `Task1.ipynb` — the full notebook with code, plots, and results
- `Iris.csv` — the dataset

## A quick note

This was done as part of the CodeAlpha Data Science Internship. It's a small, clean dataset, so getting perfect accuracy here isn't a huge feat by itself — but the point was to practice the full pipeline: cleaning data, exploring it visually, training a model, and actually evaluating whether it did a good job. That process is the real takeaway.
