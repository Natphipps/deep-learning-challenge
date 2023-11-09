# deep-learning-challenge
module 21 challenge

# Overview

Alphabet Soup is a charity organization that gives funding to select applicants to support their organization. The purpose of this assignment was to practice machine learning techniques and create a binary classifier that will help Alphabel Soup select applicants who have the highest chance of success if given funding. The Alphabet Soup business team provided a CSV file with over 34,000 organizations that have received funding in the past. The CSV contains information about each organization:

- EIN and NAME—Identification columns
  
- APPLICATION_TYPE—Alphabet Soup application type
  
- AFFILIATION—Affiliated sector of industry
  
- CLASSIFICATION—Government organization classification
  
- USE_CASE—Use case for funding
  
- ORGANIZATION—Organization type
  
- STATUS—Active status
  
- INCOME_AMT—Income classification
  
- SPECIAL_CONSIDERATIONS—Special considerations for application
  
- ASK_AMT—Funding amount requested
  
- IS_SUCCESSFUL—Was the money used effectively

# Results

- Data Preprocessing

   - What Variable(s) are the target(s) for your model?

       The target variable was the metadata from the column IS_SUCCESSFUL, this variable was chosen because it represents whether or not the organization's endeavours were sucessful after given funding from Alphabet Soup.
   
       ![image](https://github.com/Natphipps/deep-learning-challenge/assets/130694752/07c7937e-cf67-49ea-bce5-2eb4af0f402d)

  - What variable(s) are the features for your model?

      The original CSV had a total of 12 variables, however 2 of these variables were removed after considering them to not be beneficial to the analysis. The total number of features used were 9 since IS_SUCCESSFUL was used as a target variable.

  - What variable(s) should be removed from the input data because they are neither targets nor features?

      I removed the EIN, and NAME columns from my analysis. I did not believe that either variable had relevent information that would impact the analysis.
    
     ![image](https://github.com/Natphipps/deep-learning-challenge/assets/130694752/244a5bdc-f9fa-410a-8763-2aff8a2dac32)


- Compiling, Training, and Evaluating the Model

  - How many neurons, layers, and activation functions did you select for your neural network model, and why?

    I selected two hidden layers with 8 and 5 neurons. After trying multiple iterations of neurons it seemed that the accuracy of my model did not change significantly after trying these tests. For my optimized model I even got rid of a layer entirely and still got         similar results.

    ![image](https://github.com/Natphipps/deep-learning-challenge/assets/130694752/9b4058b1-9358-4592-bd19-0c8af8a88897)

  - Were you able to achieve the target model performance?

    I was unable to acheive the target model's performance. My accuracy did not increase more than 72%, even after making numerous changes and testing my model multiple times.

  - What steps did you take in your attempts to increase model performance?

    I tried increasing and decreasing bin values, adding more neurons, and dropping a layer. The one step I took that seemed to have the biggest impact was changing the number of features I was using in my model. I tried dropping more columns which put me at a lower        accuracy, I then tried adding more columns by only dropping the EIN variable. However, google colab kept running out of RAM and I was unable to complete the test. I believe if I was able to complete the test, I would've been able to to acheive the 75% performance.

# Summary

To conclude my analysis, I was only able to achieve a 72% accuracy for my deep learning model even after multiple tests. Unfortunately, due to running out of RAM while using google colab I could not successfully finish my optimization attempts. If I was able to finish my attempt I believe that I would have been able to acheive an accuracy of 75% or higher with continued testing. Overall, I think this was a good learning experience as these problems can occur when dealing with analytics and sometimes you have to try other solutions to get the desired outcome. I think it would be beneficial to try using another binary classification model to see if the preferred accuracy could have been acheived. For instance, support vector machine takes in a simple algorithm which generates significant accuracy and also uses less computational power, which was the problem I ran into while trying to complete my own analysis. If I tried to pursue more testing, I would like to try using SVM to see if it could solve the issues I was running into. 
    

