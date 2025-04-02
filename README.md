# Correlation
# 🔗 Correlation Analysis: E-Commerce Behavior & Academic Salaries

This project explores relationships in two datasets:
- **User behavior on an e-commerce website** (e.g., visits, page views)
- **Academic salaries** (from R's built-in `car` package)

## 📊 Part 1: E-Commerce Dataset

### 🧠 Key Questions
1. How frequently do users visit the site?
2. How do estimated page views relate to number of visits?
3. Is there a correlation between browsing behavior and activity?

### 🧰 Techniques Used
- Log transformation of visit frequency
- Histogram and frequency plots
- Integer mapping of page view categories
- Scatterplots (including jittered)
- Pearson correlation and hypothesis testing

---

## 🎓 Part 2: Academic Salaries Dataset

### 🧠 Key Questions
1. What are the relationships among years of service, years since PhD, and salary?
2. Are more experienced academics paid significantly more?

### 🧰 Techniques Used
- `scatterplotMatrix` for multivariate visualization
- Correlation matrix using `corrplot` and `corrplot.mixed`
- Focused analysis on `yrs.since.phd`, `yrs.service`, and `salary`

---

## 📈 Sample Outputs

| Dataset     | Key Insight |
|-------------|-------------|
| E-commerce  | Page views and site visits are moderately correlated (improves when visits are log-scaled) |
| Salaries    | Strong correlation between service and PhD years, weak to moderate with salary |

---

## 💻 How to Run

```r
install.packages(c("car", "corrplot", "psych"))
source("correlation_analysis.R")
