# DLS_ML

##Задание:

Смоделировать отток клиентов телеком компании. Эта задача очень важна на практике и алгоритмы для ее решения используются в реальных телеком компаниях, ведь если мы знаем, что клиент собирается уйти от нас, то мы попытаться удержать его, предложив какие-то бонусы.

* Произвести первичное исследование данных, обнаружить и заполнить пропуски
* Произвести анализ данных:
  1. Для численных призанков построить гистограмму или boxplot. Для категориальных посчитать количество каждого значения для каждого признака.
  2. Посмотреть на распределение целевой переменной и определить, являются ли классы несбалансированными.
* Построить линейные модели на основе данных:
  1. Обработать данные для того, чтобы к ним можно было применить LogisticRegression. Т.е. отнормировать числовые признаки, закодировать категориальные с помощью one-hot-encoding'а.
  2. С помощью кроссвалидации или разделения на train/valid выборку протестироить разные значения гиперпараметра C и выберать лучший по метрике ROC-AUC.
     - При разделении на train/valid, то использовать LogisticRegressionCV.
     - При использовании кроссвалидации использовать Pipeline и GridSearchCV.
* Воспользоваться градиентным бустингом для построения моделей (использовать catboost):
  1. Разделить выборку на train/valid. Протестировать catboost cо стандартными параметрами.
  2. Протестировать разные занчения параметров количества деревьев и learning_rate'а, выбрать лучшую по метрике ROC-AUC комбинацию.
