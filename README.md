# Ryan Stofer's Portfolio

---
---

### IMD Solutions Inc. - GlucoGuard
(_Jan 2024 - June 2024_)

**Overview:** I collaborated with a team to develop a predictive model and an application for IMD solutions Inc.'s newest product, GlucoGuard, aimed at individuals with type 1 diabetes. GlucoGuard continuously monitors glucose levels and administers glucose during nocturnal hypoglycemia to prevent low blood sugar events during sleep. The project included two key components: a predictive model and a user application.

The predictive model was designed to forecast hypoglycemic events, particularly during sleep. I created a logistic regression model due to its efficiency and effectiveness, given the limited feature set of the data. In the absence of actual patient data, we utilized CGM data from Kaggle and achieved a precision of 93.1% across 50 user data sets. The code was structured for easy deployment within the app, ensuring seamless integration with the device’s functionality.

![Gluco_ML](/assets/img/Prediction_Modeling.png)

The user application was developed to provide a user-friendly interface that connects to the device's API. This application allows users to monitor their glucose levels and receive alerts, enhancing their experience and safety when using GlucoGuard.

![Gluco_Wireframe](/assets/img/Glucoguard_Wireframe.png)

**Improvements:** While the model demonstrated promising results with experimental data, testing and retraining the model using actual patient data obtained from the GlucoGuard mouthpiece would enhance its accuracy and reliability. Additionally, incorporating more metadata could enable the development of more complex models, such as a time series model like SARIMA, which could further improve the prediction of hypoglycemic events and provide deeper insights into glucose level trends over time.

**Technical Skills:** Machine Learning, Logisitic Regression

**Tools:** Python, React Native

**Team:** Mina Yoon, Aashi Singh, Sophia Zhang, Ryan Stofer

_**Specifics and files are not shared for confidentiality purposes.**_

