# Временные ряды: Прогноз заказов для компании «Чётенькое такси».

Компания «Чётенькое такси» собрала исторические данные о заказах такси в аэропортах. Чтобы привлекать больше водителей в период пиковой нагрузки, нужно спрогнозировать количество заказов такси на следующий час.

## Цель:

Необходимо подготовить модель машинного обучения для компании «Чётенькое такси», чтобы спрогнозировать количество заказов такси на следующий час. Модель должна предсказать количество заказов с значение метрики RMSE на тестовой выборке не больше 48.

## Решение:

Были загружены и проанализированы данные. Проведена обработка данных. Выполнено объединение данных с интервалом 1 час.
Подбор параметров моделей с выполнен с использованием GridSearch.

## Вывод

Была получена модель CatBoostRegressor с лучшей метрикой качества RMSE 42.26.</br>
Это говорит, что прогнозная величина, будет соответствовать действительности с точностью +/- 42 заказа.</br>
Значение метрики RMSE на тестовой выборке не превышает требуемого порога, указанного в техническом задании 48.

## Стек:
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)  <img src="https://seaborn.pydata.org/_images/logo-wide-lightbg.svg"  title ="seaborn"  width="100" heitght ="50"  /> ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)   ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)   <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg"  title ="scikit-learn"  width="50" heitght ="25"  />  <img src="https://lightgbm.readthedocs.io/en/stable/_images/LightGBM_logo_black_text.svg"  title ="LightGBM"  width="90" heitght ="45"  />   <img src="https://upload.wikimedia.org/wikipedia/commons/c/cc/CatBoostLogo.png"  title ="CatBoost"  width="30" heitght ="30"  />
