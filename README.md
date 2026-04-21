<h1 align="center">Court Judgments Prediction using Machine Learning</h1>

<p align="center"><i>Supreme Court of Nigeria (SCN) appeal-case outcome prediction with interpretable ML workflows.</i></p>

<p align="center">
	<img src="https://img.shields.io/badge/VERSION-1.0.0-E11D48?style=for-the-badge&logo=semanticrelease&logoColor=white&labelColor=7F1D1D" alt="Version 1.0.0" />
	<img src="https://img.shields.io/badge/LICENSE-MIT-84CC16?style=for-the-badge&logo=opensourceinitiative&logoColor=white&labelColor=14532D" alt="MIT License" />
	<img src="https://img.shields.io/badge/TYPE-MACHINE%20LEARNING-8B5CF6?style=for-the-badge&labelColor=4C1D95" alt="Machine learning project" />
</p>

<p align="center">
	<img src="https://img.shields.io/badge/PYTHON-3.x-14B8A6?style=for-the-badge&logo=python&logoColor=white&labelColor=0F766E" alt="Python" />
	<img src="https://img.shields.io/badge/PANDAS-DATA-06B6D4?style=for-the-badge&logo=pandas&logoColor=white&labelColor=155E75" alt="Pandas" />
	<img src="https://img.shields.io/badge/NUMPY-ARRAYS-3B82F6?style=for-the-badge&logo=numpy&logoColor=white&labelColor=1E3A8A" alt="NumPy" />
	<img src="https://img.shields.io/badge/SCIKIT--LEARN-MODELING-6366F1?style=for-the-badge&logo=scikitlearn&logoColor=white&labelColor=4338CA" alt="Scikit-learn" />
	<img src="https://img.shields.io/badge/SEABORN-VISUALS-0EA5E9?style=for-the-badge&logo=plotly&logoColor=white&labelColor=1E40AF" alt="Seaborn" />
	<img src="https://img.shields.io/badge/JUPYTER-NOTEBOOK-A855F7?style=for-the-badge&logo=jupyter&logoColor=white&labelColor=6D28D9" alt="Jupyter Notebook" />
</p>

<p align="center">
	<a href="#-project-intro"><img src="https://img.shields.io/badge/EXPLORE-PROJECT%20INTRO-6366F1?style=for-the-badge&logo=gitbook&logoColor=white&labelColor=4F46E5" alt="Project intro" /></a>
	<a href="#-project-structure"><img src="https://img.shields.io/badge/VIEW-STRUCTURE-14B8A6?style=for-the-badge&logo=readme&logoColor=white&labelColor=0F766E" alt="Project structure" /></a>
	<a href="#-how-to-run"><img src="https://img.shields.io/badge/RUN-NOTEBOOK-A855F7?style=for-the-badge&logo=jupyter&logoColor=white&labelColor=7E22CE" alt="Run notebook" /></a>
</p>

## Court Judgments Prediction — README

This project predicts judicial outcomes for Supreme Court of Nigeria appeal cases using supervised machine learning models and compares their performance with visual diagnostics and confusion matrices.

## Table of Contents

- [🚀 Project intro](#-project-intro)
- [📁 Project structure](#-project-structure)
- [📊 Dataset](#-dataset)
- [🧠 Modeling approach](#-modeling-approach)
- [🤖 Models evaluated](#-models-evaluated)
- [📈 Outputs and artifacts](#-outputs-and-artifacts)
- [⚙️ How to run](#️-how-to-run)
- [📄 License](#-license)

## 🚀 Project intro

The repository demonstrates an end-to-end ML workflow for legal outcome prediction:

- Data profiling and exploratory analysis of SCN appeal data
- Feature engineering and preprocessing (including encoding/scaling)
- Training and comparison of multiple classification algorithms
- Performance reporting with confusion matrices and plots

## 📁 Project structure

```txt
Court-Judgments-Prediction-using-Machine-Learning/
├── CSE 445.ipynb
├── scn_appeal_cases_data.csv
├── datasetprofiling.html
├── Dataset description.pdf
├── IMAGES/
│   ├── Confusion Matrix for LogisticRegression().png
│   ├── Confusion Matrix for SVC().png
│   ├── Feature_corelation_rc_heatmap_plot.png
│   └── ...
├── LICENSE
└── README.md
```

## 📊 Dataset

- **Source:** Primsol Law Pavilion archive (distributed via Mendeley)
- **Records:** 5,585 appeal cases
- **Scope:** Criminal and civil appeal matters from the Supreme Court of Nigeria
- **Dataset link:** https://data.mendeley.com/datasets/ky6zfyf669/1

## 🧠 Modeling approach

The notebook performs:

- Data cleaning and exploratory visual analysis
- Feature transformation with `LabelEncoder` and scaling tools where required
- Train/test split and model training
- Evaluation using accuracy metrics, classification reports, and confusion matrices

## 🤖 Models evaluated

Primary and baseline models included in the notebook:

- `DummyClassifier`
- `DecisionTreeClassifier`
- `KNeighborsClassifier`
- `LogisticRegression`
- `SVC` / `OneVsRestClassifier`
- `GaussianNB`
- `MLPClassifier`
- `SGDClassifier`
- Additional ensemble experiments (`AdaBoost`, `Bagging`, `RandomForest`, etc.)

## 📈 Outputs and artifacts

- `datasetprofiling.html` contains automated dataset profiling
- `IMAGES/` contains confusion matrices and EDA plots
- `CSE 445.ipynb` contains the full workflow and model comparisons

## ⚙️ How to run

1. Install Python 3 and Jupyter.
2. Install dependencies used in the notebook:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn pandas-profiling jupyter
```

3. Open and run:

```bash
jupyter notebook "CSE 445.ipynb"
```

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.
