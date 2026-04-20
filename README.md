# EGGA-Error-Guided-Generative-AI-and-Optimized-Machine-Learning-based-Intrusion-Detection-System

This repository includes code for the paper ["EGGA: An Error-Guided Generative Augmentation and Optimized ML-Based IDS for EV Charging Network"](https://www.mdpi.com/1999-5903/18/4/202) published in Future Internet.

Authors: Li Yang (liyanghart@gmail.com) and G. Kirubavathi

Organizations: 
- The Advanced Networking Technology and Security (ANTS) Lab, Faculty of Business and IT, Ontario Tech University.
  - GitHub Account: [ANTS-OntarioTechU](https://github.com/ANTS-OntarioTechU)

The paper is publicly available at: [Paper link](https://www.mdpi.com/1999-5903/18/4/202)

## Abstract of The Paper
Electric Vehicle Charging Systems (EVCSs) are increasingly connected with the Internet of Things (IoT) and smart grid infrastructure, yet they face growing cyber risks due to expanded attack interfaces. These systems are vulnerable to various attacks that potentially impact both charging operations and user privacy. Intrusion Detection Systems (IDSs) are essential for identifying suspicious activities and mitigating risks to protect EVCS networks, but conventional ML-based IDSs are often unable to achieve optimal performance due to imbalanced datasets, complex traffic distributions, and human design limitations. In practice, EVCS traffic is typically multi-class, imbalanced, and safety-critical, where both missed attacks and false alarms can lead to denial of charging, service interruption, unnecessary incident escalation, financial loss, and reduced user trust. Automated ML (AutoML) and Generative Artificial Intelligence (GAI) have emerged as promising solutions in cybersecurity. Existing GAI and augmentation methods are mostly class-frequency-driven, but this does not necessarily improve the error-prone regions where IDSs actually fail. In this paper, we propose a GAI and an AutoML-based IDS that incorporates a Conditional Generative Adversarial Network (cGAN) with the optimized XGBoost model to improve the effectiveness of intrusion detection in EVCS networks and IoT systems. The proposed framework involves two techniques: (1) a novel cGAN-based error-guided generative augmentation (EGGA) method that extracts misclassified samples and generates a more robust training set for IDS development, and (2) an optimized IDS model that automatically constructs an optimized XGBoost model based on Bayesian Optimization with Tree-structured Parzen Estimator (BO-TPE). The main algorithmic novelty lies in EGGA, which uses model errors to guide generative augmentation toward difficult decision regions, while the overall pipeline represents a practical system-level integration of EGGA, XGBoost, and BO-TPE. To the best of our knowledge, this is the first work that combines GAI and AutoML to specifically improve detection on hard samples, enabling more autonomous and reliable identification of diverse cyber attacks in EV charging networks and IoT systems. Experiments are conducted on two benchmark EVCS and cybersecurity datasets, CICEVSE2024 and CICIDS2017, demonstrating consistent and statistically meaningful improvements over state-of-the-art IDS models. This research highlights the importance of combining automation, generative balancing, and optimized learning to strengthen cybersecurity solutions for EV charging networks and IoT systems.  

**Keywords**: cybersecurity; Intrusion Detection System; generative AI; conditional GAN; AutoML; XGBoost; Bayesian Optimization; data augmentation; EV Charging Systems; CICEVSE2024; CICIDS2017

<p float="left">
  <img src="https://github.com/LiYangHart/EGGA-Error-Guided-Generative-AI-and-Optimized-Machine-Learning-based-Intrusion-Detection-System/blob/main/Graphical_Abstract.jpg" width="1000" />
</p>

## List of Contributions

The contributions of this paper are summarized as follows:
1. It proposes EGGA, a novel error-guided generative augmentation strategy that identifies misclassified samples during cross-validation and uses a cGAN model to generate hard case-focused synthetic data and strengthen error-prone decision regions.
2. It proposes an AutoML-based optimized XGBoost model using BO-TPE for maximizing intrusion detection performance.
3. It designs a multi-stage closed-loop IDS pipeline for EV charging networks that tightly integrates a strong base learner, error-guided generative augmentation, and automated model tuning, enabling more autonomous and robust detection under imbalanced, multi-class, and nonstationary EVCS network traffic.
4. It evaluates the performance of the proposed IDS on two benchmark public cybersecurity datasets, CICEVSE2024 [13] and CICIDS2017 [14], and compares the performance with state-of-the-art GAI and optimized ML models.


## Implementation

### Machine Learning Algorithms  
* XGBoost  

### Proposed Method for Detection Error Correction
* Conditional GAN (cGAN)-based Error-Guided Generative Augmentation (EGGA)

### Optimization/AutoML Algorithms  
* Bayesian Optimization with Tree-structured Parzen Estimator (BO-TPE)

### Datasets 
1. CICIDS2017 dataset, a popular network traffic dataset for intrusion detection problems
   * Publicly available at: https://www.unb.ca/cic/datasets/ids-2017.html  
   
2. CICEVSE2024 dataset, a state-of-the-art EV charging network security dataset
   * Publicly available at: https://www.unb.ca/cic/datasets/evse-dataset-2024.html
* PS: Subsets are in the ["Data"](https://github.com/LiYangHart/EGGA-Error-Guided-Generative-AI-and-Optimized-Machine-Learning-based-Intrusion-Detection-System/tree/main/Data) Folder

### Code  
* [EGGA_AutoML_IDS_Dataset_1.ipynb](https://github.com/LiYangHart/EGGA-Error-Guided-Generative-AI-and-Optimized-Machine-Learning-based-Intrusion-Detection-System/blob/main/EGGA_AutoML_IDS_Dataset_1.ipynb): code for the sampled CICIDS2017 dataset.  
* [EGGA_AutoML_IDS_Dataset_2.ipynb](https://github.com/LiYangHart/EGGA-Error-Guided-Generative-AI-and-Optimized-Machine-Learning-based-Intrusion-Detection-System/blob/main/EGGA_AutoML_IDS_Dataset_2.ipynb): code for the sampled CICEVSE2024 dataset.

### Requirements  
* Python 3.7+ 
* [scikit-learn](https://scikit-learn.org/stable/)  
* [hyperopt](https://github.com/hyperopt/hyperopt)  
* [Xgboost](https://xgboost.readthedocs.io/en/latest/python/python_intro.html)
* [Tensorflow](https://www.tensorflow.org/install/gpu)
* [Keras](https://keras.io/)  

## Contact-Info
Please feel free to contact me for any questions or cooperation opportunities. I'd be happy to help.
* Email: [liyanghart@gmail.com](mailto:liyanghart@gmail.com)
* GitHub: [LiYangHart](https://github.com/LiYangHart)  
* LinkedIn: [Li Yang](https://www.linkedin.com/in/li-yang-phd-65a190176/)  
* Google Scholar: [Li Yang](https://scholar.google.com.eg/citations?user=XEfM7bIAAAAJ&hl=en)

## Citation
If you find this repository useful in your research, please cite this article as:  

Yang, L.; Kirubavathi, G. EGGA: An Error-Guided Generative Augmentation and Optimized ML-Based IDS for EV Charging Network Security. _Future Internet_ **2026**, 18, 202. https://doi.org/10.3390/fi18040202  

```
@Article{fi18040202,
AUTHOR = {Yang, Li and Kirubavathi, G.},
TITLE = {EGGA: An Error-Guided Generative Augmentation and Optimized ML-Based IDS for EV Charging Network Security},
JOURNAL = {Future Internet},
VOLUME = {18},
YEAR = {2026},
NUMBER = {4},
ARTICLE-NUMBER = {202},
URL = {https://www.mdpi.com/1999-5903/18/4/202},
ISSN = {1999-5903},
DOI = {10.3390/fi18040202}
}
```
