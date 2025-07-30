# Radiation-Free Scoliosis Cobb Angle Estimation via X-Ray Guided Unpaired RGB Learning


More details of this project will be released soon.

weights: [![huggingface weights](https://img.shields.io/badge/%F0%9F%A4%97%20Weights-deepang/FLEX-yellow)](https://huggingface.co/deepang/FLEX)&nbsp;

## Network Architecture

![Overview](./figures/overview1.png)

Comparison of scoliosis assessments. (a) RGB-Only: a non-invasive, cost-effective solution, but with limited accuracy due to reliance on surface imaging. (b) X-Ray-only: provides high accuracy for skeletal landmark detection but incurs radiation exposure and higher costs. (c) FLEX: achieves clinical-grade accuracy while remaining radiation-free and cost-efficient, bridging the gap between safety and precision.



## Data Description
### Dataset Name: SCO dataset

Challenge: X-ray Image-Guided RGB Vertebral Landmark Detection and Scoliosis Cobb Angle Estimation

The SCO dataset is the first cross-modal landmark detection dataset for AIS. It is created by recruiting 1001 adolescent participants from Peking Union Medical College Hospital and capturing both RGB visible-light images and X-ray images, resulting in 1001 pairs of cross-modal images (a total of 2002 images). The RGB images are captured at a resolution of 1920×1080 pixels, while the X-ray images have resolutions ranging from 2000×5000 to 3000×8000 pixels, providing high resolution for detailed representation of spinal anatomical structures. The images are obtained under standardized laboratory conditions, with subjects in a full-spine standing position, which accurately reflects the biomechanical characteristics of the spine under weight-bearing conditions and offers a physiological basis for clinical evaluation.

## Benchmark

 Quantitative comparison of vertebral landmark detection performance on the SCO dataset. The performance of three approaches covering unimodal-RGB, unimodal-X-ray and multimodal-unpaired are reported. The performance of FLEX is highlighted in <span style="color:gray;">gray</span>, and the best performance in landmark detection is recorded in <span style="color:red;">red</span>.
![Benchmark](./figures/benchmark1.png)

Quantitative comparison of Cobb angle estimation performance on the SCO dataset.
![Benchmark](./figures/benchmark2.png)

## Visualization
Qualitative visualization of landmark position errors comparing FLEX with other methods. The <span style="color:red;">red</span> dots represent the ground-truth positions, the <span style="color:green;">green</span> dots represent the predicted positions, and the <span style="color:blue;">blue</span> dashed line represents the error distance.
![Benchmark](./figures/landmark_visualization.png)

Qualitative visualization of the Cobb angle estimation of FLEX compared to other methods. The endplate used for estimating the MT, PT, and TL are represented in <span style="color:red;">red</span>.
![Benchmark](./figures/cobb_visualization.png)












