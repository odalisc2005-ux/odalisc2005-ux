
# Predictions of Animal outcomes inside the Austin Animal Shelter
## Purpose and Objectives of the project:

The dataset used is the Austin Animal Shelter Outcomes dataset:

The goal of this project was to use a supervised machine learning model to predict the outcome of an animal based on its features.
- animal type 
- breed
- age
- sex
- intake conditions
- outcome type (adopted, returned to owner, euthanized)

Specifically, the question that motivated this project was "can I predict if this animal will be returned to the owner, transferred to another shelter, adopted, or euthanized based on its physical characteristics?"

This is a classification problem, where the model learns patterns from the data and predicts the outcome category. It can help animal shelters better understand individual animals' outcome and improve planning for future plans within the animal shelter and could potentially estimate how long animals may stay inside the shelter. This would all help the animal shelter figure out if they have enough space to take more animals and if they need more resources to help additional animals that come into the animal shelter.

Prediction category - adoption, transfer, return to owner, & euthanasia
Input - age, breed, animal type, sex 
Output - what happens to the animal
Multi class classification - more then 2 outcomes 

The graphical diagram chosen was bar chart because the data is categorical while a histogram can represent numerical data. Specifically, the graphs results measured the accuracy changes for each parameter. This helps us see which model performs better.

We used the features animal type, breed, age, and sex because they directly affect what happens to an animal in a shelter. The type of animal helps us determine if dogs, cats, and other animals have different outcome patterns. Breed helps us decide if some breeds are adopted faster than others. Age tells us what age range of animals is more likely to get adopted. The animal's sex type may influence their behavior and help boost their likelihood of being adopted. The features that we removed in the “process and analyze” portion of the project were datetime, date_of_birth, monthyear, and name to get rid of any irrelevant noise and expensive information that didn't help us make predictions in the long run. 

The algorithms used were Decision trees and Random forest. For decision trees we realized that we could implement this simple baseline model to show us how the singular model performs. Random Forest on the other hand is more advanced in that it combines multiple decision trees to get better accuracy and reduces overfitting. For the “experimentation” portion of the project, we tested different values for the number of trees sent in as estimators. Specifically, we used the values 10, 50, 100, and 200 because this variation lets us see how the model performance changes over time. This showed us that the more trees sent in, the better the model performed. However, after a certain point we can see that the improvement slows down. Additionally, we used “class_weight = ‘balanced’” because this allows the model to treat all classes more fairly and prevents it from ignoring rare outcomes. 5 fold cross validation was also used to train/test split the data and test the model multiple times. Finally, we used a weighted score and not accuracy because the weighted score evaluates both precision and recall which expresses the real performance of the model.

Conclusion of the project:

The goal of this project was to predict the outcome of an animal in a shelter based on the datasets attributes. Specifically, we wanted to determine if attributes such as animal type, breed, age, and sex could help predict outcomes like adoption, transfer, or return to owner. This problem was approached as a multiclass classification task, where each animal is assigned to one of several possible outcome categories.
 
To accomplish this, we cleaned and processed the dataset, handled missing values, and encoded categorical variables so they could be used in machine learning models.Two algorithms were tested: Decision Trees and Random Forest. We chose these because Decision Trees are simple in providing clear information to complex data, while Random Forest improves performance providing high accuracy and handling highly dimensional data. Next, we experimented by changing the number of trees sent in through random forest. At last we implemented class weights to handle any imbalanced data, k fold cross validation to split the dataset, and f1-score to offer us a better metric that combines recall and precision.
 
Ultimately, what worked best for us was Random forest because it performed better than Decision tree. This indicates that adding more trees helped improve the performance of the model to an extent. We also know that the implementation of cross validation showed us results that remained consistent through the experiment of how many trees were being modeled for random forest.


One limitation of the project is that the decision tree had a lower performance than Random Forest, likely due to overfitting. Along the way we had also experimented with using accuracy scores which did not work out for us after all because the classes were imbalanced, which can make prediction more difficult. Additionally, some features like breed and age may need further processing to improve results. 


### Installation Instructions: 

1. Go to the official Python website and click Download Python for your operating system. 
2.Open the downloaded installer, check Add Python to PATH, and follow the prompts to complete installation. 
3. Open Command Prompt (Windows) or Terminal (macOS/Linux). 
4. Type pip install notebook and press Enter to install Jupyter Notebook. 
5. In the terminal, type cd followed by the path to your desired working folder, then press Enter. 6. Start Jupyter by typing jupyter notebook and pressing Enter.
7.  Wait for your browser to open at http://localhost:8888 showing the Jupyter Notebook interface. 
8. In the interface, click New and select Python 3 to create a new notebook. 
9. To rename it, right-click Untitled.ipynb, select Rename, enter a new name ending with .ipynb, and confirm.

### Features and Technology Stack:

Language: Python
IDE: Jupyter Notebook

## By Odalis Cortes 
## Contact Methods:

Email: odalisc2005@gmail.com
LinkedIn: https://www.linkedin.com/in/odaliscorteschona/

   
