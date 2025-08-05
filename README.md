# Cancer-de-mama

Este projeto comparou diversos modelos de machine learning para prever quais tumores de uma base de dados eram malignos.
Os modelos colocados a prova foram: RandomForest (com e sem balanceamento via SMOTE e balanceamento de hiperparâmetros), GradientBoosting, SVM e VotingClassifier.

Os melhores resultados se deram com o RandomForest balanceado mas os ajustes no hiperparâmetro se mostraram obsoletos.
As métricas do melhor modelo:
Matriz de Confusão com SMOTE:
 [[69  2]
 [ 2 41]]

Relatório de Classificação com SMOTE:
               precision    recall  f1-score   support

           0       0.97      0.97      0.97        71
           1       0.95      0.95      0.95        43

    accuracy                           0.96       114
   macro avg       0.96      0.96      0.96       114
weighted avg       0.96      0.96      0.96       114

Nesse exemplo (detecção de doença severa) o Recall é a métrica mais importante. Abordagens futuras serão aplicadas para melhoria desse prompt.
