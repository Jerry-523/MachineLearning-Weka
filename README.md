# MachineLearning-Weka

## Para creditg500.arff:

  Considerei:
  
     -> Árvores de Decisão (J48 no Weka);
     
     -> Naive Bayes;
     
  Esses algoritmos são adequados para tarefas de classificação binária.

 ### Results from 10-fold Cross-Validation:
Naive Bayes:

    Overall Accuracy: 75.4%
    Kappa Statistic: 0.3813
    Mean Absolute Error: 0.2936

J48 (C4.5 Decision Tree):

    Overall Accuracy: 70.2%
    Kappa Statistic: Not provided
    Mean Absolute Error: Not provided

 ### Results from 70%-30% Train-Test Split:
Naive Bayes:

    Accuracy on Test Data: 75.33%
    Kappa Statistic: 0.3537
    Mean Absolute Error: 0.2851

J48 (C4.5 Decision Tree):

    Accuracy on Test Data: 75.33%
    Kappa Statistic: 0.3537
    Mean Absolute Error: 0.2851

Comparison:

    Naive Bayes performed similarly in both evaluation methods, achieving an accuracy around 75% and showing consistent results in cross-validation and the train-test split.

    J48 does not provide specific metrics for cross-validation but achieves the same accuracy (75.33%) as Naive Bayes in the train-test split.

Selection:

Considering the available information, Naive Bayes seems to have shown more consistency in performance between cross-validation and the 70%-30% train-test split. As both Naive Bayes and J48 yielded similar accuracy in the train-test split and Naive Bayes also showed good performance in cross-validation, Naive Bayes appears to be the slightly better-performing model due to its consistency in both evaluation methods.

However, if you prioritize interpretability, J48 might be a better choice due to its tree-like structure, which is more interpretable than Naive Bayes' probability-based decision-making.