[![Open Poster](https://img.shields.io/badge/PPT-View_Poster-green?logo=googledocs&logoColor=green)](https://github.com/rrstofer/rrstofer.github.io/blob/main/assets/img/MADO_Presentation_GlucoGuard.pptx) 

---

### 2024 SoCal RUG Hackathon - Analyzing Linguistic Isolation in California
(_April 2024_)

**Overview:** I participated in a 36-hour hackathon where my team and I analyzed IPUMS US Census data to extract meaningful insights. Given the vast amount of data and the limited time frame, we focused on the variable "linguistic isolation." Linguistic isolation is defined as households where no person aged 14 or older speaks only English at home, or no person aged 14 or older who speaks a language other than English at home speaks English "very well." This definition applies to both the U.S. and Puerto Rican censuses as well as the ACS and PRCS. Our goal was to analyze how linguistic isolation trends across different states in the U.S. over the years.

We concentrated on the top five and bottom four states, discovering notable trends in California. Additionally, we performed some geospatial analysis by plotting the data from 2014 and 2022 across different IPUMS regions, highlighting a significant decline in linguistic isolation in the Southeast, Orange County/LA County, and the Bay Area. To further our analysis, we attempted to use a random forest model to predict linguistic isolation and identify key covariates. Although the model fit poorly, we found that occupation type was a primary factor in determining linguistic isolation.

![SoCalRug_Presentation_1](/assets/img/State_Ling_Iso.pdf)

![SoCalRug_Presentation_2](/assets/img/CA_Ling_Iso.pdf)

**Insights:**

Despite the constraints of the hackathon, our project provided valuable insights into linguistic isolation trends in the U.S. Our analysis revealed significant regional variations, with California showing the most notable trends. The comparison between 2014 and 2022 data indicated a marked decline in linguistic isolation in specific regions, particularly in the Southeast, Orange County/LA County, and the Bay Area. This trend suggests a potential improvement in English proficiency or demographic shifts in these areas.

Our attempt to predict linguistic isolation using a random forest model, although not highly successful, underscored the importance of occupation type as a key covariate. This insight points to the potential influence of employment sectors and economic opportunities on linguistic isolation.

**Improvements:**
For future research, a deeper exploration into feature selection and model optimization could enhance the predictive power of our models. Investigating the underlying causes of the drastic decline in linguistic isolation in certain IPUMS areas over the eight-year interval would also be valuable. Applying an interrupted time series analysis could help identify events or policy changes that contributed to this decline, providing a more comprehensive understanding of the factors driving linguistic isolation trends.

**Technical Skills:** Data Visualization

**Tools:** R, arrow

**Team:** Kabir Snell, Peyton Politewicz, Steven Yang, Ryan Stofer

[![Open Poster](https://img.shields.io/badge/PDF-View_Poster-green?logo=googledocs&logoColor=green)](https://github.com/rrstofer/rrstofer.github.io/blob/main/assets/img/RUG_Hackathon_04-2024.pdf) 

---

### Super Resolution of Land Surface Temperature (LST) images 
(_May 2022 – September 2023_)

**Overview:** I led a collaborative research project with a graduate student where we trained a U-Net-based convolutional neural network (CNN) to improve the resolution of coarse remote sensing data by utilizing high-resolution RGB imagery. 

To overcome the challenge of acquiring extensive ground truth data for CNN training, we introduced an innovative pre-training procedure. This method involved applying a randomized function to the RGB images, generating synthetic high-resolution data with varying relationships to the RGB bands. This allowed the model to learn from the abundant high-resolution RGB data before specializing in super resolution tasks. We compared our deep learning approach's effectiveness against a pixel-based statistical downscaling method and noticed a significant improvement of around 28% for its R^2 value. By using a deep learning model, we reduce the need for airborne ground truth data, providing a practical solution to enhance the resolution of coarse remote sensing data, especially when research demands exceed current resolution capabilities.

I presented our work at the Fall 2022 American Geophysical Union conference in Chicago.

![AGU Poster](/assets/img/Model_Figure.png)

**Improvements:** I would have aimed to introduce increased intricacy into both the randomization function within the pre-training process (such as incorporating non-linear transformations and adding Gaussian noise) and the overall U-Net model (by considering enhancements like the Laplace filter and deeper layers). These modifications could have been explored to further refine our ability to enhance pixel unmixing, particularly at the boundaries of distinct semantic regions.


**Technical Skills:** Convolutional Neural Network, Deep Learning, PyTorch, TensorFlow

**Tools:** Python, R

**Team:** Anna Boser, Ryan Stofer

[![Open Poster](https://img.shields.io/badge/PDF-View_Poster-green?logo=googledocs&logoColor=green)](https://github.com/rrstofer/rrstofer.github.io/blob/main/assets/img/AGU_Poster.pdf) [![Open Repository](https://img.shields.io/badge/GitHub-View_Repository-green?logo=GitHub&logoColor=green)](https://github.com/ecohydro/lst-super-res)

___

### UCSB Capstone - Deep Learning X-ray Diffraction Model 
(_January 2023 – June 2023_)

**Overview:** As part of the UCSB Capstone program, my group and I partnered with the Stanford Synchrotron Radiation Lightsource (SLAC SSRL), a division of SLAC National Accelerator Laboratory, to research and develop a deep learning model capable of classifying the resolution of individual X-ray diffraction shots.

We divided our project into two teams, each focused on a specific aspect of multi-task learning model development. One team developed a CNN for classifying images as single- or multi-lattice while my team created a CNN to predict image resolution. Using a ResNet-based architecture, both teams achieved significant success in model performance. Our multi-lattice detection  CNN achieved 94% accuracy, and the resolution quantification CNN attained a 0.96 Pearson correlation value on simulated data, with high qualitative performance observed on experimental data. This project demonstrates the potential of deep learning in addressing the data rate challenge in protein crystallography.

![Capstone_Poster](/assets/img/SLAC_1.png)
![Capstone_Poster](/assets/img/SLAC_2.png)

**Improvements:** We would like to extend our work further by testing our model on more real user data and assessing its performance on both tasks. Furthermore, we could also look into implementing more image artifacts to our simulated data sets to increase the variation in our data.


**Technical Skills:** Convolutional Neural Network, Deep Learning, PyTorch, TensorFlow

**Tools:** Python, CUDA

**Team:** Aleksander Cichosz, Vardan Martirosyan, Teo Zeng, Ryan Stofer

[![Open Poster](https://img.shields.io/badge/PDF-View_Poster-green?logo=googledocs&logoColor=green)](https://github.com/rrstofer/rrstofer.github.io/blob/main/assets/img/SLAC_Poster.pdf) [![Open Repository](https://img.shields.io/badge/GitHub-View_Repository-green?logo=GitHub&logoColor=green)](https://github.com/dermen/resonet)

___

### National Hate Crime Model
(_January 2022 - March 2022_)

**Overview:** During my undergraduate machine learning course, my partner and I were assigned the task of developing a machine learning model on a topic of our choice. We chose to create a model capable of classifying offenders' races based on data from hate crimes recorded by the FBI Crime Data Explorer from 2010 to 2019. To achieve this, we explored a range of machine learning models, including Random Forest, Naive-Bayes, Boosting, and Logistic Regression. We also created an HTML report that documented our thought processes, offering explanations for exploratory data analysis (EDA), data preprocessing, and model testing and evaluation.

Upon analyzing our results, a noteworthy pattern emerged: our Random Forest model exhibited exceptional accuracy when classifying White offenders but significantly higher errors when dealing with minority groups. This trend was consistent across all our models. The root cause lay in the imbalanced distribution of hate crime offender races, with over 75% being White offenders. Further investigation, including variance importance analysis, revealed that the description of the bias (the type of hate crime offense) held the most significant influence in determining a hate crime offender's race. Ultimately, our best-performing models were Random Forest and Boosting, both with an error rate of approximately 23%.

In conclusion, our project demonstrated that predicting an offender's race using various crime features is feasible. However, it may be inherently biased due to the pronounced disparity in the distribution of crimes among different offender races.

![HC_1](/assets/img/hate_crime_1.PNG)
![HC_2](/assets/img/hate_crime_2.PNG)

**Improvements:**  Considering the uneven distribution of offender races in our dataset, we would have liked to enhance our pipeline to overcome this obstacle. These improvements would encompass oversampling and data augmentation techniques, stratified data sampling methods, and the implementation of more stringent regularization measures which would all be designed for mitigating the impact of our data imbalance.

**Technical Skills:** Machine Learning, Random Forest, Naive-Bayes, Boosting, Logistic Regression

**Tools:** R, R Markdown

**Team:** Mitchell Rapaport, Ryan Stofer

[![Open Report](https://img.shields.io/badge/HTML-View_Report-green?logo=html5&logoColor=green)](https://github.com/rrstofer/rrstofer.github.io/blob/main/assets/img/hate_crime_project.html) [![Open Rmd](https://img.shields.io/badge/R-View_Report-green?logo=R&logoColor=green
)](https://raw.githubusercontent.com/rrstofer/rrstofer.github.io/main/assets/img/hate_crime_project.Rmd)
