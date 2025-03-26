# Post-Divorce-Impact-on-Children-Data-Analysis-Visualization
### A data analysis and visualization on post-divorce impact on children using Python Pandas, Seaborn and Plotly

## Problem Statement

The healthcare research centre aims to explore and understand the psychological effects of parental divorce on children, specifically focusing on emotional stability, academic performance, and overall mental health outcomes. The centre seeks to identify key factors contributing to children’s emotional well-being, whether therapy interventions are effective, and how different post-divorce scenarios (custody arrangements, social support, etc.) impact their development.  
The analysis will help provide evidence-based insights to guide the development of more effective interventions, therapeutic programs, and support structures to mitigate adverse impacts on children affected by parental divorce.

---

## Business Questions

### Emotional and Psychological Impact
1. **What is the relationship between the child’s emotional stability score and the type of custody arrangement (e.g., joint, mother, father, foster care)?**
   - **Goal:** Determine if the type of custody arrangement has a direct correlation with a child's emotional stability.
   
2. **How do depression and anxiety levels correlate with emotional stability scores in children after parental divorce?**
   - **Goal:** Understand how mental health factors such as depression and anxiety are influencing emotional stability in children.
   
3. **How does the child’s self-reported happiness score correlate with therapy receipt and type (Cognitive Behavioral Therapy vs. Family Therapy)?**
   - **Goal:** Evaluate the effectiveness of different therapy types in improving a child’s perceived happiness and emotional well-being.
   
4. **Does the availability of peer support positively impact the child’s emotional stability and academic performance?**
   - **Goal:** Investigate whether having peer support networks helps improve emotional resilience and academic performance.

### Academic Performance
5. **How does a child’s academic performance relate to their emotional stability and therapy received?**
   - **Goal:** Assess whether emotional stability, therapy, or both influence the academic outcomes in children after divorce.
   
6. **What is the impact of parental income level on a child’s academic performance post-divorce?**
   - **Goal:** Explore if socioeconomic status influences academic outcomes for children of divorced parents.
   
7. **Do children living with one parent (vs. foster care) perform better academically?**
   - **Goal:** Compare academic performance based on post-divorce living arrangements to see if children fare better living with their biological parents or in foster care.

### Social Trust and Future Relationships
8. **How does the child’s reported level of social trust relate to their relationship difficulties as an adult?**
   - **Goal:** Determine if trust issues arising from parental divorce affect future relationships and emotional stability.
   
9. **What is the correlation between a child’s reported relationship difficulty and factors like therapy received, post-divorce residency, and parental income level?**
   - **Goal:** Identify key contributing factors to future relationship challenges in children of divorced parents.

### Health and Support Systems
10. **How does the availability of health insurance impact the child’s access to mental health care and therapy after divorce?**
    - **Goal:** Investigate whether having health insurance increases access to therapeutic interventions and improves emotional stability.
   
11. **Is there a correlation between the child joining a support group and their mental health outcomes (e.g., reduced depression/anxiety levels)?**
    - **Goal:** Assess whether joining support groups provides relief and improves mental health outcomes.

### Post-Divorce Residencies and Custody Types
12. **How do different post-divorce residencies (Mother, Father, Foster Care) influence the child’s emotional stability and happiness?**
    - **Goal:** Examine if the child’s living situation post-divorce affects their emotional well-being and happiness.

### Effectiveness of Interventions
13. **Does therapy, in combination with other factors like peer support and post-divorce residency, lead to improved emotional stability in children?**
    - **Goal:** Assess whether therapy, combined with factors like peer support and residency, can significantly reduce emotional distress in children.

---

## Data Description

The dataset consists of 5000 rows and 18 columns, with both numerical and categorical variables. Below is a breakdown of the columns and their respective data types:

### Columns:

1. **Child_ID:**  
   - **Type:** Numerical (integer IDs from 1 to 5000).
   
2. **Age_at_Divorce:**  
   - **Type:** Numerical (e.g., 11, 8, 17 — integers representing age).

3. **Custody_Type:**  
   - **Type:** Categorical (e.g., "Mother", "Father", "Joint", "Foster Care").
   
4. **Therapy_Received:**  
   - **Type:** Categorical (e.g., "Yes", "No").

5. **Therapy_Type:**  
   - **Type:** Categorical (e.g., "Cognitive Behavioral Therapy", "Family Therapy", "None").

