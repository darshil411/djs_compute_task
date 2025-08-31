# UFC Fighters Data Analysis (EDA)

This project explores a dataset of **UFC fighters** and their statistics.  
The goal was to **clean the data, handle missing values & outliers, and perform Exploratory Data Analysis (EDA)** using Python libraries like **NumPy, Pandas, Matplotlib, and Seaborn**.

---
##  Dataset

This analysis uses the **UFC Fighters' Statistics** dataset from **Kaggle**:  
[https://www.kaggle.com/datasets/aaronfriasr/ufc-fighters-statistics/data](https://www.kaggle.com/datasets/aaronfriasr/ufc-fighters-statistics/data)

## 🗂️ Steps Performed

### 1. Data Cleaning
- Checked for **duplicates** → none found.  
- Converted **stance** into categories and fixed **dob** format.  
- Filled missing **weight** values with the **median**.  
- Created **weight categories** (40 -60kg,60-90kg ,90-120kg , etc.).  
- Filled missing **height** and **reach** using the **median of weight categories**.  
- Found extreme outlier (**249kg**) → capped to **200kg** (still high but realistic).  
- Separated **new players** with only physical attributes (no performance stats).  

### 2. Exploratory Data Analysis
- **Histograms** → numeric columns skewed towards 0 (many new players).  
- **Heatmap** → confirmed **height & reach depend on weight**.  
- **Barplots**:  
  - Submission attempts vs weight category → **60–90kg fighters** attempted the most.  
  - Wins vs weight category → **40–60kg fighters** won the most, followed by 60–90kg.  
- **Fighting Style (strike/takedown ratio)** → **Strikers performed better than grapplers**.  
- **Age vs Wins (scatterplot)** → no clear trend; most clustered around ~50 wins.  
- **Reach vs Wins (scatterplot)** → **V-shaped curve** → peak wins around **185cm reach**.  
- **Stance vs Wins (barplot)** → **Open stance** > Southpaw > Orthodox > Sideways.  

---

## 📌 Key Insights

- **40–90kg fighters** dominated in wins and submissions.  
- **Striking styles** had a clear edge over grappling.  
- Optimal **reach (~185cm)** gave better win chances.  
- **Open stance** fighters outperformed all others.  
- **Age was not a strong factor** for wins.  

---

## ⚙️ How to Run

1. Clone the repository:
   ```bash
       git clone https://github.com/darshil411/djs_compute_task.git
       cd ufc-fighters-eda
- Install required libraries: `pip install numpy pandas matplotlib seaborn`  
- Open the notebook in Jupyter: `jupyter notebook ufc_fighter.ipynb`  

