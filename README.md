# MV-DEFEAT

This repository provides the code for our paper "An evidential deep learning framework for multi-view mammogram analysis"



### Introduction

We proposed a multi-view deep evidential neural network approach for assessment of mammograms by aggregating multiple views of a mammogram, utilizing the potential of Dempster-Shafer evidential theory and combination rule to handle uncertain or conflicting evidence. 


<div align=center><img width="900" height="400" alt="MV-DEFEAT" src="images/mv_defeat.png"/></div>

The main objectives of the proposed approach are to enhance the precision and reliability of the mammogram density assessment by using a multi-view method and an
evidential optimization loss function. The main contributions of this study are as follows:
1. Performing extensive experiments to identify the optimal pre-trained CNN model for mammogram assessment task.
2. Extending the pre-trained CNN backbone architecture by incorporating evidential layers.
3. Developing a multi-view deep evidential neural network trained with a multi-view evidential loss function
4. Demonstrating the proposed model’s generalization and transferability capabilities on unseen datasets.

We conducted experiments on two open-source digital mammogram datasets, VinDr-Mammo and DDSM, which include 4,977 and 1,885 mammogram examinations, respectively. In addition, we validated MV-DEFEAT generalization and transferability capabilities on two independent datasets, CMMD and VTB, with 826 and 765 mammogram examinations, respectively.

### Requirements

python
Pytorch (enabled with CUDA), torchvision
Matplotlib, seaborn, scikitplot
scikit-learn
numpy
pandas
munch
yml
tqdm
Pillow
timm 

### Training and evaluation

Please, change the config file path for dataset path. Create log file folder to save the model path. 

Training: 'python train.py --config_path ddsm_ipsilateral_config.yml'
Evaluation: 'python evaluate.py'



## Contact
For any questions or further information, please contact hamid.behravan@uef.fi.

License: CC BY-NC 4.0


## Citation
Please cite the following work:
Gudhe, N. R., Mazen, S., Sund, R., Kosma, V. M., Behravan, H., & Mannermaa, A. (2024).  "A Multi-View Deep Evidential Learning Approach for Mammogram Density Classification," in IEEE Access, vol. 12, pp. 67889-67909, 2024, doi: 10.1109/ACCESS.2024.3399204. 

### Acknowledgement

Part of the code is borrowed from https://github.com/hanmenghan/TMC



