# GAN
A generative adversarial network (GAN) is a class of machine learning frameworks and a prominent framework for approaching generative AI. The concept was initially developed by Ian Goodfellow and his colleagues in June 2014.In a GAN, two neural networks contest with each other in the form of a zero-sum game, where one agent's gain is another agent's loss.

# CycleGAN
The model architecture is comprised of two generator models: one generator (Generator-A) for generating images for the first domain (Domain-A) and the second generator (Generator-B) for generating images for the second domain (Domain-B).  

Domain-B -> Generator-A -> Domain-A  
Domain-A -> Generator-B -> Domain-B  
Each generator has a corresponding discriminator model (Discriminator-A and Discriminator-B). The discriminator model takes real images from Domain and generated images from Generator to predict whether they are real or fake.  

Domain-A -> Discriminator-A -> [Real/Fake]  
Domain-B -> Generator-A -> Discriminator-A -> [Real/Fake]  
Domain-B -> Discriminator-B -> [Real/Fake]  
Domain-A -> Generator-B -> Discriminator-B -> [Real/Fake]  
  
I use CycleGAN to achieve the transformation of human face caricature, Summer to Winter and Day to Night  
  ![image](https://github.com/wendellgithub0206/cycleGAN/assets/61726383/91127097-a849-4591-83b9-0e069b1d87b5)
# Dataset
[Selfie2anime](https://www.kaggle.com/datasets/arnaud58/selfie2anime)  
[Day2Night](https://www.kaggle.com/datasets/heonh0/daynight-cityview)  
[Summer2Winter](https://www.kaggle.com/datasets/balraj98/summer2winter-yosemite)  





