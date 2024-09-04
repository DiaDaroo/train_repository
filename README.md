### [Персонализация предложений постоянным клиентам](https://github.com/DiaDaroo/data_science_projects/blob/main/Обработка%20данных.ipynb)

**Цель:**

Руководство компании желает разработать решение, которое позволит персонализировать предложения постоянным клиентам, чтобы увеличить их покупательскую активность. 
Нужно промаркировать уровень финансовой активности постоянных покупателей. В компании принято выделять два уровня активности: «снизилась», если клиент стал покупать меньше товаров, и «прежний уровень».


**Используемые модели:**

В проекте был осуществлен перебор моделей и их гиперпараметров:

* KNeighborsClassifier ('models__n_neighbors': range(1, 20), 'preprocessor__num': [StandardScaler(), MinMaxScaler(), 'passthrough'])  
* DecisionTreeClassifier ('models__max_depth': range(2, 20), 'models__max_features': range(2,5), 'preprocessor__num': [StandardScaler(), MinMaxScaler(), 'passthrough'])
* SVC ('models__kernel': ['linear', 'rbf', 'poly'], 'preprocessor__num': [StandardScaler(), MinMaxScaler(), 'passthrough'])
* LogisticRegression, ('models__C': range(1,5), 'preprocessor__num': [StandardScaler(), MinMaxScaler(), 'passthrough'])