6. **Emotional_Stability_Score:**  
   - **Type:** Numerical (e.g., 3, 10, 5 — integers, likely a scale).

7. **Academic_Performance:**  
   - **Type:** Numerical (e.g., 78, 89, 59 — integers, likely a percentage or score).

8. **Peer_Support_Available:**  
   - **Type:** Categorical (e.g., "Yes", "No").

9. **Depression_Level:**  
   - **Type:** Numerical (e.g., 5, 3, 7 — integers, likely a scale).

10. **Anxiety_Level:**  
    - **Type:** Numerical (e.g., 7, 8, 1 — integers, likely a scale).

11. **Social_Trust_Level:**  
    - **Type:** Numerical (e.g., 7, 6, 9 — integers, likely a scale).

12. **Parent_Income_Level:**  
    - **Type:** Categorical (e.g., "High", "Low", "Medium").

13. **Divorce_Conflict_Level:**  
    - **Type:** Categorical (e.g., "Medium", "Low", "High").

14. **Post_Divorce_Residency:**  
    - **Type:** Categorical (e.g., "Father", "Mother", "Foster Care").

15. **Health_Insurance_Access:**  
    - **Type:** Categorical (e.g., "Yes", "No").

16. **Support_Group_Joined:**  
    - **Type:** Categorical (e.g., "Yes", "No").

17. **Relationship_Difficulty:**  
    - **Type:** Categorical (e.g., "Yes", "No").

18. **Self_Reported_Happiness:**  
    - **Type:** Numerical (e.g., 3, 1, 4 — integers, likely a scale).

### Summary of Classification:

- **Categorical Columns:**  
   - **Total:** 10 categorical columns  
   - **Columns:** Custody_Type, Therapy_Received, Therapy_Type, Peer_Support_Available, Parent_Income_Level, Divorce_Conflict_Level, Post_Divorce_Residency, Health_Insurance_Access, Support_Group_Joined, Relationship_Difficulty

- **Numerical Columns:**  
   - **Total:** 8 numerical columns  
   - **Columns:** Child_ID, Age_at_Divorce, Emotional_Stability_Score, Academic_Performance, Depression_Level, Anxiety_Level, Social_Trust_Level, Self_Reported_Happiness

### Final Answer:
- **Number of Rows:** 5000
- **Number of Columns:** 18
- **Number of Categorical Columns:** 10
- **Number of Numerical Columns:** 8

---

## Methods and Approach


In this project, the following tools and libraries were used to process and analyze the data:

1. **Python:** The primary programming language used for data analysis and model implementation.
   
2. **Pandas:** Used extensively for data manipulation, cleaning, and processing. Pandas DataFrame was used for handling and exploring the dataset.

3. **Seaborn:** Utilized for statistical data visualization. Seaborn was used to create informative and aesthetically pleasing plots to explore correlations and distributions of various variables.

4. **Plotly:** Employed for creating interactive visualizations. Plotly was particularly useful for creating interactive charts and graphs, allowing for deeper insights into the data.

These tools provided a robust framework for data analysis, visualization, and interpretation of the results.

---

## Results and Insights


Let's break down the Results---

1. **What is the relationship between the child’s emotional stability score and the type of custody arrangement (e.g., joint, mother, father, foster care)?**

**Boxplot** 

