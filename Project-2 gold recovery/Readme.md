# Второй сборный проект.

Подготовка прототипа модели машинного обучения для предсказания коэффициент восстановления золота из золотосодержащей руды.

## Цель:

Необходимо подготовить прототип модели машинного обучения для компании разрабатывающей решения для эффективной работы промышленных предприятий.
Модель должна предсказать коэффициент восстановления золота из золотосодержащей руды.

## Решение:
Были загружены и проанализированы данные. Проведена обработка данных.
Входе работы была написана функций для вычисления sMAPE.
Были исключены мультиколлинеарные признаки с корреляцией более 0.9.
Используя Pipeline и RandomizedSearch было выполнено масштабирование признаков, и подбор параметров с учетом кросс-валидации, а также вычислена метрика качества sMAPE со значением 4,35 .

## Вывод

Наилучшее качество показала модель "случайного леса" с итоговым значение метрики качества SMAPE = 4.35 Проверка на адекватность показала, что качество модели случайного леса SMAPE =4.35 лучше константой модели SMAPE =5.66.
Следовательно модель случайного леса может принята в работу.

## Стек:
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)  <img src="https://seaborn.pydata.org/_images/logo-wide-lightbg.svg"  title ="seaborn"  width="100" heitght ="50"  /> ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)   ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)   <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg"  title ="scikit-learn"  width="50" heitght ="25"  />
