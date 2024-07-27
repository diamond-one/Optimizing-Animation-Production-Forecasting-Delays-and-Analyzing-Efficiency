
## **Introduction**

This project aims to analyze efficiency in the animation production process across StudioA, StudioB, and StudioC. The primary focus is on identifying optimal team sizes, standardizing production processes, and improving overall efficiency across blocking and spline stages.

## **Data Collection Methodology**

**Data Sources and Tools:**
- Data was collected from various animation studios, detailing episode-level metrics, including frames completed, hours spent, and the number of animators involved.
- The data was processed using Python's pandas library for data cleaning and analysis, and visualizations were created using Matplotlib and Seaborn.

**Timeframe and Scope:**
- The analysis covers episodes across different studios using historical data from the previous 18 months, focusing on key production stages: blocking and spline.

**Challenges and Considerations:**
- Inconsistent data entries, particularly non-numeric values in critical columns, required thorough cleaning.
- Normalizing metrics across studios was essential for accurate comparison, addressing varying practices and data recording standards.

---

## **Story 1: Efficiency Analysis Across Studios**

**Data Insight**: 
An analysis of efficiency ratios across different studios revealed significant variations. StudioA consistently demonstrated superior performance compared to StudioB and StudioC, indicating differences in workflow efficiency and resource allocation.

**Method**:
To evaluate and compare the efficiency across studios, efficiency ratios were calculated for two key stages: blocking and spline. The **efficiency ratio** for each stage was defined as the output achieved per unit of input (e.g., number of frames per hour per animator). The analysis involved the following steps:
1. **Data Collection**: Data on the number of animators, frames completed, and hours spent was gathered for each studio and stage.
2. **Efficiency Calculation**: The efficiency ratio was computed using the formula:

   ![Efficiency Ratio](https://latex.codecogs.com/png.latex?\bg{white}\text{Efficiency%20Ratio}%20=%20\frac{\text{Output%20(Frames%20Completed)}}{\text{Input%20(Hours)}%20\times%20\text{Number%20of%20Animators}})

3. **Visualization**: Boxplots were created to illustrate the variability in efficiency across blocking and spline stages for StudioA, StudioB, and StudioC. These boxplots highlight the median efficiency and variability (interquartile range, IQR), providing a clear comparison of each studio's performance and efficiency consistency. Outliers were filtered out to focus on the core data and provide a clearer analysis.

**Boxplots** illustrating the variability in efficiency across studios, highlighting the need for standardized practices.
![f104e8da-296b-477d-9eef-fae38d194dfb](https://github.com/user-attachments/assets/7c0f4a63-bee4-48c1-b14b-24c6ad7fdbde)

**Solution**:
- **Standardize Efficiency Benchmarks**: Implement best practices from StudioA across all studios to standardize efficiency metrics.
- **Workflow Review**: Conduct a detailed review of workflows in StudioB and StudioC to identify specific inefficiencies and optimize processes.

---

## **Story 2: Correlating Animator Count with Production Metrics**

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

- **Efficiency Standardization**: Utilize StudioA's successful practices to set efficiency standards across all studios.
- **Optimized Team Sizes**: Refine team size allocations to match the complexity and needs of each episode, improving overall efficiency.

---

## **Conclusion**

This analysis provides a comprehensive overview of efficiencies in animation production across different studios. By implementing the suggested solutions, studios can refine their production processes, better manage resources, and ultimately produce higher-quality animations more efficiently. The project's focus on efficiency standardization and resource optimization offers new avenues for improvement beyond the existing analysis.