![Question1_Boxplot](https://github.com/user-attachments/assets/2b3e444c-8c4f-4243-8449-51152a29921f)

The **box plot** demonstrates the distribution of **emotional stability scores** for each custody type.  The median score for **Mother** Custody is **6**, while for other custody types **(Father, Joint, Foster Care)**, it is **5**. This suggests that children in **Mother** Custody tend to have slightly higher emotional stability. Since the boxes are of similar width, variability in scores is comparable across custody types. This indicates that while custody type has some impact, other factors may also influence emotional stability.

**Bargraph**

![Question1_Barplot](https://github.com/user-attachments/assets/1fb63b08-d8ad-46bb-ab64-3eb3ef0d3fb7)

This **bar chart** represents the **average emotional stability score** for children under different custody types. 
* If one custody type (e.g., Mother or Joint Custody) has a higher mean score, it suggests that children in this custody arrangement tend to have better emotional stability.

* A lower mean score for a group (e.g., Foster Care or Legal Guardian) may indicate higher emotional distress.

Here, **Mother Custody** has the **highest mean emotional stability score (5.57)**, suggesting children in this arrangement may experience the most stable emotional environment.

**Foster Care** follows closely with a **mean score** of **5.45**, which is surprisingly higher than **Father** **(5.41)** and **Joint Custody (5.39)**, indicating that support systems in foster care may contribute to emotional stability.

Father and Joint Custody show slightly lower scores, implying potential emotional challenges related to custody dynamics or adjustments, but the differences are minimal.

2. **How do depression and anxiety levels correlate with emotional stability scores in children after parental divorce?**

**BubbleChart**

![Question2_BubblePlot](https://github.com/user-attachments/assets/a18e0e55-22ab-4546-8c16-b5af7b69d59d)

This bubble chart demonstrates :

* The relationship between depression levels and emotional stability scores.

* The size of each bubble indicates the depression level, with larger bubbles representing higher depression levels.

* The color of each bubble will represent the anxiety level, allowing you to see if there's any correlation between anxiety levels and the depression-emotional stability relationship.

1. The color gradient indicates the anxiety level. Yellow represents higher anxiety levels, and blue represents lower anxiety levels. This color coding allows you to easily distinguish between different anxiety levels in the data points.

2. As depression levels increase, the size of the bubbles increases, meaning that higher depression levels are visually represented by larger bubbles. This helps to immediately identify which data points have higher depression levels.

3. Emotional stability scores and anxiety levels fluctuate as depression levels increase. This shows that while depression levels are rising (larger bubbles), emotional stability does not follow a simple trend.

4. In some cases, as depression increases, emotional stability might also increase, while in other cases, emotional stability decreases. Similarly, anxiety levels do not follow a single direction; sometimes they increase with depression, and sometimes they decrease.

The chart suggests that depression and emotional stability are not directly correlated, as emotional stability fluctuates even with increasing depression levels.  The anxiety level interacts dynamically with depression and emotional stability. In some cases, high depression might coincide with high anxiety (yellow color), while in others, high depression might correlate with lower anxiety (blue color). 

**DensityHeatMap** 

![Question2_DensityHeatmap](https://github.com/user-attachments/assets/9df484a7-9151-493f-8d80-909b0d0346ab)

A **density heatmap** that shows the relationship between Depression Level, Emotional Stability Score, and Anxiety Level. 

The color gradient indicates the anxiety level. Yellow represents higher anxiety levels, and blue represents lower anxiety levels.

From the **heatmap**, it can be observed that as the Depression Level increases, the Emotional Stability Score also tends to increase. However, the Anxiety Level does not follow a consistent pattern, with fluctuations observed. This suggests that while higher depression levels are sometimes associated with better emotional stability, the relationship between anxiety and these two factors is not linear. Anxiety levels appear to increase and decrease unpredictably across different ranges of depression and emotional stability scores, indicating that anxiety may not always correlate directly with changes in depression or emotional stability.

3. **How does the child’s self-reported happiness score correlate with therapy receipt and type (Cognitive Behavioral Therapy vs. Family Therapy)?**

**Piechart**

![Question3_Piechart](https://github.com/user-attachments/assets/304d392d-1ee9-4a1b-bc74-dde326119e29)

The **pie chart** delineates  the proportional distribution of different therapy types and their corresponding happiness scores, highlighting which therapy types have the most influence or frequency in the dataset.  

The **pie chart** shows that **Family Therapy (represented by the blue section)** makes up **66.9%** of the total data, while **Cognitive Behavioral Therapy (CBT) (represented by the red section)** accounts for **33.1%**. This distribution suggests that a higher proportion of individuals in the dataset received Family Therapy compared to **Cognitive Behavioral Therapy.**

**Bargraph**

![Question3_Barchart](https://github.com/user-attachments/assets/7c77d403-60a5-4c0f-8b5f-f1b5e4a6640e)

The bar chart will display the mean happiness scores for each therapy type. Each bar represents a different therapy type (such as Cognitive Behavioral Therapy, Family Therapy, etc.)  

The bar chart reveals that **Cognitive Behavioral Therapy (CBT)**, represented by the blue bar, has a slightly higher mean **happiness score of 5.46**, compared to **Family Therapy**, represented by the red bar, which has a mean **happiness score of 5.38.**

**This suggests that, on average, individuals who underwent Cognitive Behavioral Therapy reported slightly higher levels of happiness than those who received Family Therapy.** 



































