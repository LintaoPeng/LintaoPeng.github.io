---
title: "Research"
permalink: /research/
author_profile: true
---

## Wide-Filed High Resolution Imaging
 Wide-field and high-resolution (HR) imaging are essential for various applications such as aviation reconnaissance, topographic mapping, and safety monitoring. The existing techniques require a large-scale detector array to capture HR images of the whole field, resulting in high complexity and heavy cost. 

In our research, we aim to build an agile wide-field imaging framework with selective high resolution that requires only two detectors. It builds on the statistical sparsity prior of natural scenes that the important targets locate only at small regions of interest (ROI), instead of the whole field. Under this assumption, we use a short-focal camera to image a wide field with a certain low resolution and use a long-focal camera to acquire the HR images of ROI. To automatically locate ROI in the wide field in real time, we propose an efficient deep-learning-based multiscale registration method that is robust and blind to the large setting differences (focal, white balance, etc) between the two cameras. Using the registered location, the long-focal camera mounted on a gimbal enables real-time tracking of the ROI for continuous HR imaging. We demonstrated the novel imaging framework by building a proof-of-concept setup with only 1181 gram weight, and assembled it on an unmanned aerial vehicle for air-to-ground monitoring. 

For detail information, please refer to [Agile wide-field imaging with selective high resolution](https://www.osapublishing.org/oe/fulltext.cfm?uri=oe-29-22-35602)



##  Underwater Image Enhancement
Due to the absorption and scattering of light by water molecules, impurities and suspended matter dissolved in water, underwater images often have poor visual quality. Although existing underwater image enhancement(UIE) methods have achieved nice performance in quantitative evaluation indicators, there are still several major problems:

(1) Due to the lack of large-scale real underwater image datasets covering rich underwater scenes, existing data-driven UIE methods often have unstable performance in complex real underwater scenes.

(2) The existing network methods ignore the inconsistent characteristics of the attenuation degree of the underwater image in the channel dimension and the space dimension.

​	In order to solve the above problems, we first constructed a large-scale underwater image dataset called LSUI  which containing rich underwater scenes and contains 5004 pictures collected from the real underwater world, each with a corresponding reference image. Secondly, we introduced the transformer model to the UIE task for the first time, and inserted channel-wise multi-scale feature fusion tranformer (CMSFFT) and spatial-wise global feature modeling tranforme (SGFMT) on the basis of Unet-Gan. The entire model is named U-shape Transformer. Thirdly, based on the color perception principle of the human eye, we propose a novel multi-color space loss function that combines the advantages of RGB, LAB, and LCH color spaces to calculate network loss to improve the visual quality of our results.

