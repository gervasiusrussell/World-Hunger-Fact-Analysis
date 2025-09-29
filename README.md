# 🌍 World Hunger Fact

This project analyzes **global hunger data** using R, focusing on children under five years old. The study highlights hunger trends, severity levels across countries, and changes over time using statistical analysis and visualization.

## 📌 Project Overview

* **Topic**: World Hunger and Global Hunger Index (GHI)
* **Objective**:

  * Identify trends in global hunger over time
  * Highlight countries with severe hunger levels
  * Raise awareness of hunger’s devastating impacts on child development, health, education, and economic growth
* **Relevance**: Supports **SDG #2: Zero Hunger**

## 📊 Data Sources

All datasets are taken from Kaggle:

* [Global Hunger Index](https://www.kaggle.com/datasets/whenamancodes/the-global-hunger-index)
* Share of children underweight
* Share of children stunted
* Share of children wasted

## ⚙️ Methodology

1. **Data Preprocessing**

   * Merge datasets into one unified table
   * Handle missing values: drop rows with >2 NA, replace small NA counts with column mean
   * Remove redundant columns

2. **Feature Engineering**

   * Construct `hunger_rate` = average of

     * Child underweight
     * Child stunting
     * Child wasting

3. **Exploratory Data Analysis (EDA)**

   * Summary statistics (mean, median, skewness)
   * Boxplots and outlier detection
   * Density plots to analyze hunger index distribution over years

4. **Classification of Hunger Severity** (based on GHI scale):

   * **Low** ≤ 9.9
   * **Moderate** 10.0 – 19.9
   * **Serious** 20.0 – 34.9
   * **Alarming** 35.0 – 49.9
   * **Extremely Alarming** ≥ 50.0

## 📂 Repository Structure

```
World-Hunger-Fact/
│── data/                  # Raw datasets (CSV)  
│── explorationFunction.R  # Utility function for outlier detection  
│── world_hunger.Rmd       # Main R Markdown report  
│── README.md              # Project documentation  
```

## 📈 Expected Output

* Cleaned and merged dataset
* Hunger severity classification by country
* Trends of global hunger index across years (2000, 2006, 2012, 2021)
* Visualizations: boxplots, density plots, summary tables

## 👥 Authors

* Jonathan William Gunawan (2702251794)
* Vincentius Jonathan Tanujaya (2702259632)
* I Made Bagus Narendra (2702268561)
* Nixon Alexander (2702248420)

## 📚 References

* [World Vision Canada – World Hunger Facts](https://www.worldvision.ca/stories/food/world-hunger-facts-how-to-help#What%20is%20world%20hunger)
* [RRI – Kelaparan Krisis Serius](https://www.rri.co.id/kupang/nasional/714100/kelaparan-krisis-serius-yang-menjadi-perhatian-dunia)
* [Byju’s Global Hunger Prep Notes](https://byjus.com/free-ias-prep/global)
