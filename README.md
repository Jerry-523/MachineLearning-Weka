# MachineLearning-Weka

## For creditg500.arff:

###  I choose these algorithms:
  
     -> Decision Tree (J48 no Weka);
     
     -> Naive Bayes;
     
  These algorithms are suitable for binary classification tasks.
  ### Validation
![validation](https://github.com/Jerry-523/MachineLearning-Weka/assets/92488227/944b0f91-9495-45f1-a294-e3f048ee2c2f)

  

 ### Results from 10-fold Cross-Validation:
#### Naive Bayes:

    Overall Accuracy: 75.4%
    Kappa Statistic: 0.3813
    Mean Absolute Error: 0.2936

#### J48 (C4.5 Decision Tree):

    Overall Accuracy: 70.2%
    Kappa Statistic: Not provided
    Mean Absolute Error: Not provided

   ### Results from 70%-30% Train-Test Split:
#### Naive Bayes:

    Accuracy on Test Data: 75.33%
    Kappa Statistic: 0.3537
    Mean Absolute Error: 0.2851

#### J48 (C4.5 Decision Tree):

    Accuracy on Test Data: 75.33%
    Kappa Statistic: 0.3537
    Mean Absolute Error: 0.2851

### Comparison:

  Naive Bayes performed similarly in both evaluation methods, achieving an accuracy around 75% and showing consistent results in cross-validation and the train-test split.
  J48 does not provide specific metrics for cross-validation but achieves the same accuracy (75.33%) as Naive Bayes in the train-test split.

### Selection:

Considering the available information, Naive Bayes seems to have shown more consistency in performance between cross-validation and the 70%-30% train-test split. As both Naive Bayes and J48 yielded similar accuracy in the train-test split and Naive Bayes also showed good performance in cross-validation, Naive Bayes appears to be the slightly better-performing model due to its consistency in both evaluation methods.

### Prediction
#### Confusion matrices

The confusion matrices provide a detailed insight into the model's classifications, allowing us to identify correct and incorrect classifications for each class. Let's analyze the confusion matrices provided for NaiveBayes in both evaluations (Cross-Validation and 70% train - 30% test):

#### NaiveBayes - Cross-Validation:

    Correctly classified as 'good': 605
    Correctly classified as 'bad': 149
    Incorrectly classified as 'bad' when they are 'good': 95
    Incorrectly classified as 'good' when they are 'bad': 151

#### NaiveBayes - 70% train - 30% test:

    Correctly classified as 'good': 186
    Correctly classified as 'bad': 40
    Incorrectly classified as 'bad' when they are 'good': 35
    Incorrectly classified as 'good' when they are 'bad': 39

Analyzing both confusion matrices, it's evident that the performance of the NaiveBayes model is better in the Cross-Validation evaluation, where there is a higher number of correct classifications for both the 'good' and 'bad' classes compared to the performance in the 70% train and 30% test set. It's important to note that the model seems to struggle more in correctly classifying the 'bad' class, as the number of correct classifications is lower in both evaluations.

## For Mnist Net
### NaivesBayes
Time taken to build model: 7.9 seconds

=== Stratified cross-validation ===
=== Summary ===

Correctly Classified Instances       41547               69.245  %
Incorrectly Classified Instances     18453               30.755  %
Kappa statistic                          0.658 
Mean absolute error                      0.0615
Root mean squared error                  0.2472
Relative absolute error                 34.1832 %
Root relative squared error             82.4083 %
Total Number of Instances            60000     

=== Detailed Accuracy By Class ===

                 TP Rate  FP Rate  Precision  Recall   F-Measure  MCC      ROC Area  PRC Area  Class
                 0.874    0.015    0.861      0.874    0.867      0.853    0.975     0.852     0
                 0.939    0.021    0.851      0.939    0.893      0.880    0.968     0.827     1
                 0.581    0.014    0.817      0.581    0.679      0.661    0.934     0.727     2
                 0.641    0.019    0.791      0.641    0.708      0.683    0.927     0.706     3
                 0.427    0.010    0.827      0.427    0.563      0.566    0.932     0.676     4
                 0.282    0.013    0.682      0.282    0.399      0.406    0.903     0.594     5
                 0.930    0.044    0.700      0.930    0.799      0.783    0.959     0.707     6
                 0.640    0.011    0.867      0.640    0.737      0.721    0.963     0.810     7
                 0.649    0.094    0.427      0.649    0.515      0.463    0.871     0.431     8
                 0.894    0.100    0.496      0.894    0.638      0.619    0.928     0.535     9
    Weight Avg.  0.692    0.034    0.735      0.692    0.686      0.670    0.937     0.690     

=== Confusion Matrix ===

       a    b    c    d    e    f    g    h    i    j   <-- classified as
    5174    8   81   14   25   36  284    8  221   72 |    a = 0
       0 6329   28   39    4   40   79    3  159   61 |    b = 1
     131   85 3460  313   61   63  888   23  880   54 |    c = 2
     112  179  260 3932   34   65  222  134  741  452 |    d = 3
      50   32  120   40 2494  171  422  122  584 1807 |    e = 4
     373   81   79  390   87 1527  305   41 2174  364 |    f = 5
      52   62  105    2    6   72 5504    2  105    8 |    g = 6
      33   50   22  100  109   19    8 4011  107 1806 |    h = 7
      57  566   74  120   64  216  139   36 3796  783 |    i = 8
      27   41    8   21  133   29    8  245  117 5320 |    j = 9

