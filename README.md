# Flow Pattern Classifier
This is a Python script that generates synthetic data for flow pattern classification based on different parameters and then uses a Decision Tree classifier to predict the flow pattern based on the input parameters.

## Flow Patterns
Flow patterns refer to the different types of flow regimes that can be observed in a multiphase flow. The flow pattern is determined by various parameters such as fluid densities, viscosities, flow rates, pipe diameters, and surface tension. The four main types of flow patterns that can be observed in a two-phase flow are:

- Bubble flow: In this flow pattern, gas bubbles are dispersed in the liquid phase in a random manner.
- Intermittent flow: This flow pattern is characterized by the presence of large bubbles or slugs of gas separated by liquid plugs.
- Stratified flow: In this flow pattern, the liquid and gas phases are separated by a distinct interface.
- Annular flow: This flow pattern is characterized by the presence of a continuous gas phase surrounding a thin liquid film on the pipe wall.

## Synthetic Data Generation
The script generates synthetic data for flow pattern classification by randomly selecting values for the different parameters such as oil density, gas density, oil viscosity, gas viscosity, surface tension, flow rate, and pipe diameter. The ranges for these parameters are defined at the beginning of the script. Based on the parameter values, the script then calculates the Reynolds number, Froude number, and Weber number for the flow, which are used to classify the flow pattern.

## Data Visualization
After generating the synthetic data, the script visualizes the distribution of the target variable (flow pattern) using a histogram. It's always a good idea to start by looking at the distribution of the target variable to see if there is any class imbalance or other issues.

The script also creates a correlation matrix and a pair plot to visualize the correlation between the different parameters and the target variable. The correlation matrix shows the correlation coefficients between the different pairs of parameters, while the pair plot shows the pairwise relationships between the different parameters.

## Decision Tree Classifier
Finally, the script splits the data into training and testing sets, trains a Decision Tree classifier on the training set, and evaluates the accuracy of the classifier on the testing set. The accuracy is printed to the console.

Overall, this script is a simple example of how synthetic data generation and machine learning can be used to classify flow patterns based on different parameters.
