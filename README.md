# **Forecasting Delays and Analyzing Efficiency in Animation Production**

## **Introduction**

This project aims to analyze and forecast delays in the animation production process across three studios—StudioA, StudioB, and StudioC. The primary goal is to identify inefficiencies, provide actionable insights, and standardize production processes to enhance efficiency. Key metrics analyzed include blocking and spline days (estimated, scheduled, actual), efficiency ratios, and correlations between animators and production metrics.

![output (1)](https://github.com/user-attachments/assets/d143c401-126a-4f22-971d-6d5790ca5773)

## **Data Collection Methodology**

**Data Sources and Tools:**
- Data was collected from various animation studios, detailing episode-level metrics, including time estimates, actuals, and quotas.
- The data was processed using Python's pandas library for data cleaning and analysis, and visualizations were created using Matplotlib and Seaborn.

**Timeframe and Scope:**
- The analysis covers episodes across different studios over a specified period, focusing on key production stages: blocking and spline.

**Challenges and Considerations:**
- Inconsistent data entries, particularly non-numeric values in critical columns, required thorough cleaning.
- Normalizing metrics across studios was essential for accurate comparison, addressing varying practices and data recording standards.

---

## **Stories and Solutions**

### **Story 1: Forecasting Delays in Animation Production**

**Data Insight:**
The analysis revealed significant episodes with either overestimated or underestimated blocking and spline days. Notably, Episodes `309A` and `309B` in StudioC showed the largest positive delays, indicating a need for improved estimation techniques.

**Solution:**
- **Refined Forecasting Model**: Utilize historical data to develop a more accurate forecasting model, enabling better prediction of production timelines.
- **Buffer System**: Introduce a buffer system to accommodate unforeseen delays, thereby reducing the impact on overall project timelines.


- **Histograms** showcasing the distribution of delays in both blocking and spline stages, highlighting episodes with significant deviations.
  
![output (2)](https://github.com/user-attachments/assets/0cf04078-741f-4f87-9e6d-2dab40e0e456)
![output (3)](https://github.com/user-attachments/assets/f6727eeb-bde4-42b4-bee0-c0f2232dfbd7)

---

### **Story 2: Efficiency Analysis Across Studios**

**Data Insight:**
Efficiency ratios varied significantly across studios. StudioA consistently showed better performance compared to StudioB and StudioC, indicating differences in workflow efficiency and resource allocation.

**Solution:**
- **Standardize Efficiency Benchmarks**: Implement best practices from StudioA across all studios to standardize efficiency metrics.
- **Workflow Review**: Conduct a detailed review of StudioB and StudioC workflows to identify specific inefficiencies and optimize processes.

- **Boxplots** illustrating the variability in blocking and spline efficiency across studios, highlighting the need for standardized practices.
  
![output (5)](https://github.com/user-attachments/assets/8ba2413a-f816-44ec-8f11-af9092d85776)
![output (6)](https://github.com/user-attachments/assets/35e42995-27cb-4162-af29-fdf95cd3a916)

---

### **Story 3: Correlating Animator Count with Production Metrics**

**Data Insight:**
A noticeable correlation was found between the number of animators and efficiency metrics. Episodes with fewer animators generally showed higher efficiency ratios, suggesting potential overstaffing or underutilization.

**Solution:**
- **Optimize Team Sizes**: Use historical data to optimize team sizes, ensuring that animator allocation matches the episode's complexity.
- **Flexible Staffing Strategies**: Implement flexible staffing strategies to dynamically adjust team sizes as needed, maintaining efficiency without overstaffing.

**Scatter Plots** showing the relationship between the number of animators and efficiency ratios for both blocking and spline stages.
![output (8)](https://github.com/user-attachments/assets/ecea7cb4-c014-4a8f-80de-420b4acf2ffc)

---

## **Key Insights and Recommendations**

- **Improved Forecasting**: Implement advanced predictive models to better estimate project timelines and resource needs.
- **Efficiency Standardization**: Utilize StudioA's successful practices to set efficiency standards across all studios.
- **Optimized Team Sizes**: Refine team size allocations to match the complexity and needs of each episode, improving overall efficiency.

---

## **Conclusion**

This analysis provides a comprehensive overview of delays and efficiencies in animation production across different studios. By implementing the suggested solutions, studios can refine their production processes, better manage resources, and ultimately produce higher-quality animations more efficiently. The project's focus on forecasting, efficiency standardization, and resource optimization offers new avenues for improvement beyond the existing analysis.



