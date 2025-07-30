# Movie Recommender System

This repository contains code and notebooks for exploratory data analysis (EDA), preprocessing, and feature engineering on the [MovieLens 10M dataset](https://grouplens.org/datasets/movielens/10m/). The goal is to build a foundation for developing and evaluating movie recommendation algorithms.


## Project Goals

- ✅ Parse MovieLens 10M data (ratings, movies, genres).
- ✅ Simulate a basic non-contextual bandit environment.
- 🧠 Implement contextual bandits (e.g., LinUCB, Thompson Sampling).
- 🔬 Integrate neural bandits for advanced exploration-exploitation tradeoffs.
- 📊 Evaluate and visualize performance (e.g., cumulative reward).


## Project Structure

```
movie-recommender/
├── data/                  # MovieLens datasets (not tracked by git)
├── notebooks/             # Jupyter notebooks for EDA and preprocessing
├── .gitignore
├── environment.yml        # Conda environment specification
└── README.md
```

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/wayneotemah/movie-recommender.git
cd movie-recommender
```

### 2. Download the Data

Download the MovieLens 10M dataset from [GroupLens](https://grouplens.org/datasets/movielens/10m/) and extract it into the `data/ml-10M100K/` directory.

### 3. Set Up the Conda Environment

Create the environment using the provided `environment.yml`:

```bash
conda env create -f environment.yml
conda activate movie-recommender
```

If you don't have an `environment.yml`, you can create one with the following content:

```yaml
name: movie-recommender
channels:
  - defaults
  - conda-forge
dependencies:
  - python=3.10
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - jupyter
  - notebook
  - scikit-learn
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

Open and run the notebooks in the `notebooks/` directory.

## Notebooks

- **01_eda_and_preprocessing.ipynb**: Exploratory data analysis and preprocessing steps for the MovieLens dataset.

## Notes

- The `data/` directory is excluded from version control via `.gitignore`.
- All code is written for Python 3.10+ and tested on Linux.
- Visualizations are created using Matplotlib and Seaborn.

## License

This project is for research and educational purposes only. Please see the [MovieLens license](https://grouplens.org/datasets/movielens/) for dataset usage terms.

---

**Author:** Wenslous Otema Egesa
**Contact:** wayneotemahegesa@gmail.com