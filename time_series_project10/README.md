# Проект: Прогнозирование количества заказов такси

**Описание проекта**  
Компания **«Чётенькое такси»** собрала исторические данные о заказах такси в аэропортах. Основной задачей проекта было создать модель, способную прогнозировать количество заказов такси на следующий час. Это поможет компании привлекать больше водителей в периоды пиковой нагрузки и улучшит качество обслуживания клиентов.

**Цель**: Разработать модель для предсказания количества заказов на такси на следующий час с уровнем RMSE не более 48 на тестовой выборке.

**Основные этапы проекта**:
1. Загрузка и подготовка данных, включая ресемплирование по часам и создание временных признаков.
2. Исследовательский анализ данных для выявления трендов и сезонности.
3. Обучение моделей с подбором гиперпараметров (Linear Regression, CatBoost, LightGBM, RandomForest).
4. Оценка моделей на тестовой выборке и сравнение с дамми-моделью.

**Результаты**  
Модель **CatBoost** показала наилучший результат, удовлетворяя требованиям по метрике RMSE. Добавленные временные признаки (лаговые значения и скользящее среднее) позволили значительно повысить точность прогноза. Сравнение с константной моделью подтвердило высокую предсказательную способность выбранной модели.

## Стек технологий

- **Язык программирования**: Python
- **Библиотеки**:
  - `pandas`, `numpy` 
  - `matplotlib`, `seaborn` 
  - `scikit-learn` 
  - `CatBoost`, `LightGBM`, `RandomForest`