# MachineLearning-Weka

## Para creditg500.arff:

  Considerei:
  
     -> Árvores de Decisão (J48 no Weka);
     
     -> Naive Bayes;
     
  Esses algoritmos são adequados para tarefas de classificação binária.

  10-fold cross-validation results:

    Accuracy: 70.5%
    Kappa statistic: 0.2467
    Detailed Accuracy By Class:
        True Positive Rate (TP Rate) for 'good': 84.0%
        True Positive Rate (TP Rate) for 'bad': 39.0%
    Confusion Matrix:
        Correctly classified 'good' instances: 588
        Correctly classified 'bad' instances: 117
        Incorrectly classified 'good' instances as 'bad': 112
        Incorrectly classified 'bad' instances as 'good': 183

Train-Test Split results (70%-30%):

    Accuracy: 73.67%
    Kappa statistic: 0.2579
    Detailed Accuracy By Class:
        True Positive Rate (TP Rate) for 'good': 86.9%
        True Positive Rate (TP Rate) for 'bad': 36.7%
    Confusion Matrix:
        Correctly classified 'good' instances: 192
        Correctly classified 'bad' instances: 29
        Incorrectly classified 'good' instances as 'bad': 29
        Incorrectly classified 'bad' instances as 'good': 50
