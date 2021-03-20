# covid-diagnosis

* [code](https://github.com/noah992/covid-diagnosis/tree/main/code)
   * book1 - interpretable model
   * book2 - predictive model
* [data](https://github.com/noah992/covid-diagnosis/tree/main/data)

## Summary

* Problem
    * Predict whether people have covid as accurately as possible - book 2
    * What symptoms/body conditions could be a sign for COVID - book 1
* Dataset - [Coronavirus Disease 2019 (COVID-19) Clinical Data Repository](https://covidclinicaldata.org/)
* EDA - Analyze association between posivity of covid test and symptoms that the patients have - book1
* Modeling - book2
    * Neural Network
    * `VotingClassifier` with `XGB`, `RandomForest`, `LogisticRegression`, `SVM`
* Conclusion
    * Below features are relatively big signs that infer you would have COVID more likely
        * Loss of smell
        * Loss of taste
        * Muscle sore
        * Body temperature
        * Heaedach
    * Neural Network with 77 % accuracy

## Problem

COVID made big impact on our world. It infects through countries rapidly and bring severe health problem all over the world.

I analyzed what kind of people should go diagnosis for covid. Idealy everyone should go but it is not very realistic and will be big loaden on hospitals so I would like to provide health workers insights that what kind of people is infected by COVID more likely so this analysis could help the health workers to pre-screen patients and would reduce infection on site.

I got dataset of COVID test results and the patients clinic information. I would like to find symptoms or clinic information which have relatively strong assciation with COVID positivity. Also I would like to create predictive model as accurately as possible.

Obtained from [Coronavirus Disease 2019 (COVID-19) Clinical Data Repository](https://covidclinicaldata.org/)

This predictive model could help both of health workers and patients that they could know if the patients are positive by answering questions so this reduce their time and loaden a lot.

## Model
Neural Network with 77% accuracy
