# **Data Mining Fundamentals: A Study Guide**
### **Quiz**

Instructions: Answer the following questions in 2-3 sentences each.

1. What is the difference between symmetric and asymmetric binary attributes? Provide an example of each.
2. Explain the difference between interval-scaled and ratio-scaled attributes, and give an example of each.
3. Describe the curse of dimensionality and why it is important in data mining.
4. What are quartiles, and how are they used in the context of boxplots?
5. Explain the difference between a histogram and a quantile plot.
6. Describe the key characteristics of a normal distribution curve and what percentages of data fall within 1, 2, and 3 standard deviations from the mean.
7. Explain the purpose of data visualization and list three benefits it provides in the context of data mining.
8. What are geometric projection visualization techniques? Name and describe two different methods.
9. Explain the concept of cosine similarity and its application in document analysis.
10. Describe the key characteristics of a data matrix and a dissimilarity matrix, including the number of modes each contains.

### **Quiz Answer Key**
1. Symmetric binary attributes have two states that are equally important (e.g., gender), while asymmetric binary attributes have outcomes that are not equally important (e.g., a medical test result), where one state is usually more significant and assigned the value 1.
2. Interval-scaled attributes have equal-sized units, indicating order and magnitude, but no true zero point (e.g., temperature in Celsius). Ratio-scaled attributes also have equal-sized units and order, but they have an inherent zero point, allowing for ratio comparisons (e.g., temperature in Kelvin or monetary quantities).
3. The curse of dimensionality refers to the challenges that arise when dealing with high-dimensional data, including increased computational complexity, sparsity, and the potential for irrelevant features to obscure meaningful patterns. It is important because it can significantly impact the performance and accuracy of data mining algorithms.
4. Quartiles divide a dataset into four equal parts: Q1 (25th percentile), Q2 (median, 50th percentile), and Q3 (75th percentile). In boxplots, the ends of the box represent Q1 and Q3, and the median is marked within the box, providing a visual summary of the data's central tendency and spread.
5. A histogram displays tabulated frequencies of data as bars, showing the proportion of cases within non-overlapping intervals of a variable. In contrast, a quantile plot displays all of the data, plotting quantile information by indicating that approximately 100 fi% of the data are below or equal to the value xi.
6. A normal distribution curve is symmetric and bell-shaped, characterized by its mean (μ) and standard deviation (σ). Approximately 68% of the measurements fall within μ±σ, 95% within μ±2σ, and 99.7% within μ±3σ.
7. The purpose of data visualization is to gain insight into data through graphical representation. It helps provide a qualitative overview of large datasets, search for patterns and relationships, and find interesting regions for quantitative analysis.
8. Geometric projection visualization techniques involve visualizing geometric transformations and projections of data. Two common methods are scatterplot matrices, which display all possible pairwise scatterplots of the dimensions, and parallel coordinates, which represent each data item as a polygonal line intersecting parallel axes representing the attributes.
9. Cosine similarity measures the cosine of the angle between two non-zero vectors, representing the similarity between them. In document analysis, it is used to determine the similarity between documents based on the term frequencies, where a higher cosine value indicates greater similarity.
10. A data matrix is an n x p matrix with n data points and p dimensions, representing the raw data in a multi-dimensional space and has two modes. A dissimilarity matrix stores the pairwise distances between n data points, forming a triangular matrix that registers only the distance and has a single mode.
### **Essay Questions**
1. Discuss the different types of attributes encountered in data mining, including nominal, binary, ordinal, interval, and ratio. Provide examples of each and explain how the choice of attribute type affects the selection of appropriate data mining techniques.
2. Explain the concepts of central tendency and dispersion. Describe several measures of each, such as mean, median, mode, variance, and standard deviation. How do these measures help in understanding the distribution and characteristics of data?
3. Compare and contrast different data visualization techniques discussed in the material. Include a discussion of pixel-oriented, geometric projection, icon-based, and hierarchical visualization techniques. Provide specific examples of when each technique is most appropriate.
4. Explain the concepts of similarity and dissimilarity in data mining. Discuss different measures for computing similarity and dissimilarity for various attribute types, including nominal, binary, and numeric data. Provide examples of how these measures are used in data analysis tasks.
5. Discuss the importance of understanding and getting to know your data before applying data mining algorithms. How can basic statistical descriptions, data visualization, and similarity/dissimilarity measures help in this process? Provide examples of potential pitfalls if this step is skipped.
### **Glossary of Key Terms**
- **Attribute**: A data field representing a characteristic or feature of a data object.
- **Nominal** Attribute: A categorical attribute representing names or categories, such as hair color or marital status.
- **Binary** Attribute: A nominal attribute with only two states, typically represented as 0 or 1.
- **Ordinal** Attribute: An attribute with values that have a meaningful order or ranking, such as size (small, medium, large).
- **Interval-Scaled Attribute**: A numeric attribute measured on a scale of equal-sized units, with order and magnitude, but no true zero point, such as temperature in Celsius.
- **Ratio-Scaled Attribute**: A numeric attribute with an inherent zero point, allowing for ratio comparisons, such as temperature in Kelvin.
- **Discrete Attribute**: An attribute with a finite or countably infinite set of values, such as zip codes or professions.
- **Continuous Attribute**: An attribute with real numbers as attribute values, such as temperature or height.
- **Data Object**: Represents an entity in a dataset, also called samples, examples, instances, data points, objects, or tuples.
- **Dimensionality**: The number of attributes (dimensions, features, variables) that describe a data object.
- **Curse of Dimensionality**: The challenges that arise when dealing with high-dimensional data, including increased computational complexity and sparsity.
- **Sparsity**: A characteristic of data where only the presence of certain attributes is significant, while most values are zero.
- **Mean**: The average of a set of numerical values.
- **Median**: The middle value in a sorted set of numerical values.
- **Mode**: The value that occurs most frequently in a dataset.
- **Quartiles**: Values that divide a dataset into four equal parts (Q1, Q2, Q3).
- **Inter-Quartile Range (IQR)**: The difference between the third quartile (Q3) and the first quartile (Q1), representing the spread of the middle 50% of the data.
- **Outlier**: A data point that is significantly different from other data points in the dataset, often defined as a value higher or lower than 1.5 x IQR.
- **Variance**: A measure of the spread of data points around the mean.
- **Standard Deviation**: The square root of the variance, representing the typical deviation of data points from the mean.
- **Boxplot**: A graphical representation of the five-number summary (min, Q1, median, Q3, max) of a distribution, used to visualize central tendency, spread, and outliers.
- **Histogram**: A graphical display of tabulated frequencies, shown as bars, representing the distribution of a numerical variable.
- **Quantile Plot**: A plot displaying all of the data with the values sorted in increasing order, fi indicates that approximately 100 fi% of the data are below or equal to the value xi.
- **Quantile-Quantile (Q-Q) Plot**: A plot comparing the quantiles of two univariate distributions to assess if they have a similar shape and distribution.
- **Scatter Plot**: A plot displaying pairs of values as points in a plane, used to visualize the relationship between two variables.
- **Data Visualization**: The process of mapping data onto graphical primitives to gain insight, overview large datasets, and identify patterns.
- **Pixel-Oriented Visualization**: A visualization technique where each data dimension is mapped to a pixel in a separate window.
- **Geometric Projection Visualization**: A visualization technique involving geometric transformations and projections of the data, such as scatterplot matrices and parallel coordinates.
- **Icon-Based Visualization**: A visualization technique that represents data values as features of icons, such as Chernoff faces or stick figures.
- **Hierarchical Visualization**: A visualization technique that uses a hierarchical partitioning of data into subspaces, such as dimensional stacking or tree-maps.
- **Similarity**: A numerical measure of how alike two data objects are.
- **Dissimilarity**: A numerical measure of how different two data objects are.
- **Data Matrix**: A matrix where rows represent data points and columns represent attributes.
- **Dissimilarity Matrix**: A matrix that stores the pairwise distances or dissimilarities between data points.
- **Minkowski Distance**: A generalized distance measure between two points in a multi-dimensional space.
- **Manhattan Distance (L1 Norm)**: The sum of the absolute differences between the coordinates of two points.
- **Euclidean Distance (L2 Norm)**: The straight-line distance between two points.
- **Cosine Similarity**: A measure of similarity between two non-zero vectors, based on the cosine of the angle between them, used in document analysis and other applications.