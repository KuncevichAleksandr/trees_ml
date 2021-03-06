
## Использование
1. Клонируйте этот репозиторий на свой компьютер.
2. Скачайте [Forest Cover Type](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset) датасет, сохраните csv локально (по умолчанию путь *data/heart.csv* от корня репозитоория).
3. Убедитесь, что Python 3.9 и Poetry установлены на вашем компьютере.
4. Установите зависимости проекта (выполните эту и следующие команды в терминале из корня клонированного репозитория):
```sh
poetry install
```
5. Запустите обучение с настройками по умолчанию:
```sh
poetry run train
```
Можно настроить дополнительные параметры (например, гиперпараметры) в интерфейсе командной строки. Чтобы получить их полный список, воспользуйтесь справкой:
```sh
poetry run train --help
```
6. Запустите пользовательский интерфейс MLflow, чтобы просмотреть информацию о проведенных экспериментах:
```sh
poetry run mlflow ui
```

## Три разных набора гиперпараметров 
![](https://github.com/KuncevichAleksandr/trees_ml/blob/main/three_hyperparameters.png)

## Лучшие параметры для GradientBoostingClassifier, найденные с помощью GridSearchCV
![](https://github.com/KuncevichAleksandr/trees_ml/blob/main/gbc_best_params.png)

## Две модели. 1. GradientBoostingClassifier. 2.RandomForestClassifier
![](https://github.com/KuncevichAleksandr/trees_ml/blob/main/two_model.png)