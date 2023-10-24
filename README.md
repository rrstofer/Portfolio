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

**Overview:** **Overview:** During my undergraduate machine learning course, my partner and I were assigned the task of developing a machine learning model on a topic of our choice. We chose to create a model capable of classifying offenders' races based on data from hate crimes recorded by the FBI Crime Data Explorer from 2010 to 2019. To achieve this, we explored a range of machine learning models, including Random Forest, Naive-Bayes, Boosting, and Logistic Regression. We also created an HTML report that documented our thought processes, offering explanations for exploratory data analysis (EDA), data preprocessing, and model testing and evaluation.

Upon analyzing our results, a noteworthy pattern emerged: our Random Forest model exhibited exceptional accuracy when classifying White offenders but significantly higher errors when dealing with minority groups. This trend was consistent across all our models. The root cause lay in the imbalanced distribution of hate crime offender races, with over 75% being White offenders. Further investigation, including variance importance analysis, revealed that the description of the bias (the type of hate crime offense) held the most significant influence in determining a hate crime offender's race. Ultimately, our best-performing models were Random Forest and Boosting, both with an error rate of approximately 23%.

In conclusion, our project demonstrated that predicting an offender's race using various crime features is feasible; however, it may be inherently biased due to the pronounced disparity in the distribution of crimes among different offender races.

![HC_1](/assets/img/hate_crime_1.PNG)
![HC_2](/assets/img/hate_crime_2.PNG)

**Improvements:**  Considering the uneven distribution of offender races in our dataset, we would have liked to enhance our pipeline to overcome this obstacle if given more time. These improvements would encompass oversampling and data augmentation techniques, stratified data sampling methods, and the implementation of more stringent regularization measures which would all be designed for mitigating the impact of our data imbalance.

**Technical Skills:** Machine Learning, Random Forest, Naive-Bayes, Boosting, Logistic Regression

**Tools:** R, R Markdown

**Team:** Mitchell Rapaport, Ryan Stofer

[![Open Report](https://img.shields.io/badge/HTML-View_Report-green?logo=html5&logoColor=green)](/assets/img/hate_crime_report.html) [![Open Rmd](https://img.shields.io/badge/R-View_Report-green?logo=R&logoColor=green
)](/assets/img/hate_crime_report.Rmd)

