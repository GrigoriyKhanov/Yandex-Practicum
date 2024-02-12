# Финальный проект: Прогноз оттока клиентов оператор связи «ТелеДом».

Прогноз оттока клиентов оператор связи «ТелеДом». Построение модели на основании исторических данных, значение метрики качества «ROC-AUC» должно быть не менее 0,85.

## Цель:

Оператор связи «ТелеДом» хочет бороться с оттоком клиентов. Для этого его сотрудники начнут предлагать промокоды и специальные условия всем, кто планирует отказаться от услуг связи. Чтобы заранее находить таких пользователей, «ТелеДому» нужна модель, которая будет предсказывать, разорвёт ли абонент договор. Предоставлены персональные данные о некоторых клиентах, информацию об их тарифах и услугах. Необходимо обучить модель для прогноза оттока клиентов.

## Решение:
Были загружены и проанализированы данные. Созданные новые признаки. Проведена проверка признаков на Мультиколлинеарность
Используя Pipeline и RandomizedSearch было выполнено масштабирование, кодирование признаков и подбор параметров с учетом кросс-валидации, а также вычислена метрика качества roc_auc. Для лучшей модели была найдена важность признаков и построена матрица ошибок. 

## Вывод
В ходе работы над данными «ТелеДом» по прогнозу оттока клиентов была полученная модель LGBMClassifier. Метрика качества roc_auc полученной модели составляет 0.904, вероятность ошибки модели составляет не более 10%. Значение метрики качества полученной модели превосходит требования технического задания, значение метрики не менее 0.85.

## Стек:
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) <img src="https://seaborn.pydata.org/_images/logo-wide-lightbg.svg"  title ="seaborn"  width="100" heitght ="50"  /> ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)  ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)   <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg"  title ="scikit-learn"  width="50" heitght ="25"  />  <img src="https://lightgbm.readthedocs.io/en/stable/_images/LightGBM_logo_black_text.svg"  title ="LightGBM"  width="90" heitght ="45"  />
