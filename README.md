# RFB Implementation

Collected data points (x, y pairs) and training on them with both Multi-layer Perceptron (MLP) and Radial Basis Functions (RBF) networks for analysis and comparison.

## Equation

$$y = 1/3 + 0.5.sin(3x.π) + μ\\0 < x < 1\\−0.7 < μ < 0.7$$

# Dataset

<table class="tg">
<tbody>
<tr>
<td>
<p align="center">
<img width="360" src="./images/ds-train.png">
</p></td>
<td>
<p align="center">
<img width="360" src="./images/ds-valid.png">
</p></td></tr>
</tbody>
</table>

# Training

## MLP

To implement MLP, keras library is used.

- Model architecture
<p align="center">
<img src="./images/mlp-arch.png">
</p>

## RBF

To find RBF layer centers, two methods are used:

1. K-Means clustering
2. a Gaussian mixture model probability distribution

The radius is found by finding the maximum distance between each two centers.

# Results

<table class="tg">
<tbody>
<tr>
<td>
<p align="center">
<img width="360" src="./images/res-train.png">
</p></td>
<td>
<p align="center">
<img width="360" src="./images/res-valid.png">
</p></td></tr>
</tbody>
</table>
