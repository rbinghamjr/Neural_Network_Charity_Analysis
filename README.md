# Neural_Network_Charity_Analysis

## Overview

The purpose of this analysis is to use a neral network deep learning to determine loan applicants success if funded by Alphabet Soup.

## Results

### Data Preprocessing

- target variables = IS_SUCCESSFUL. This variable is used to determine whether the previous applicants were successful or not
- feature variables = APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and SPECIAL_CONSIDERATIONS
- invalid variables = EIN and NAME. These variables were removed from the data due to being used for identification and hold no value for our model

### Compiling, Training, and Evaluating the Model

- The first run of the model, there were two hidden layer used of 80 and 30 neurons using the "relu" activation type.

![image](https://user-images.githubusercontent.com/90691846/151706038-afe0e781-dd5b-4949-8c91-4c3dd6c2ec58.png)

![image](https://user-images.githubusercontent.com/90691846/151706053-45a6edcf-d076-4b10-964c-1962eba1b8f0.png)


- The first optimization attempt reviewed income amount and with the same amount of layers, neurons, and activation type.

![image](https://user-images.githubusercontent.com/90691846/151706073-4d039bf6-158d-40b6-a74e-b6132fbeabf8.png)

![image](https://user-images.githubusercontent.com/90691846/151706088-46dd1c20-792a-47bb-8c3b-caff5fd80a31.png)


- The second optimization attempt utilized three hidden layers with 80, 50, and 30 nerons.

![image](https://user-images.githubusercontent.com/90691846/151706120-6884a27b-d181-4768-bfe7-59ebc69da9de.png)

![image](https://user-images.githubusercontent.com/90691846/151706137-70ec4fc1-e369-44a6-ae4f-8fbc375092d1.png)


- The third optimization attempt utilized 2 hidden layers with 80 and 50 nerons and activiation type "tanh" was used.

![image](https://user-images.githubusercontent.com/90691846/151706181-90de3320-8b44-469f-b2f0-b7c5edba9e1e.png)

![image](https://user-images.githubusercontent.com/90691846/151706213-0b72f8c7-acf4-47c9-b27d-0a76cf980857.png)


- The first model had the highest accuracy but the target model performance of 75% was not achieved.

## Summary

Although the target was not achieved in mulitple attempts, continual fine tuning of the model should be able to achieve the expected results. Multiple attempts generated similar accuracy so another model might be beneficial to achieve the desired results. One option would be the Random Forest Classifier since it would combine multiple smaller models into a more accurate model utilizing decision trees to determine the final outcome.
