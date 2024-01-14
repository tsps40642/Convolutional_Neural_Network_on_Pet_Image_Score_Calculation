# Convolutional_Neural_Network_on_Pet_Image_Recognition

## Overview
PetFinder.my, a leading animal welfare platform in Malaysia that rehomes strays, empowers rescuers, and develops technology solutions for animal welfare.  

As of 2023 December, PetFinder is featuring 200k pets on their platform, and they have helped 70k pets find their new home. This project aims to develop an AI-based tool to enhance the appeal of pet photos on PetFinder’s website, which will aid in increasing the chance of adoption for stray and shelter animals.  

By analyzing raw images and metadata of dogs and cats, our solution offers a deep learning algorithm that can predict the “Pawpularity” of pet photos, aside from PetFinder, the solution would also guide worldwide shelters and rescuers to save more innocent lives. 

## Solution Overview
In our mission to develop an effective solution for enhancing the appeal of pet photos on PetFinder’s platform and increasing adoption rates, we embarked on a multi-step approach leveraging Convolutional Neural Networks (CNNs).  

Initially, our attempt to construct a custom CNN yielded suboptimal results. Recognizing the power of pretrained models, we transitioned to utilizing Keras' pretrained models, beginning with a regression version. Interestingly, our initial intuition suggested that metadata might not contribute significantly, as it could already be encapsulated in the pretrained model. To explore alternative avenues, we also reframed the problem as a classification task, treating the 100 integers of "Pawpularity" scores as 100 categories. Our incorporation of metadata through Support Vector Regression (SVR) proved unhelpful, affirming our earlier speculation.  

After extensive experimentation, we found that employing the regression-based approach led us to the most accurate predictions for our model with the lowest Root Mean Square Error (RMSE) score. This comprehensive exploration of model architectures and data representations underscores our commitment to delivering a robust AI-based tool for PetFinder, poised to make a meaningful impact on the lives of stray and shelter animals globally.  

There are 2 solution routes and the corresponding ipynb files are listed respectively.  
1. If viewing the problem as a regression task, we use:  
   (1) Data-preprocessing_on_image_array.ipynb  
   (2) CNN_regression_on_pawpularity_score.ipynb  
2. If Viewign the problem as a classification task, we use:  
   (1) Data-preprocessing_on_image_array.ipynb  
   (2) Data-preprocessing_on_onehot_encoding_on_metadata.ipynb  
   (3) CNN_classification_on_pawpularity.ipynb    

Data source from a past Kaggle competition:   
(PetFinder.my - Pawpularity Contest) https://www.kaggle.com/competitions/petfinder-pawpularity-score/overview  

### Other elaborations on methedoogy, exploratory data analysis, code comments, model performance, and future step are all in Project_write_up_document.pdf.  

### Credit to other team members: Guoquan Lin, Otto Gaulke, Yen Chen Hsu, Joyce Wu  
