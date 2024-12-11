# Gestalt Principles in Data Visual

## Table of Content
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Getstalt Principle](#getstalt-principle)

## Project Overview
Gestalt Principles in Data Visualization helps create graphs, diagrams, or visualizations that are more intuitive and easy to understand. By leveraging the natural way the human brain organizes visual elements, Gestalt principles can improve the effectiveness of data communication.
This project further explains how the Application of Gestalt Principles in Data Visualization.

## Data Source
The dataset used is [shapes_dataset.csv](https://github.com/user-attachments/files/18090581/shapes_dataset.csv)

The dataset contains the following columns:
- shape: Type of shape (circle, square, triangle).
- color: Color of the shape (red, blue, green, yellow).
- x: X-coordinate of the shape on a grid.
- y: Y-coordinate of the shape on a grid.
- size: Size of the shape (radius for circles, side length for squares, etc.).

## Gestalt Principles
### Similarity
Create a scatter plot where shapes are grouped based on their color or type

Here are the steps to create a scatter plot:
- Load the dataset using pandas
- Each shape is grouped by the shape column using (markers), while the color is determined by the color column. The size of the markers is adjusted by the size column to make the visualization clearer.

![scatter plot](https://github.com/user-attachments/assets/d65d3324-16a4-4df1-81e6-c3852b1f8ecc)

### Proximity
Demonstrate the principle of proximity by clustering shapes

Here are the steps to create a clustering:
- Plot all shapes using x and y coordinates.
- Apply a clustering method using scikit-learn's DBSCAN (Density-Based Spatial Clustering of Applications with Noise) algorithm to find clusters of shapes based on spatial proximity.
  
![clusters](https://github.com/user-attachments/assets/b4d318fe-15eb-45ae-a63f-af91df0d51b9)

Output explanation:
The scatter plot shows the results of proximity clustering using the DBSCAN algorithm. Each cluster is labeled differently (e.g., "Cluster 0" and "Cluster 1"), while points that do not belong to a cluster are considered noise (if any).

### Closure
Create an incomplete shape that visually suggests a complete figure

Here are the steps to create an incomplete shape:
- Select a shape from the dataset to form a rough circle or square, in this case I chose circles.
- Leave a gap to test whether viewers see a closed figure.

![incomplete shape](https://github.com/user-attachments/assets/1fa66e96-3870-4a41-b3d4-1b75a154505b)

Output explanation
I selected circles from the dataset and arranged them in such a way that they formed a pattern resembling a full circle. However, there are gaps or missing parts in the arrangement.
In this image, despite the gaps in the circles, the human brain tends to see the pattern as a complete circle.
With intentional gaps, this experiment tests the extent to which the brain can complete the missing parts.


### Continuity
Illustrate how the human eye follows continuous lines

Here are the steps:
- Identify shapes in the dataset that can form a smooth path.
- Place the shapes in such a way that they resemble curves or continuous lines.
  
![continuous path](https://github.com/user-attachments/assets/3fa2908c-b062-4467-a629-7c65b487a762)

Output explanation:
I used a combination of circular and square shapes arranged in a particular order of position (x, y) to form a path. Black dotted lines are used to show the visual relationship between these shapes.
In this image, the visual path connected by the dotted lines helps the human eye to follow the flow of shapes, even though the shapes are different (circle and square).This shows how humans perceive shapes in the context of a larger pattern, despite changes in shape or color.

