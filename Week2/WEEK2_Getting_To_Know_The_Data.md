# **Getting to Know Your Data**
This includes data objects, attribute types, basic statistical descriptions, data visualization techniques, and measures of data similarity and dissimilarity.

### **1. Data Objects and Attributes**

**Data Object** represent **entities** in a dataset (e.g., customers, patients, students). These are also referred to as **samples**, **examples**, **instances**, **data points**, **objects**, or **tuples**. 

*"Data sets are made up of data objects... A data object represents an entity."*

**Attributes** describe **the characteristics of data objects** (e.g., customer_ID, name, address). Attributes are also known as **dimensions**, **features**, or **variables**.

**Attribute types**
- **Nominal**: Categories or names (e.g., hair color, marital status).
- **Binary**: Two states (0 and 1). Can be symmetric (gender) or asymmetric (medical test result). 
- **Ordinal**: Meaningful order, but magnitude between values is unknown (e.g., size {small, medium, large}, grades, education levels). 

*"Values have a meaningful order (ranking) but magnitude between successive values is not known."*

**Numeric types - Quantitative values**
- **Interval**: Equal-sized units, order, but no true zero-point (e.g., temperature in Celsius, calendar dates).
- **Ratio**: Inherent zero-point, allowing for magnitude comparisons (e.g., temperature in Kelvin, length, monetary quantities).
- **Discrete**: Finite or countably infinite values (e.g., zip codes, words in a document).
- **Continuous**: Infinite values within a range (e.g., temperature, weight).

### **2. Types of data sets**
- **Record Data**: Most common, including **relational records**, **data matrices**, **document data (term-frequency vectors)**, and **transaction data**.
- **Graph and Network Data**: Examples include the **World Wide Web**, **social networks**, **web graphs**, and **molecular structures**.
- **Ordered Data**: Sequences of data, including **video data**, **temporal data (time series)**, **sequential data (transaction sequences)**, **genetic sequence data**, and **spatial/image/multimedia data**.

**Important characteristics of structured data**
- **Dimensionality**: Number of attributes and challenges arising from high dimensionality.
- **Sparsity**: Only presence of data counts.
- **Resolution**: Patterns depend on the scale.
- **Distribution**: Centrality and dispersion of data.

### **3. Statistical Descriptions of Data**

**Purpose**: To better understand the data, we have central tendency, variation, and spread.

**Central Tendency Measures**
- Mean $\rightarrow$ average value
- Weighted Mean $\rightarrow$ average value considering weights
- Trimmed Mean $\rightarrow$ mean after removing extreme values
- Median $\rightarrow$ middle value
- Mode $\rightarrow$ most frequent value

**Dispersion Measures**
- **Variance and Standard Deviation** $\rightarrow$  Measures of data spread around the mean
- **Quartiles** $\rightarrow$ Q1 (25th percentile), Q3 (75th percentile)
- **Inter-Quartile Range (IQR)** $\rightarrow$ Q3 - Q1
- **Five-Number Summary** $\rightarrow$ Min, Q1, Median, Q3, Max
- **Boxplot** $\rightarrow$ Visual representation of the five-number summary, with outliers

**Data Distribution**
- **Symmetric vs. Skewed Data** $\rightarrow$ understanding how data is distributed around the mean. 

Positively skewed data has a long tail on the right, while negatively skewed data has a long tail on the left.

### **4. Data Visualization Techniques**

**Purpose**: Gain insights into an information space by mapping data onto graphical primitives, identify patterns, trends, structure, irregularities, relationships among data.

**Categorization of Techniques**
- **Pixel-Oriented** $\rightarrow$ maps dimension values to pixels
- **Geometric Projection** $\rightarrow$ uses transformations and projections (e.g., scatterplots, landscapes, parallel coordinates)
- **Icon-Based** $\rightarrow$ represents data values as features of icons (e.g., Chernoff faces, stick figures)
- **Hierarchical** $\rightarrow$ partitions data into subspaces (e.g., dimensional stacking, tree-maps)

**Specific Visualization Methods**
- **Boxplots** $\rightarrow$ display the five-number summary and outliers
- **Histograms** $\rightarrow$ show the distribution of frequencies
- **Quantile Plots** $\rightarrow$ show the data's behavior and unusual occurrences
- **Q-Q Plots** $\rightarrow$ compare quantiles of two distributions
- **Scatter Plots** $\rightarrow$ show relationships between two variables. "Provides a first look at bivariate data to see clusters of points, outliers, etc."
- **Landscapes** $\rightarrow$ visualizes data as a perspective landscape
- **Parallel Coordinates** $\rightarrow$ displays each data item as a polygonal line intersecting axes representing attribute values
- **Chernoff Faces** $\rightarrow$ uses facial features to represent data dimensions.
- **Stick Figures** $\rightarrow$ uses stick figures with varying limb angles/lengths to represent data dimensions
- **Dimensional Stacking** $\rightarrow$ partitions the attribute space into 2D subspaces
- **Tree-Maps** $\rightarrow$ hierarchical partitioning of the screen
- **InfoCubes** $\rightarrow$ 3D visualization using nested semi-transparent cubes
- **Cone Trees** $\rightarrow$ 3D visualization of hierarchical information

### **5. Measuring Similarity and Dissimilarity**
- **Similarity** $\rightarrow$ numerical measure of how alike two data objects are. Higher values indicate greater similarity
- **Dissimilarity (Distance)** $\rightarrow$ numerical measure of how different two data objects are. Lower values indicate greater similarity
- **Proximity** $\rightarrow$ a general term referring to either similarity or dissimilarity

**Data Matrix vs. Dissimilarity Matrix** $\rightarrow$ data matrix stores attribute values, while the dissimilarity matrix stores distances between data points

**Proximity Measures for Different Attribute Types**
- **Nominal** $\rightarrow$ simple matching
- **Binary** $\rightarrow$ contingency table, distance measures (symmetric and asymmetric), Jaccard coefficient
- **Numeric** $\rightarrow$ standardization (Z-score)
- **Minkowski Distance**  $\rightarrow$ a general distance measure that includes **Manhattan**, **Euclidean**, and **Supremum** distances as special cases
    - **Euclidean & Manhattan Distance** $\rightarrow$ numeric data comparison
    - **Jaccard Coefficient** $\rightarrow$ binary attribute similarity.
    - **Cosine Similarity** $\rightarrow$ text/document similarity. Measures the cosine of the angle between two vectors.

- **Ordinal** $\rightarrow$ rank-based methods
- **Mixed Type** $\rightarrow$ weighted formula to combine effects of different attribute types

### **Key Takeaways**

- Understanding the types of data and their attributes is crucial for effective data mining
- Statistical descriptions and visualizations provide insights into data characteristics
- Choosing appropriate similarity and dissimilarity measures is essential for tasks like clustering and classification
- This chapter lays the groundwork for data preprocessing, a critical step in the data mining process

This document provides a structured overview of fundamental concepts in data mining, focusing on understanding data before performing any analysis. Further chapters will build upon these concepts to explore preprocessing, pattern discovery, and advanced mining techniques.