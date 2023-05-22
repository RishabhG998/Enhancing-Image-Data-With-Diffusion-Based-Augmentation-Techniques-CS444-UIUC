# UIUC-Deep-Learning-for-Computer-Vision-CS444-project

The problem addressed in this project is how to generate more diverse and realistic data to improve the performance
of deep learning models. We investigate the use of diffusion models, a recently proposed generative model, for
data augmentation and compare their performance with other commonly used techniques such as RandAugment,
AutoAugment, MixUp, CutOut, and CutMix.

Our line of attack involves using an off-the-shelf diffusion model to generate training dataset, which is then used to train a ResNet-based model. The system architecture for augmenting data involves adapting the diffusion model to
images of new concepts through multi-class textual inversion. The system generates M augmented versions of each
image in the dataset using a pretrained stable diffusion checkpoint.

We find that diffusion-based data augmentation coupled with MixUp can outperform other techniques in terms of
accuracy and generalization on the chosen dataset, especially when the amount of training data is limited. The results show an improvement of more than 5% over the baseline on the PASCAL VOC dataset. These results suggest that
diffusion models have the potential to become a valuable tool for data augmentation in deep learning.
