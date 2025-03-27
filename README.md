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

The bar chart displays the mean happiness scores for each therapy type. Each bar represents a different therapy type (such as Cognitive Behavioral Therapy or family Therapy).  

The bar chart reveals that **Cognitive Behavioral Therapy (CBT)**, represented by the blue bar, has a slightly higher mean **happiness score of 5.46**, compared to **Family Therapy**, represented by the red bar, which has a mean **happiness score of 5.38.**

**This suggests that, on average, individuals who underwent Cognitive Behavioral Therapy reported slightly higher levels of happiness than those who received Family Therapy.** 

**Boxplot**

![Question3_Boxplot](https://github.com/user-attachments/assets/d411aaa3-42e8-439b-aef6-26d85c839637)

The **box plot** shows that both **Cognitive Behavioral Therapy (CBT)** and **Family Therapy** have the same median **happiness score of 5.** This suggests that both therapies have similar average effects on happiness, though the spread and outliers may differ.


4. **Does the availability of peer support positively impact the child’s emotional stability and academic performance?**

**Scatterplot**-

![Question4_ScatterPlot](https://github.com/user-attachments/assets/2a0a0427-5c47-4e46-91d0-e7a947310560)

The bubble chart shows that as the Emotional Stability Score increases, the Academic Performance Score also increases. This trend appears to be influenced by the availability of peer support.

**When peer support is available (Yes):** The bubbles representing these points tend to be larger, indicating a positive correlation between emotional stability and academic performance.

**When peer support is not available (No):** The bubbles are smaller, and the relationship between emotional stability and academic performance might be less pronounced or fluctuating.

This suggests that peer support might play a role in improving both emotional stability and academic performance.

5. **How does a child’s academic performance relate to their emotional stability and therapy received?**

**Bargraph - Academic Performance by Therapy Type**

![Question5_Bargraph](https://github.com/user-attachments/assets/e25a6608-cc23-485e-99d5-934fc9a6b8be)

The bar chart illustrates the average academic performance based on whether therapy was received or not.

* **When therapy was received (Yes):** The bar is colored green and shows an average academic performance score of 75.26.

* **When therapy was not received (No):** The bar is colored red and shows an average academic performance score of 74.82.

This suggests that therapy might have a slight positive effect on academic performance, as the average score for those who received therapy is marginally higher than for those who did not.

**Bargraph - Academic Performance vs Emotional Stability by Therapy Received**

![Question5_Bargraph2](https://github.com/user-attachments/assets/3baa5ecd-f640-4148-9377-1af21395df30)

In the bar chart, based on the therapy received (Yes or No), we can observe the following insights:

**For Academic Performance:**

* When therapy is received (Yes), the average academic performance is 75.26.

* When therapy is not received (No), the average academic performance is 74.82.

**For Emotional Stability Score:**

* When therapy is received (Yes), the average emotional stability score is 5.43.

* When therapy is not received (No), the average emotional stability score is 5.48.


**Academic Performance** is slightly better for those who have received therapy (75.26 vs. 74.82).

**Emotional Stability** is slightly better for those who have not received therapy (5.48 vs. 5.43).


6. **What is the impact of parental income level on a child’s academic performance post-divorce?**

**Bargraph**

![Question6_Bargraph3](https://github.com/user-attachments/assets/ed6f5b35-23c2-4744-8994-2602a749663d)

In the bar graph showing Academic Performance by Parent Income Level:

* The **High income group**, represented by the **light green bar**, has an **academic performance score** of **75.61.**

* The **Low income group**, represented by the **light red bar**, has an **academic performance score** of **74.64.**

* The **Medium income group**, represented by the **light blue bar**, has an **academic performance score** of **74.86.**

This suggests that students with higher parental income tend to have slightly better academic performance compared to those with lower or medium income.

**Treemap**

![Question6_Treegraph](https://github.com/user-attachments/assets/d61e4b81-4e7e-4ac1-8c76-ad3cc44506c5)

In the Treemap of Academic Performance by Parent Income Level:

* **Medium income group (blue)** has a total academic performance score of 128,624.

* **High income group (red)** has a total academic performance score of 126,284.

* **Low income group (green)** has a total academic performance score of 120,326.

This suggests that students from medium-income families collectively have the highest academic performance, followed by high-income and then low-income families. However, this does not indicate individual performance but rather the total contribution of each income group.

**ViolinPLot**

![Question6_ViolinPlot](https://github.com/user-attachments/assets/5949cb84-cf35-4111-a3a0-631e035c3088)

The violin plot shows that academic performance scores range from 50 to 100 across all **parent income levels (High, Medium, Low)** with a similar distribution. The median score is around **75-80** for all groups, and the **interquartile range (IQR)** is consistent, indicating no significant performance gap. The density of scores is highest between **80-90**, meaning most students score within this range. The distribution is **symmetric**, with no extreme outliers, suggesting income level has little impact on academic performance.


7. **Do children living with one parent (vs. foster care) perform better academically?**

**Bargraph**

![Question7_Bargraph](https://github.com/user-attachments/assets/53188bc4-50db-45c4-abfd-e98c4ce2e83d)

The bar chart compares **academic performance based on post-divorce residency**. The **Mother category (goldenrod)** has the highest average score of **75.644**, followed by **Father (dark red)** at **74.768**, and **Foster Care (royal blue)** at **74.734**. The differences are minimal, suggesting post-divorce residency type has little impact on academic performance.


**Sunburst**

![Question7_Sunburst](https://github.com/user-attachments/assets/7ec7b971-0b4f-439e-a56c-fbe40ea7322d)

The sunburst chart visualizes the distribution of academic performance based on post-divorce residency type. The **Foster Care category (blue)** has the highest count at 1,689, followed by **Father (red)** at 1,656 and **Mother (green)** at 1,655. The counts are relatively balanced across categories, suggesting no significant dominance of one residency type over others in terms of student population.


**Piechart**

![Question7_Pie](https://github.com/user-attachments/assets/43f6e54a-8129-4dcb-9102-38fe0c0c82a4)

The pie chart shows the distribution of academic performance across different post-divorce residency types. The percentages are nearly equal, with **Foster Care (blue) at 33.6%**, **Mother (red) at 33.4%**, and **Father (green) at 33%**. This suggests that academic performance is fairly consistent across residency types, indicating no major advantage or disadvantage based on where a student resides after divorce.


**Boxplot**

![Question7_Boxplot](https://github.com/user-attachments/assets/4894409b-ff2d-4c85-9b15-11048ab27188)

The box plot shows the distribution of academic performance across different post-divorce residency types. The median score for students living with their **mother is 77**, which is slightly higher than those living with their **father (74)** or in **foster care (74)**. This suggests that, on average, students residing with their mother tend to perform slightly better academically. However, the spread (interquartile range) and possible outliers would provide more insight into performance variability across these groups.


8. **How does the child’s reported level of social trust relate to their relationship difficulties as an adult?**

**ScatterPLot**

![Question8_ScatterPlot](https://github.com/user-attachments/assets/2a44a32e-705f-4fe1-b6a6-028231f1cb7a)

There does not appear to be a strong correlation between Social Trust Level and Relationship Difficulty based on this scatter plot. The relationship might be complex or influenced by other factors not captured in this visualization. A more detailed statistical analysis (like logistic regression) could help clarify any underlying patterns.


**DensityHeatMap**

![Question8_DensityHeatmap](https://github.com/user-attachments/assets/bdea4c38-faf0-423b-882f-7b382084cf01)

There is no direct linear relationship between Social Trust Level and Relationship Difficulty. The count of people experiencing relationship difficulties varies across trust levels, suggesting the presence of other influencing factors beyond just social trust.


9. **What is the correlation between a child’s reported relationship difficulty and factors like therapy received, post-divorce residency, and parental income level?**

**Bargraph**

![Question9_Bargraph](https://github.com/user-attachments/assets/f061fdcd-8459-476e-8dc5-db073071c71b)

When there is a relationship difficulty (i.e., for "Yes"), **Foster Care** has the highest average relationship difficulty score at **0.525**, followed by **Father** at **0.483**, and **Mother** with the lowest score of **0.465**. In contrast, when there is no relationship difficulty (i.e., for "No"), Mother has the highest average score at **0.503**, closely followed by **Foster Care** at **0.509**, and **Father** with the lowest score of **0.48**. **Overall, Foster Care tends to have the highest difficulty score in both cases, while Mother's and Father's scores are relatively close, with Mother slightly higher when there is no difficulty, and Father slightly higher when there is a difficulty.**


10. **How does the availability of health insurance impact the child’s access to mental health care and therapy after divorce?**

**DonutChart**

![Question10_Donutchart](https://github.com/user-attachments/assets/558a70b2-731f-4b77-b69f-03b0c12c96b0)

This suggests that almost half of the individuals have access to health insurance **(Yes/1)**, while the other half does not **(No/0)**. The **donut chart** visually represents these proportions with the blue section covering **50.2%** of the chart and the red section covering **49.8%.**

This gives an easy visual comparison of the two groups, helping to highlight the nearly equal distribution of health insurance access.

11. **Is there a correlation between the child joining a support group and their mental health outcomes (e.g., reduced depression/anxiety levels)?**

**Histplot**

![Question11_Histplot](https://github.com/user-attachments/assets/7ef0e6c9-5dc4-422b-bf5b-eb0ab754ad42)

The histogram shows the distribution of **Depression Levels** based on whether individuals **joined a support group or not**. The **blue bars** represent individuals **who did not join a support group**, while the **orange bars** indicate those **who did**. Across all depression levels, the count of non-members is consistently higher than that of support group members. The distribution appears uniform, with no extreme spikes at specific depression levels. The **KDE curves** further highlight this trend, showing that the overall depression level patterns are similar for both groups, with non-members having a slightly higher density. **This suggests that while support group participation exists, it does not drastically alter the depression level distribution.**


12. **How do different post-divorce residencies (Mother, Father, Foster Care) influence the child’s emotional stability and happiness?**

**Boxplot**

![Question12_Boxplot](https://github.com/user-attachments/assets/a7d89c9c-95b8-4761-bc56-4f28e1f81408)


The Box Plot indicates - 

**Father (Blue)** has the highest median emotional stability score of 6.

**Foster Care (Red)** has a median emotional stability score of 5.

**Mother (Green)** also has a median emotional stability score of 5.

This means that, on average, individuals in the "Father" category tend to have higher emotional stability post-divorce compared to those in the "Foster Care" and "Mother" categories, who have the same median emotional stability score.


13. **Does therapy, in combination with other factors like peer support and post-divorce residency, lead to improved emotional stability in children?**

**DensityMap**

![Question13_DensityHeatmap](https://github.com/user-attachments/assets/724d5c3b-dd15-442b-a10e-c0d5ba0da5df)

The heatmap suggests that peer support has a more significant impact on emotional stability in Family Therapy, with a notable increase in the emotional stability score when peer support is available **(9230 vs. 9091)**. In contrast, peer support shows minimal impact on emotional stability for Cognitive Behavioral Therapy (CBT), as the scores are nearly identical whether peer support is available or not **(4481 vs. 4505)**. This indicates that Family Therapy may benefit more from peer support, while CBT's effectiveness seems to be less influenced by it, possibly due to the individual-focused nature of CBT compared to the more interpersonal dynamics of Family Therapy.

---

## Conclusion

This analysis highlights the significant impact of parental divorce on children's emotional stability, academic performance, and future relationships. Key findings suggest that custody arrangements, therapy, peer support, and socioeconomic factors play a crucial role in shaping children's well-being post-divorce. Therapy, particularly Cognitive Behavioral Therapy, appears to enhance emotional resilience, while peer support contributes positively to both emotional and academic outcomes. Additionally, access to health insurance improves mental health care availability, reducing anxiety and depression levels.  

These insights emphasize the need for targeted interventions, improved therapy programs, and stronger support structures to mitigate the adverse effects of parental divorce and promote healthier emotional and psychological development in children.


## Project Link-

Due to bigger size of .ipynb file I could not upload it in github. Here is the shared google link [https://drive.google.com/drive/folders/1ITkoowND94D2NMyI2qlQduCwT-lBPBir?usp=drive_link]. 


