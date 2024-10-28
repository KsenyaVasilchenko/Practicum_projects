# Проект: Прогнозирование уровня удовлетворённости сотрудников и вероятности увольнения

![Распределение уровня удовлетворенности работой для уволенных и оставшихся сотрудников](https://github.com/KsenyaVasilchenko/Practicum_projects/blob/main/precast_project_2_p7/images_7/employee_1.png)

В рамках данного проекта были построены модели машинного обучения для прогнозирования уровня удовлетворённости сотрудников и вероятности их увольнения из компании "Работа с Заботой". Модели продемонстрировали хорошие результаты на тестовой выборке, что указывает на их эффективность в управлении персоналом.

## Цель проекта

Цель проекта — разработка системы, которая поможет предсказывать уровень удовлетворенности сотрудников и вероятность их увольнения, что позволит компании оптимизировать управление персоналом и повысить удовлетворенность работников.

## Задачи проекта

1. Первичная обработка и исследовательский анализ данных:
   - Проведен анализ данных о 1000 сотрудниках, включая их уровень удовлетворенности (в шкале от 1 до 10) и причины увольнения.
   - Выявлено, что средний уровень удовлетворенности сотрудников составляет 6.5, при этом 30% сотрудников указали на высокую рабочую нагрузку как причину своей неудовлетворенности.

   ![Анализ уровня удовлетворённости сотрудника работой в компании, целевой признак](https://github.com/KsenyaVasilchenko/Practicum_projects/blob/main/precast_project_2_p7/images_7/employee_2.png)

2. Подготовка данных для моделирования:
   - Изменены названия столбцов для удобства работы, удалены 50 дублирующих записей и произведена очистка данных.

3. Обучение моделей:
   - Задача регрессии:
     - Для прогнозирования уровня удовлетворённости была обучена модель DecisionTreeRegressor с гиперпараметрами:
       - max_depth=10
       - min_samples_leaf=10
       - min_samples_split=5
     - Метрика SMAPE показала 14.8%, что говорит о хорошем качестве предсказаний.
     
   - Задача классификации:
     - Для прогнозирования вероятности увольнения была обучена модель DecisionTreeClassifier с параметрами:
       - max_depth=6
       - max_features=6
       - random_state=42
     - Метрика ROC-AUC на тренировочной выборке составила 0.92, что указывает на высокую способность модели различать классы. Модель была протестирована на тестовой выборке, и были получены предсказания с точностью 90%.

4. Анализ важности признаков:
   - Выявлены ключевые признаки, оказывающие наибольшее влияние на уровень удовлетворенности и вероятность увольнения. К ним относятся:
     - Рабочая нагрузка
     - Оценка от руководства
     - Время на отдых

5. Выводы и рекомендации:
   - Подготовлены рекомендации по улучшению уровня удовлетворенности сотрудников:
     - Оптимизация процессов управления для равномерного распределения нагрузки.
     - Регулярные обзоры работы сотрудников и обратная связь от руководства для повышения мотивации.

## Основные результаты

1. Влияние рабочей нагрузки:
   - Рабочая загруженность оказывает значительное влияние на уровень удовлетворенности. Рекомендуется пересмотреть распределение задач среди сотрудников.

2. Корреляция с оценкой руководства:
   - Высокая корреляция (0.78) между уровнями удовлетворенности сотрудников и оценками, полученными от руководства. Регулярная обратная связь может способствовать улучшению мотивации.

3. Текучесть кадров в отделе технологий:
   - Отдел технологий имеет наивысшую долю уволившихся сотрудников (40%). Рекомендуется уделить внимание поддержке и управлению этим отделом, а также провести опросы для выявления причин увольнения.

## Заключение

Результаты проекта показывают, что примененные модели машинного обучения могут эффективно прогнозировать уровень удовлетворённости сотрудников и вероятность их увольнения. Это позволяет компании "Работа с Заботой" принимать обоснованные управленческие решения, что способствует повышению вовлеченности и удержания сотрудников.

## Стек технологий

- Язык программирования: Python
- Библиотеки:
  - `pandas`
  - `numpy`
  - `seaborn`,`matplotlib` 
  - `scikit-learn`
  - `shap`