# Ансабль моделей: Определение рыночной стоимости автомобилей

Сервис по продаже автомобилей с пробегом «Не бит, не крашен» разрабатывает приложение для привлечения новых клиентов. В нём можно быстро узнать рыночную стоимость своего автомобиля.

## Цель:

Необходимо подготовить модель машинного обучения для определения стоимости автомобилей. Значение метрики RMSE должно быть меньше 2500.

## Решение:

Были загружены и проанализированы данные. Проведена обработка данных. </br>
В Обучение моделей реализован процесс обучения ансамбля из трех моделей: решающих деревьев, LightGBM и Catboost, для задачи регрессии. Загружены и подготовлены обучающие и целевые признаки из датасета.</br>
Созданы два пайплайна: один для числовых (num_pipeline) и один для категориальных признаков (cat_pipeline).</br>
Пайплайн включают в себя стандартизацию, генерацию полиномиальных признаков, устранение мультиколлинеарности и заполнение пропущенных значений методом ближайших соседей (KNNImputer).</br>
Создан ColumnTransformer, который применяет соответствующий пайплайн к числовым и категориальным признакам.</br>
Выбраны основные модели для ансамбля: решающие деревья DecisionTreeRegressor, LGBMRegressor и CatBoostRegressor.</br>
Использован RandomizedSearchCV для подбора лучших гиперпараметров. Обучение моделей проведено с использованием кросс-валидации (cv=3) и оценки метрики RMSE. </br>
Рассчитана метрика качества RMSE для ансамбля моделей показала результат RMSE: 1511.72.

## Вывод

Рассчитана метрика качества RMSE для ансамбля моделей: DecisionTreeRegressor, LGBMRegressor и CatBoostRegressor на тестовых данных показала результат RMSE: 1511.72, что меньше требуемого значения метрики 2500 в задании.

## Стек:
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)  ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)  <img src="https://seaborn.pydata.org/_images/logo-wide-lightbg.svg"  title ="seaborn"  width="100" heitght ="50"  />  ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)   ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)   <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg"  title ="scikit-learn"  width="50" heitght ="25"  />  <img src="https://feature-engine.trainindata.com/en/latest/_images/FeatureEngine.png"  title ="feature-engine"  width="30" heitght ="25"  />, <img src="https://lightgbm.readthedocs.io/en/stable/_images/LightGBM_logo_black_text.svg"  title ="LightGBM"  width="90" heitght ="45"  />  <img src="https://upload.wikimedia.org/wikipedia/commons/c/cc/CatBoostLogo.png"  title ="CatBoost"  width="30" heitght ="30"  />
