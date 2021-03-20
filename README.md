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

## Dataset

Obtained from [Coronavirus Disease 2019 (COVID-19) Clinical Data Repository](https://covidclinicaldata.org/)
Data dictionary [Coronavirus Disease 2019 (COVID-19) Clinical Data Repository](https://covidclinicaldata.org/)

## Conclusion

### book1

Symptoms which has high association with covid test result

|feature|coefficient|
|-|-|
|fever| .27|
|muscle sore| .23|
|temperature| .21|
|loss of smell| .22|
|loss of taste| .21|

### book2
Neural Network with 77% accuracy

## Recommendation & Note

Relatively `loss_of_smell,`, `loss_of_taste`, `muscle_sore`, `temperature`, `headach` have strong associaion with `covid_test_results`. Health workers can pre-screen patients by giving questionaire and they would group based on the result so that they could reduce infection on site

They can assume if a patients report below symptoms, the patient could be infected by COVID more likely

A patient
* cannot smell
* cannot taste
* has sore muscle
* has high temperature
* has headache

This newral networl model would be used to pre-screen potential patients of COVID and reduce infections on site. In terms of use in medical site, the model is expected to be able to predict at over 99% accracy so there is a lot of space to improve. One way is get more data of `positive`, and `XGBoost` is especially high bias so I would get better result by reducing columns.
