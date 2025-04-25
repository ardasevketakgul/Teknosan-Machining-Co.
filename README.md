#  Project Proposal for DSA 210

## **Project Title:**  
Analyzing Worker Performance in Teknosan Machining Co. Based on Experience Levels

## **Researcher:**  
Arda Şevket Akgül
## **Course & Term:**  
DSA 210 - Introduction to Data Science  
Spring 2024-2025  

---

## **Project Overview**  
This project aims to analyze worker performance data at Teknosan Machining Co. using various data analyzing techniques. The objective is to explore how worker experience levels correlate with productivity and defect rates through visual representations. The project will involve data cleaning, exploratory analysis, and graphical interpretations to present meaningful insights.

---

## **Data Sources**  
### **Primary Dataset: Worker Performance Data**  
- Collected from Teknosan Machining Co.  
- Contains variables such as:  
  - Worker ID  
  - Shift Type (Day/Night)  
  - Work Hours  
  - Productivity Metrics (Parts Produced, Defect Rates)  
  - Machine Usage
   
    

### **Supportive Dataset: Worker Experience Data**  
- Collected from Teknosan Machining Co.  
- Contains variables such as:  
  - Employment Duration
  
  

These datasets will be analyzed and visualized to identify trends and patterns in relation to worker experience.

---



## **Research Question & Hypothesis**  
### **Hypothesis: The Impact of Worker Experience on Defect Rates**  
**H₀ (Null Hypothesis):** Worker experience has no significant impact on defect rates.  
**H₁ (Alternative Hypothesis):** More experienced workers produce fewer defects.  

---

## **Analysis Plan**  
### **1. Data Collection & Cleaning **  
- Verify data completeness and consistency  
- Handle missing values & outliers  

### **2. Exploratory Data Analysis (EDA) & Visualization**  
- Visualize trends in worker experience vs. defect rates  
- Generate scatter plots, histograms, and bar charts  
- Create heatmaps and correlation matrices to explore relationships  
#**I wanted to visualize how efficient each worker is, one by one. In this scatter plot, every point represents a single worker. I sorted them by order in the dataset and plotted their efficiency scores. This helps to see which workers are much higher or lower than the others in terms of productivity.**
  ![Efficiency Scatter](visualization/ekrankaydı/c)






### **3. Hypothesis Testing **  

**Hypothesis 1**: Do more experienced workers perform better?
In order to investigate whether experience affects productivity, I grouped workers into two categories based on their years of experience:

Low Experience: 5 years or less
High Experience: more than 5 years
I then calculated the average efficiency for both groups and applied an independent samples t-test to evaluate the statistical significance of the difference.

Null Hypothesis (H0): There is no difference in efficiency between low and high experience groups.
Alternative Hypothesis (H1): Workers with more experience are more efficient.
After conducting the t-test, I observed a p-value below 0.05, indicating a statistically significant difference between the groups. Therefore, I rejected the null hypothesis and concluded that more experienced workers tend to be more efficient.
![Experience Boxplot](visualization/ekrankaydı/a)

**Hypothesis 2**: Do night shift workers perform worse?
To test whether working the night shift negatively affects productivity, I compared the efficiency of:

Day Shift Workers: shift 1 and 2
Night Shift Workers: shift 3
I performed both an independent t-test and a correlation analysis between shift number and efficiency.

Null Hypothesis (H0): There is no relationship between shift and efficiency.
Alternative Hypothesis (H1): Night shift workers are less efficient than day shift workers.
The p-value from the statistical tests was much higher than 0.05 (around 0.8), which means I failed to reject the null hypothesis. There is no statistically significant difference in efficiency between shifts. Thus, I cannot conclude that night shifts reduce productivity based on the available data.
![Shift Scatter](visualization/ekrankaydı/b)



### **3. Overall Conclusion on Hypothesis Testing** 
Overall Conclusion

In this project, I tested two different hypotheses about worker productivity at Teknosan.

First, I checked if more experienced workers have better efficiency. I used a t-test method by dividing workers into low and high experience groups. The results showed that experienced workers are actually more efficient, and the difference was statistically significant.

Second, I wanted to see if night shift workers have lower productivity. I did a t-test and also checked correlation between shift numbers and efficiency scores. In this case, the p-value was very high, so I could not find any meaningful difference between day and night shifts.

In short, experience seems to help productivity, but working at night does not make a big difference based on our data.

---







