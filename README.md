Optimizing Animation Production: Forecasting Delays and Analyzing Efficiency

## **Introduction**

This project aims to analyze and forecast delays in the animation production process across three studios—StudioA, StudioB, and StudioC. The primary goal is to identify inefficiencies, provide actionable insights, and standardize production processes to enhance efficiency. Key metrics analyzed include blocking and spline days (estimated, scheduled, actual), efficiency ratios, and correlations between animators and production metrics.

![image](https://github.com/user-attachments/assets/08fd948b-3f35-4bd0-9a3a-fef035dcc7ba)

## **Data Collection Methodology**

**Data Sources and Tools:**
- Data was collected from various animation studios, detailing episode-level metrics, including time estimates, actuals, and quotas.
- The data was processed using Python's pandas library for data cleaning and analysis, and visualizations were created using Matplotlib and Seaborn.

**Timeframe and Scope:**
- The analysis covers episodes across different studios using historical data from the previous 18 months, focusing on key production stages: blocking and spline.

**Challenges and Considerations:**
- Inconsistent data entries, particularly non-numeric values in critical columns, required thorough cleaning.
- Normalizing metrics across studios was essential for accurate comparison, addressing varying practices and data recording standards.

---

## **Stories and Solutions**

### **Story 1: Forecasting Delays in Animation Production**

**Data Insight:**
The analysis revealed significant episodes with either overestimated or underestimated blocking and spline days, indicating a need for improved estimation techniques.

**Solution:**
- **Refined Forecasting Model**: A refined forecasting tool was developed using historical data, incorporating variables such as team size, work capacity, and episode complexity. This model improves the accuracy of production timeline predictions.
- **Buffer System**: A 1-day buffer per episode was introduced to accommodate unforeseen delays, mitigating the impact on overall project timelines.
  
![5481035b-8b50-48bb-8e29-1df8600ceb82](https://github.com/user-attachments/assets/31c929df-c018-4576-8c9e-7a9980813422)

---

### **Story 2: Efficiency Analysis Across Studios**

**Data Insight**: 
An analysis of efficiency ratios across different studios revealed significant variations. StudioA consistently demonstrated superior performance compared to StudioB and StudioC, indicating differences in workflow efficiency and resource allocation.

**Method**:
To evaluate and compare the efficiency across studios, efficiency ratios were calculated for two key stages: blocking and spline. The **efficiency ratio** for each stage was defined as the output achieved per unit of input (e.g., number of frames per hour per animator). The analysis involved the following steps:
1. **Data Collection**: Data on the number of animators, frames completed, and hours spent was gathered for each studio and stage.
2. **Efficiency Calculation**: The efficiency ratio was computed using the formula:

   ![Efficiency Ratio](https://latex.codecogs.com/png.latex?\bg{white}\text{Efficiency%20Ratio}%20=%20\frac{\text{Output%20(Frames%20Completed)}}{\text{Input%20(Hours)}%20\times%20\text{Number%20of%20Animators}})

3. **Visualization**: Boxplots were created to illustrate the distribution of efficiency ratios for blocking and spline stages across StudioA, StudioB, and StudioC. These boxplots highlight the median efficiency, variability (IQR), and outliers, providing a clear view of each studio's performance.

**Solution**:
- **Standardize Efficiency Benchmarks**: Implement best practices from StudioA across all studios to standardize efficiency metrics.
- **Workflow Review**: Conduct a detailed review of workflows in StudioB and StudioC to identify specific inefficiencies and optimize processes.

**Boxplots** illustrating the variability in efficiency across studios, highlighting the need for standardized practices.
  
![f104e8da-296b-477d-9eef-fae38d194dfb](https://github.com/user-attachments/assets/7c0f4a63-bee4-48c1-b14b-24c6ad7fdbde)


---

### **Story 3: Correlating Animator Count with Production Metrics**

**Data Insight:**
A noticeable correlation was found between the number of animators and efficiency metrics. Episodes with fewer animators generally showed higher efficiency ratios, suggesting potential overstaffing or underutilization.

**Method for Determining Optimal Team Sizes:**
To identify the optimal team size for maximizing efficiency, the following method was employed:

1. **Data Collection**: Efficiency metrics were calculated for both Blocking and Spline stages, using the ratio of actual output to expected output for each project or episode.

2. **Filtering Outliers**: Data points with efficiencies below 0.65 or above 1.2 were removed to focus on the core data range and reduce the impact of extreme values.

3. **Optimal Efficiency Identification**:
   - The top 10% most efficient projects were identified by calculating the 90th percentile of the efficiency distribution for both Blocking and Spline stages.
   - The average number of animators for these top 10% most efficient projects was then calculated, representing the optimal team size.

4. **Visualization**: Scatter plots were created to illustrate the relationship between the number of animators and efficiency ratios, with trend lines and the optimal team sizes highlighted.

**Solution:**
- **Optimize Team Sizes**: Historical data was used to optimize team sizes, ensuring that animator allocation matched the episode's complexity.
- **Flexible Staffing Strategies**: Flexible staffing strategies were implemented to dynamically adjust team sizes as needed, maintaining efficiency without overstaffing.

**Scatter Plots** showing the relationship between the number of animators and efficiency ratios for both blocking and spline stages.

![4afe87f7-3575-4157-abb7-54fbc2e71e3c](https://github.com/user-attachments/assets/6e759ba5-d0dd-48bd-8ae1-109428c70391)


---

## **Key Insights and Recommendations**

- **Improved Forecasting**: Implement advanced predictive models to better estimate project timelines and resource needs.
- **Efficiency Standardization**: Utilize StudioA's successful practices to set efficiency standards across all studios.
- **Optimized Team Sizes**: Refine team size allocations to match the complexity and needs of each episode, improving overall efficiency.

---

## **Conclusion**

This analysis provides a comprehensive overview of delays and efficiencies in animation production across different studios. By implementing the suggested solutions, studios can refine their production processes, better manage resources, and ultimately produce higher-quality animations more efficiently. The project's focus on forecasting, efficiency standardization, and resource optimization offers new avenues for improvement beyond the existing analysis.
