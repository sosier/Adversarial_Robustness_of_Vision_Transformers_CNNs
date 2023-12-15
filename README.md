# Adversarial Robustness of Vision Transformers and Convolutional Neural Networks

Code for the paper "Adversarial Robustness of Vision Transformers and Convolutional Neural Networks" by [Sean Osier](smo2152@columbia.edu) and [Yutong Zhou](yz4429@columbia.edu), Columbia University for COMS 4995: Neural Networks & Deep Learning.

## Abstract

We study the impact of various hyperparameter and training choices on the adversarial robustness of both Vision Transformers and Convolutional Neural Networks. Ultimately, we identify several factors that significantly impact the models’ adversarial accuracy. In particular, normalization (both layer and batch) is extremely detrimental to adversarial robustness. We also find that increasing model size / capacity increases model adversarial robustness up to a particular size, after which it generally provides no further benefit. We additionally confirm the importance of proper model fit (neither under nor overfitting) to maximizing adversarial robustness. Finally, in a simple case-study, we demonstrate how our findings can be applied to dramatically improve the adversarial robustness of a Vision Transformer model over an adversarially naive implementation.

## Key Results

### Vision Transfomer (ViT)

![image](https://github.com/sosier/Adversarial_Robustness_of_Vision_Transformers_CNNs/assets/13408985/bc35e1c4-0bde-4417-939b-b83e962e6c87)

### Convolutional Neural Network (CNN)

![image](https://github.com/sosier/Adversarial_Robustness_of_Vision_Transformers_CNNs/assets/13408985/14be8b43-64d5-4313-bc42-c43ff2d278cb)

## How to Run the Code / Replicate Our Experiments

1. Navigate to the file [Adversarial_Robustness_of_Vision_Transformers_CNNs.ipynb](Adversarial_Robustness_of_Vision_Transformers_CNNs.ipynb)
2. Click the "Open in Colab" button to open the notebook in Google Colab:  
![image](https://github.com/sosier/Adversarial_Robustness_of_Vision_Transformers_CNNs/assets/13408985/5aa79f38-8349-4942-99f5-076213d03ec5)
3. In Google Colab, run the workbook as you would any regular notebook
   - A GPU connection is highly recommended as replicating the experiments will require well over 1,000 model training runs. WARNING: Even with a GPU, replicating all experimental training runs will take many hours of runtime.
   - As such, a Google Drive connection where you can save / persist training run results is also highly recommended, and required if you want to fully replicate our experiments. If you are using the free Google Colab plan you will NOT be able to complete all runs before Google kicks you off, so saving the training results somewhere is critical.
