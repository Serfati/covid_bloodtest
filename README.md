<img src="https://in.bgu.ac.il/marketing/graphics/BGU.sig3-he-en-white.png" height="48px" align="right" /> 
<img src="https://static.timesofisrael.com/www/uploads/2020/07/iStock-1214535321.jpg" height="200px"/> 

  
  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Serfati/twitter_nlp) ![](https://img.shields.io/apm/l/atomic-design-ui.svg?)
# Description  

The World Health Organization (WHO) characterized the COVID-19, caused by the SARS-CoV-2, as a pandemic on March 11, while the exponential increase in the number of cases was risking to overwhelm health systems around the world with a demand for ICU beds far above the existing capacity, with regions of Italy being prominent examples.

Brazil recorded the first case of SARS-CoV-2 on February 26, and the virus transmission evolved from imported cases only, to local and finally community transmission very rapidly, with the federal government declaring nationwide community transmission on March 20.

Until March 27, the state of São Paulo had recorded 1,223 confirmed cases of COVID-19, with 68 related deaths, while the county of São Paulo, with a population of approximately 12 million people and where Hospital Israelita Albert Einstein is located, had 477 confirmed cases and 30 associated death, as of March 23. Both the state and the county of São Paulo decided to establish quarantine and social distancing measures, that will be enforced at least until early April, in an effort to slow the virus spread.

One of the motivations for this challenge is the fact that in the context of an overwhelmed health system with the possible limitation to perform tests for the detection of SARS-CoV-2, testing every case would be impractical and tests results could be delayed even if only a target subpopulation would be tested.
## Dataset 
This dataset contains anonymized data from patients seen at the Hospital Israelita Albert Einstein, at São Paulo, Brazil, and who had samples collected to perform the SARS-CoV-2 RT-PCR and additional laboratory tests during a visit to the hospital.

All data were anonymized following the best international practices and recommendations. All clinical data were standardized to have a mean of zero and a unit standard deviation.

### Data fields
- Hematocrit,Leukocytes,Potassium etc.
- SARS-Cov-2 exam result - target; 1 for positive and 0 for negative test

### Data Augmentation
**SMOTE**

![](https://www.researchgate.net/publication/319413978/figure/fig2/AS:533727585333249@1504261980375/Data-augmentation-using-semantic-preserving-transformation-for-SBIR.png)

this technique, minority class data are synthetically over-sampled, presenting for the training subset the same proportion of instances for the positive and the
negative class.

### Training and Testing Models
Let us try the following models:

- Random Forest
- XGBoost
- Logistic Regression

Scoring function will be F1, since it is more costly to have false negatives than false positives

#### **Nested K-Fold Cross Validation**

![](https://hackingmaterials.lbl.gov/automatminer/_images/cv_nested.png)

## Model Explanation using SHAP
![](https://raw.githubusercontent.com/slundberg/shap/master/docs/artwork/shap_header.png)


## ⚠️ Prerequisites  
  
- [Python 3.6](https://www.python.org/download/releases/3.6/)  
- [Git 2.26](https://git-scm.com/downloads/)  
- [PyCharm IDEA](https://www.jetbrains.com/pycharm/) (recommend)  

## 📦 How To Install  
  
You can modify or contribute to this project by following the steps below:  
  
**1. Clone the repository**  
  
- Open terminal ( <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>T</kbd> )  
  
- [Clone](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) to a location on your machine.  
 ```bash  
 # Clone the repository 
 $> git clone https://github.com/serfati/covid_bloodtest.git  

 # Navigate to the directory 
 $> cd covid_bloodtest
  ``` 

**2. Install Dependencies**  
  
 ```bash  
 # install with pip/conda 
 $> pip install -r requirments.txt
 ```  

**3. launch of the project**  
  
 ```bash  
 # Run nootebook 
 $> jupyter notebook AML.ipynb
 ```  

- **Or open with Colab**
  
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Serfati/covid_bloodtest)

---  

> author Serfati
  
## ⚖️ License  
  
This program is free software: you can redistribute it and/or modify it under the terms of the **MIT LICENSE** as published by the Free Software Foundation.  
  
**[⬆ back to top](#description)**
