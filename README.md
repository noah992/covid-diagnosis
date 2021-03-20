# covid-diagnosis

* [code](https://github.com/noah992/covid-diagnosis/tree/main/code)
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
