# Optimizing Spatial Sensing Performance with Kriging and SRGAN – A Feasibility Study
 
## Abstract
Several studies have aimed at improving sensor performance through deep learning. In this paper, we explore the feasibility of using advanced machine learning techniques, specifically Kriging and Super Resolution Generative Adversarial Networks, to enhance the performance and accuracy of simulated force sensitive resistor matrices with a low number of sensors. Kriging is a geostatistical method that uses spatial correlations to interpolate or predict values at unsampled locations, while Super Resolution Generative Adversarial Networks (SRGAN) are a type of generative adversarial network that can generate high-resolution (HR) images from low-resolution (LR) inputs. Our results suggest that machine learning techniques can provide a powerful tool for enhancing the accuracy performance (90% Structural Similarity Index) of force sensing technologies, with potential applications in a wide range of fields, especially in autonomous vehicles.<br>

## Link to Paper
[IEEE Publication](https://ieeexplore.ieee.org/document/10325319)

## Directory
1. [Simulation.ipynb](Data_Simulation\04172023_Simulation.ipynb)
- This file contains code to simulate data points (similar to pressure sensors on a car seat)
- This file contains code to apply Ordinary Kriging to convert data points into pressure heatmap images for both LR and HR data points
- The LR images will then be the input while the HR images will be the ground truth images for SRGAN model.

2. [SRGAN.ipynb](SRGAN\SRGAN\SRGAN\04172023_SRGAN.ipynb)
- This file contains code to load and preprocess the heatmap images including tensor transformation and normalization.
- This file contains code to build the SRGAN model.
- This file contains code to train and test the model.
- This file contains the evaluation of the results including structural similarity index and peak signal-to-ratio index.