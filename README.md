# 🌍 CO₂ Emissions Across Global Countries

**Authors**:

* Atta Ur Rahman — Reg # 2024122
* Zawar Fahim — Reg # 2024494
* Hamza Sami — Reg # 2024212

---

## 📌 Overview

This project performs a comprehensive **statistical analysis** of global annual CO₂ emissions using Python. It demonstrates how to clean and preprocess real-world datasets, calculate meaningful statistics, and visualize data distributions. Key analyses include:

* Descriptive Statistics (mean, variance)
* Frequency Distribution via **Histograms** and **Pie Charts**
* **Grouped Data Analysis** using class midpoints
* **Confidence & Tolerance Intervals**
* **Hypothesis Testing** on log-transformed emissions

> **Dataset Source**: [Kaggle - Global CO₂ Emissions by Country (1750–2022)]([https://www.kaggle.com/datasets/patricklford/global-co-emissions](https://www.kaggle.com/datasets/yoannboyere/co2-ghg-emissionsdata))

---

## 🔬 Abstract

This report investigates CO₂ emissions across countries using data science techniques. Starting from raw CSV data, the project applies rigorous data cleaning, statistical modeling, and inferential methods to explore trends, detect outliers, and validate assumptions. It concludes with a one-sample **t-test** to test if the average emission (log-transformed) exceeds a certain threshold.

---

## 🧪 Methodology

### 1. **Data Cleaning**

* Missing values and non-positive entries were dropped from the emission column.

### 2. **Descriptive Statistics**

* Original **mean** and **variance** of emissions computed.
* Dataset found to be **highly skewed**, dominated by a few high-emission countries.

### 3. **Frequency Distribution**

* Data was split into **7 emission intervals**, ranging from `<1M` to `>1B` tonnes.
* Frequencies visualized using:

  * 📊 Histogram
  * 🥧 Pie Chart

### 4. **Grouped Statistics**

* Midpoints of emission intervals were used to estimate **mean** and **variance** from grouped data.

### 5. **Interval Estimations**

* Data was split into training (80%) and test (20%) subsets.
* Applied **log transformation** for normalization.
* Computed:

  * ✅ **95% Confidence Interval**
  * ✅ **95% Tolerance Interval**

### 6. **Hypothesis Testing**

* **Null Hypothesis (H₀)**: μ = 16
* **Alternative Hypothesis (H₁)**: μ > 16
* A one-sample **t-test** was used to verify whether the log-mean of emissions significantly exceeds 16.

---

## 📈 Results

### A. **Original Statistics**

| Metric   | Value          |
| -------- | -------------- |
| Mean     | 206,735,607.30 |
| Variance | 1.93 × 10¹⁸    |

### B. **Grouped Analysis**

* Estimated mean and variance from grouped data closely matched the original values, validating the grouping technique.

### C. **Interval Estimations**

| Interval Type  | Lower Bound | Upper Bound |
| -------------- | ----------- | ----------- |
| 95% Confidence | 15.2977     | 15.3932     |
| 95% Tolerance  | 9.3797      | 21.3112     |

* Validation on the test set showed strong coverage accuracy.

### D. **Hypothesis Test**

* **T-statistic**: *\[Insert]*
* **P-value**: *\[Insert]*
* ✅ Null hypothesis **rejected** → The log-transformed mean emission is statistically greater than 16.


## 🧾 Technologies Used

* Python 3
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy


---

## 📚 References

1. [Y. Boyere, Kaggle Dataset - CO₂ & GHG Emissions](https://www.kaggle.com/datasets/yoannboyere/co2-ghg-emissionsdata)
2. [P. L. Ford, Kaggle Dataset - Global CO₂ Emissions](https://www.kaggle.com/datasets/patricklford/global-co-emissions)

---

## 📌 Conclusion

This project demonstrates how real-world data can be analyzed using fundamental statistical methods. From data cleaning to hypothesis testing, each step reveals meaningful environmental insights that can influence global sustainability efforts and policymaking.

---

## 🤝 Acknowledgments

Special thanks to our instructors and peers who guided us through the ES111 (Probability & Statistics) course.

