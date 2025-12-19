# Student Performance Prediction and Learning Behavior Analysis

A machine learning project that predicts student outcomes and analyzes learning behaviors using the Open University Learning Analytics Dataset (OULAD).

## Project Description

This project addresses two primary objectives using machine learning and data mining techniques:

**1. Predictive Modeling**  
We developed classification models to predict student outcomes (Pass/Distinction versus Fail/Withdrawn) based on demographic information, assessment performance, and virtual learning environment engagement data. The XGBoost classifier achieved 91.98% accuracy with 95.45% recall in identifying at-risk students.

**2. Behavioral Analysis**  
We analyzed learning behavior patterns to understand:
- The effectiveness of cramming versus distributed study practices
- Student performance trajectories over time, including comeback and burnout patterns
- Behavioral combinations associated with academic success or failure using association rule mining

The analysis combines data from 32,593 students across 22 course modules, including over 10 million clickstream events and 173,912 assessment submissions.

## Dataset

**Source:** Open University Learning Analytics Dataset (OULAD)

The dataset files are not included in this repository due to size constraints (467 MB total).

### Download Instructions

1. Visit the official OULAD website: https://analyse.kmi.open.ac.uk/open_dataset

2. Download these four CSV files:
   - studentInfo.csv (3.3 MB)
   - studentAssessment.csv (5.4 MB)
   - studentRegistration.csv (1.1 MB)
   - studentVle.csv (432.8 MB)

3. Place all files in the `data/raw/` directory of this repository

### Citation
```
Kuzilek, J., Hlosta, M., & Zdrahal, Z. (2017).
Open University Learning Analytics dataset.
Scientific Data, 4, 170171.
https://doi.org/10.1038/sdata.2017.171
```

## How to Run the Project

### Prerequisites

- Python 3.8 or higher
- Jupyter Notebook

### Installation Steps

1. Clone this repository:
```bash
git clone https://github.com/OULAD-Analysis/Student-Learning-Patterns-OULAD.git
cd Student-Learning-Patterns-OULAD
```

2. Install required Python packages:
```bash
pip install -r requirements.txt
```

3. Download the dataset files from the official OULAD website (see Dataset section above)

4. Place all four CSV files in the `data/raw/` directory

5. Launch Jupyter Notebook:
```bash
jupyter notebook
```

6. Open and run `notebooks/01_complete_analysis.ipynb`

7. Execute all cells sequentially from top to bottom

### Expected Runtime

The complete notebook takes approximately 15-20 minutes to run, depending on your system specifications. The longest processing time occurs during the clickstream data analysis due to the large file size.

### Output Files

After running the notebook, you will find generated files in:
- `outputs/figures/` - Visualizations and charts
- `outputs/models/` - Trained machine learning models
- `data/processed/` - Intermediate processed datasets

## Additional Documentation

- **Complete Report:** See `reports/Final_Report.pdf` for detailed methodology and findings


## License

MIT License

## Contact

For questions or issues, contact: Ilayaraj Rajmohan (irajmohan@binghamton.edu)

---

