# College Data K-Means Clustering Project

## Project Description

This project implements the K-Means Clustering algorithm using the College Data dataset. The objective is to group colleges into two clusters and compare the generated clusters with the actual college type (Private or Public).

The project includes exploratory data analysis, data cleaning, clustering using K-Means, and evaluation of the clustering results.

---

## Dataset

Dataset: `College_Data`

Target Variable (used only for evaluation):

* `Private`

Features include various college characteristics such as:

* Apps
* Accept
* Enroll
* Top10perc
* Top25perc
* F.Undergrad
* P.Undergrad
* Outstate
* Room.Board
* Books
* Personal
* PhD
* Terminal
* S.F.Ratio
* perc.alumni
* Expend
* Grad.Rate

---

## Project Workflow

### Exploratory Data Analysis (EDA)

The notebook includes:

* Dataset overview using `head()`
* Dataset information using `info()`
* Statistical summary using `describe()`
* Scatter plot:

  * Room.Board vs Grad.Rate
  * Colored by Private
* Scatter plot:

  * Outstate vs F.Undergrad
  * Colored by Private
* Histogram of Outstate based on Private colleges
* Histogram of Grad.Rate based on Private colleges

---

## Data Cleaning

The notebook identifies colleges with a graduation rate greater than 100%.

The incorrect value is corrected by setting:

* `Grad.Rate = 100`

---

## Machine Learning Model

Algorithm:

* K-Means Clustering

Parameters:

* Number of Clusters = 2

Steps:

1. Remove unnecessary columns.
2. Prepare the feature matrix.
3. Train the K-Means clustering model.
4. Generate cluster labels.

---

## Model Evaluation

To compare the generated clusters with the actual college categories:

* Converted the `Private` column into numerical labels.

* Evaluated the clustering results using:

* Confusion Matrix

* Classification Report

---

## Concepts Used

* Exploratory Data Analysis (EDA)
* Scatter Plots
* Histograms
* Data Cleaning
* Unsupervised Learning
* K-Means Clustering
* Cluster Centers
* Confusion Matrix
* Classification Report

---

## Project Structure

```text
K-Means-Clustering-Project/
│
├── 02-K Means Clustering Project.ipynb
├── College_Data
└── README.md
```

---

## Requirements

* Python 3.x
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## How to Run

1. Clone this repository.
2. Place the `College_Data` dataset in the project folder.
3. Open `02-K Means Clustering Project.ipynb`.
4. Run all cells from top to bottom.

---

## Author

Meet Tailor — Data Science Learner

GitHub: https://github.com/MeetTailor-Data

---

## License

Created for learning and educational purposes only.
