## 4S-DT: Self-supervised super sample decomposition for transfer learning with application to COVID-19 detection


## Introduction

4S-DT was proposed to overcome the limitations and costs of data annotations for COVID-19 cases by learning visual features from a large set of unlabelled CXR images. 
The model starts by extracting feature representations from the unlabelled CXR images using a stacked autoencoder model. Then, the features are fed into the DBSCAN clustering algorithm to generate pseudo-labels. Third, the pre-trained ResNet-18 network is used for training the pretext task and classifying the pseudolabels. Finally, the learnt features from the pretext model are fine-tuned to a downstream task using a parametric clustering algorithm (k-means) to detect small cases of COVID-19 from CXR images. The model was
evaluated on two CXR datasets with a small number of COVID-19 cases. Due to the limited availability of large publicly accessible COVID-19 datasets at that time,
we used two different CXR labelled datasets referred to dataset-A and dataset-B. 4S-DT achieved a high accuracy of 97.54% and 99.80% for detecting COVID-19 cases in dataset-A and dataset-B, respectively. 

### Requirements
To run this project, you'll need the following dependencies:
- **Python**: 3.8
- **TensorFlow**: Version 2.13
- Other required libraries: 
  - `NumPy`
  - `Matplotlib`
  - `scikit-learn`
  - `OpenCV`

 ## Model Overview
 
<p align="center">
  <img src="https://github.com/ascodeuser/4S-DT-Model/raw/main/image/4S-DT_Model.png" alt="Model Figure" width="750"/>
</p>

### Citation
If you use this code or method in your research, please cite the following paper:


*@article{abbas20214s,
  title={4S-DT: Self-supervised super sample decomposition for transfer learning with application to COVID-19 detection},
  author={Abbas, Asmaa and Abdelsamea, Mohammed M and Gaber, Mohamed Medhat},
  journal={IEEE Transactions on Neural Networks and Learning Systems},
  volume={32},
  number={7},
  pages={2798--2808},
  year={2021},
  publisher={IEEE}
}*


