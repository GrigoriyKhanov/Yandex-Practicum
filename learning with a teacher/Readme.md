# Обучение с учителем

Прогноз оттока клиентов из банка. Построение модели с предельно большим значением F1-меры.
Из «Бета-Банка» стали уходить клиенты. Каждый месяц. Немного, но заметно. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.

## Цель:

Нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет. Используя предоставленые исторические данные о поведении клиентов и расторжении договоров с банком.
Постройть модель с значением F1-меры не менее 0.59.

## Решение:
Были загружены и проанализированы данные. Проведена обработка данных. 
Выполнено кодирование и масштабирования признаков, борьба с дисбалансом. 
Подбор параметров моделей выполнен с использованием GridSearch и RandomizedSearch

## Вывод
Выбрав лучшую модель "Случайного леса" и проведя финальное тестирование, получили значение F1 меры 0.613, что превышает требования по запрошенной метрике F1 меры 0.59.

## Стек:
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)  <img src="https://seaborn.pydata.org/_images/logo-wide-lightbg.svg"  title ="seaborn"  width="100" heitght ="50"  /> ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)  ![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=%white) 
<img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg"  title ="scikit-learn"  width="50" heitght ="25"  />

