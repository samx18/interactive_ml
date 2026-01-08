# K-Nearest Neighbors Interactive Simulation Guide

## What You'll Learn

This simulation teaches you how the **k-nearest neighbors (KNN)** algorithm works using a relatable house pricing scenario. You'll understand:

- How computers make predictions based on similar examples
- Why the choice of 'k' (number of neighbors) matters
- How distance calculations work in machine learning
- The concept of "majority voting" in classification

## How to Use the Simulation

### 1. Tabs Overview
- **🎮 Interactive Tab**: Contains the main simulation controls and real-time feedback
- **🧠 Intuition Tab**: Explains the core concepts behind KNN with analogies and examples

### 2. Understanding the Setup
- **Red dots** = Expensive houses (larger size, better location)
- **Blue dots** = Affordable houses (smaller size, lower location scores)
- **X-axis** = House size in square feet (800-3000 sq ft)
- **Y-axis** = Location score (1-10, where 10 is the best location)

### 2. Making Predictions
1. **Click anywhere** on the chart to place a new house
2. Watch as the algorithm:
   - Finds the k nearest neighbors (animated red lines)
   - Shows distance calculations
   - Counts votes from neighbors
   - Makes a prediction

### 3. Experimenting with K
- Use the slider to change the number of neighbors (k = 1 to 15)
- Try different k values for the same house location
- Notice how the prediction might change

## Key Learning Points

### What is K-Nearest Neighbors?
KNN is like asking your neighbors for advice! When you want to know if a house is expensive or affordable, you:
1. Look at the k most similar houses nearby
2. See what category most of them belong to
3. Predict that your house belongs to the majority category

### Why Does K Matter?
- **Low k (1-3)**: Very sensitive to individual data points, might be influenced by outliers
- **High k (7-15)**: More stable predictions, considers broader patterns
- **Too high k**: Might ignore local patterns and always predict the most common category

### Real-World Applications
KNN is used in:
- Recommendation systems (Netflix, Amazon)
- Medical diagnosis
- Image recognition
- Market research
- Credit scoring

## Try These Experiments

1. **Border Exploration**: Click near the boundary between red and blue clusters. How does k affect the prediction?

2. **Outlier Testing**: Click near a single isolated point. What happens with k=1 vs k=7?

3. **Cluster Centers**: Click in the middle of a cluster. Does k matter as much here?

4. **Edge Cases**: Click at the very edges of the chart. How confident should you be in these predictions?

## Understanding the Visualization

- **Animated red lines** show connections to the k nearest neighbors
- **Numbers on lines** show the calculated distances (normalized)
- **Highlighted houses** (thick borders) are the selected neighbors
- **Step-by-step explanations** guide you through the algorithm

## Advanced Concepts (Optional)

### Distance Calculation
The simulation uses **Euclidean distance** with normalized features:
- Both house size and location are scaled to 0-1 range
- This ensures fair comparison between different units
- Distance = √[(size₁-size₂)² + (location₁-location₂)²]

### Limitations to Consider
- KNN assumes similar houses should be close together
- It doesn't work well with irrelevant features
- Performance can be slow with large datasets
- Sensitive to the scale of features

Enjoy exploring the algorithm! The best way to learn is to experiment with different scenarios and observe how the predictions change.