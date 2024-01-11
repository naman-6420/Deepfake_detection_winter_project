## DeepFake-Image-Detection
Tried to replicate the results of research papers attached in the repo to classify real and AI-generated images.

Implemented the hierarchical multi-level approach mentioned in paper 2 where each level results are as follows:

Level-1: To classifiy real class from fake class Achieves 54% accuracy to detect real and Fake Images (Trained on Dalle generated fake images and Laiom Real images and tested on Biggan generated fake images).

Level-2: The model trained for detecting the source of Fake image(GANs vs DMs) achieves a Testing Accuracy of 63%(Trained on dalle and biggan).

Level-3: To determine class from each gan models(9) and diffusion models(4) , (achieved max accuracy of 48% training and testing on the 4 different diffusion models).

In each level a pretrained ResNet50 classifier was used with FCNN layers added in the end for respective classification task, along with fine tuning or unfreezing some layers of ResNet50 to train it to our specific task.
All the above models are still under work, and constant attempt is being made to replicate accuracy of the reasearch papers.

## Datasets Used:

Diffusion Models: [Link](https://drive.google.com/file/d/1FXlGIRh_Ud3cScMgSVDbEWmPDmjcrm1t/view)

GAN's: [Link](https://drive.google.com/file/d/1z_fD3UKgWQyOTZIBbYSaQ-hz4AzUrLC1/view)




