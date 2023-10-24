# Ryan Stofer's Portfolio

---
---

### Education
M.S. - Data Science, University of California, Irvine (Expected _December 2024_)
B.S. - Applied Mathematics & Statistics and Data Science, University of California, Santa Barbara (_June 2023_)

___

### Capstone: Deep Learning X-ray Diffraction Model 
(_January 2023 – June 2023_)

**Overview:** As part of the UCSB Capstone program, my group and I partnered with the Stanford Synchrotron Radiation Lightsource (SLAC SSRL), a division of SLAC National Accelerator Laboratory, to research and develop a deep learning model capable of classifying the resolution of individual X-ray diffraction shots.

We divided our project into two teams, each focused on a specific aspect of multi-task learning model development. One team developed a CNN for classifying images as single- or multi-lattice, while my team created a CNN to predict image resolution. Using a ResNet-based architecture, both teams achieved significant success in model performance. Our multi-lattice detection  CNN achieved 94% accuracy, and the resolution quantification CNN attained a 0.96 Pearson correlation value on simulated data, with high qualitative performance observed on experimental data. This project demonstrates the potential of deep learning in addressing the data rate challenge in protein crystallography.

![Capstone_Poster](/assets/img/SLAC_Poster.png)

**Improvements:** If allotted more time, we would have liked to extend our work further by testing our model on more real user data and assessing its performance on both tasks. Furthermore, we could also look into implementing more image artifacts to our simulated data sets to increase the variation in our data.


**Technical Skills:** Convolutional Neural Network, Deep Learning, PyTorch, TensorFlow

**Tools:** Python, CUDA

**Team:** Aleksander Cichosz, Vardan Martirosyan, Teo Zeng, Ryan Stofer

[![Open Poster](https://img.shields.io/badge/PDF-View_Poster-green?logo=googledocs&logoColor=green)](https://github.com/rrstofer/rrstofer.github.io/blob/main/assets/img/SLAC_Poster.pdf) [![Open Repository](https://img.shields.io/badge/GitHub-View_Repository-green?logo=GitHub&logoColor=green)]([https://github.com/rrstofer/rrstofer.github.io/blob/main/assets/img/SLAC_Poster.pdf](https://github.com/dermen/resonet))

___

### Super Resolution of Land Surface Temperature (LST) images 
(_May 2022 – September 2023_)

**Overview:** I led a collaborative research project with a graduate student where we trained a U-Net-based convolutional neural network (CNN) to improve the resolution of coarse remote sensing data by utilizing high-resolution RGB imagery. 

To overcome the challenge of acquiring extensive ground truth data for CNN training, we introduced an innovative pre-training procedure. This method involved applying a randomized function to the RGB images, generating synthetic high-resolution data with varying relationships to the RGB bands. This allowed the model to learn from the abundant high-resolution RGB data before specializing in super resolution tasks. Our approach's effectiveness was demonstrated by comparing our deep learning model to a pixel-based statistical downscaling method. By using a deep learning model, we reduce the need for airborne ground truth data, providing a practical solution to enhance the resolution of coarse remote sensing data, especially when research demands exceed current resolution capabilities.

I presented our work at the Fall 2022 American Geophysical Union conference in Chicago.

![AGU Poster](/assets/img/AGU_Poster.png)

**Improvements:** Given additional time, I would have aimed to introduce increased intricacy into both the randomization function within the pre-training process (such as incorporating non-linear transformations and adding Gaussian noise) and the overall U-Net model (by considering enhancements like the Laplace filter and deeper layers). These modifications could have been explored to further refine our ability to enhance pixel unmixing, particularly at the boundaries of distinct semantic regions.


**Technical Skills:** Convolutional Neural Network, Deep Learning, PyTorch, TensorFlow

**Tools:** Python, R

**Team:** Anna Boser, Ryan Stofer

[![Open Poster](https://img.shields.io/badge/PDF-View_Poster-green?logo=googledocs&logoColor=green)](https://github.com/rrstofer/rrstofer.github.io/blob/main/assets/img/AGU_Poster.pdf) [![Open Repository](https://img.shields.io/badge/GitHub-View_Repository-green?logo=GitHub&logoColor=green)](https://github.com/ecohydro/lst-super-res)

### National Hate Crime Model

**Overview:** As part of my machine learning course for my undergrad, we were tasked with developing a machine learning model regarding any topic of choice. So, I collaborated with a partner to create a machine learning model that is able to classify the offender's race given all recorded hate crimes in 2010-2019 from the FBI Crime Data Explorer.

We ran a variety of models inclduing Random Forest, Naive-Bayes, Boosting, and Logistic Regression in order to classify an offender's race. We created an HTML report that goes over our thought processes and shows line-by-line explanation for EDA, data-processing, and model testing and evaluation.

![HC_1](/assets/img/hate_crime_1.PNG)
![HC_2](/assets/img/hate_crime_2.PNG)

[![Open Report](https://img.shields.io/badge/HTML-View_Report-green?logo=html5&logoColor=green)](/assets/img/hate_crime_report.html)
[![Open Rmd](https://img.shields.io/badge/R-View_Report-green?logo=R&logoColor=green
)](/assets/img/hate_crime_report.Rmd)

**Team:** Mitchell Rapaport, Ryan Stofer
