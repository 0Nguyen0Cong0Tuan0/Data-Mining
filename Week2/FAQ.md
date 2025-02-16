# **Data Mining Data Types, Attributes, and Similarity Measures**

### **What are the main types of data sets encountered in data mining?**
Data sets can be categorized into several types, including record data (relational records, data matrix, document data like text documents represented as term-frequency vectors, and transaction data), graph and network data (e.g., the World Wide Web, social networks), ordered data (video data, temporal data, sequential data like transaction sequences, and genetic sequence data), and spatial/image/multimedia data.

### **What are the key attribute types, and how do they differ?**
Attributes, which describe data objects, can be nominal (categories or names), binary (two states), ordinal (meaningful order but unknown magnitude between values), or numeric (quantitative). Numeric attributes can be interval-scaled (equal-sized units but no true zero-point, like temperature in Celsius) or ratio-scaled (inherent zero-point, like temperature in Kelvin or monetary quantities). Attributes can also be discrete (finite or countably infinite values) or continuous (real numbers as values).

### **How are central tendency and data dispersion measured, and why are they important?**
Central tendency is measured by the mean (average), weighted mean (average considering weights), trimmed mean (average after removing extreme values), median (middle value), and mode (most frequent value). Data dispersion is measured by quartiles, inter-quartile range (IQR), variance, and standard deviation. These measures are important for understanding the distribution and spread of data, identifying outliers, and gaining a comprehensive view of the data's characteristics.

### **What is a boxplot, and how can it be used to analyze data dispersion?**
A boxplot is a graphical representation of the five-number summary (minimum, first quartile (Q1), median, third quartile (Q3), and maximum). The box represents the IQR, with the median marked inside. Whiskers extend to the minimum and maximum values within a certain range, and outliers are plotted as individual points. Boxplots provide a visual way to compare the distribution and identify outliers in different datasets.

### **What are some common techniques for visualizing data, and what insights can they provide?**
Common data visualization techniques include histograms (frequencies of values), quantile plots (showing the percentage of data below or equal to a given value), quantile-quantile (Q-Q) plots (comparing quantiles of two distributions), scatter plots (showing relationships between two variables), pixel-oriented techniques, geometric projection techniques (e.g., scatterplot matrices, parallel coordinates, landscapes), icon-based techniques (e.g., Chernoff faces, stick figures), and hierarchical techniques (e.g., dimensional stacking, tree-maps, cone trees, info-cubes). These techniques help to identify patterns, trends, outliers, and relationships within the data.

### **How does cosine similarity work, and what are its common applications?**
Cosine similarity measures the similarity between two vectors by calculating the cosine of the angle between them. It's calculated as $\frac{d1 · d2}{||d1|| ||d2||}$, where d1 · d2 is the dot product of the vectors, and ||d|| is the length of vector d. It's particularly useful for document data represented as term-frequency vectors. Applications include information retrieval, biologic taxonomy, and gene feature mapping.

### **What are some common distance measures for numeric data, and how do they differ?**
Common distance measures for numeric data include Minkowski distance, which generalizes several other distances. Special cases of Minkowski distance include Manhattan distance (L1 norm, sum of absolute differences), Euclidean distance (L2 norm, straight-line distance), and supremum distance (Lmax norm, maximum difference between any component). The choice of distance measure depends on the specific application and the desired properties.

### **How are similarity and dissimilarity measured for different attribute types, including nominal, binary, and mixed-type attributes?**
For nominal attributes, simple matching (ratio of matches to total variables) can be used. For binary attributes, different measures like the Jaccard coefficient are used, particularly when asymmetry is present. For mixed-type attributes, a weighted formula can combine the effects of different attribute types, using normalization for numeric attributes and converting ordinal attributes to interval-scaled equivalents.