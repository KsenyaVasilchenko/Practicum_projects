# Анализ рынка недвижимости Санкт-Петербурга

![Санкт-Петербург](https://github.com/KsenyaVasilchenko/Practicum_projects/blob/main/EDA_project2/images_project2/october03.jpg)

## Описание проекта

<div style="background-color: #f9f9f9; padding: 15px; border-radius: 8px;">
Данный проект посвящен анализу факторов, влияющих на стоимость недвижимости в Санкт-Петербурге и прилегающих районах. Были изучены основные параметры, оказывающие влияние на цену квартир, такие как площадь, количество комнат, тип этажа и расстояние до центра города. Проект позволяет лучше понять динамику рынка недвижимости, выявить ключевые закономерности и аномалии, а также принять обоснованные решения в сфере покупки или продажи недвижимости.
</div>

## Основные результаты анализа

### 1. Зависимость цены от параметров квартиры
Эти параметры могут быть важными факторами при определении рыночной стоимости квартиры, и их следует учитывать при анализе и принятии решений о покупке или продаже недвижимости
- Площадь квартиры — главный фактор, напрямую влияющий на цену.
- Количество комнат и тип этажа оказывают дополнительное влияние, но менее значительное.
- Удалённость от центра снижает стоимость, за исключением элитных пригородных зон.

<div style="display: flex; justify-content: space-between; gap: 10px;">
  <img src="https://github.com/KsenyaVasilchenko/Practicum_projects/blob/main/EDA_project2/images_project2/depend_price_area.png" alt="График зависимости цены от общей площади" width="45%">
  <img src="https://github.com/KsenyaVasilchenko/Practicum_projects/blob/main/EDA_project2/images_project2/depend_price_rooms.png" alt="График зависимости цены от количества комнат" width="45%">
</div>

### 2. Анализ средней цены по годам
Анализ средней цены показал:
- Самая высокая средняя цена была зафиксирована в 2014 году, но количество объявлений в этом году было минимальным.
- В 2017 году наблюдалось наибольшее количество объявлений о продаже недвижимости.

### 3. Стоимость недвижимости в зависимости от расстояния до центра Санкт-Петербурга
Проанализирована зависимость средней стоимости квартир от удалённости от центра Санкт-Петербурга:
- С увеличением расстояния от центра города, цена за квадратный метр снижается.
- На расстоянии от 25 до 30 км от центра наблюдается неожиданный рост стоимости, что может быть связано с наличием эксклюзивных объектов недвижимости в маленьких населенных пунктах.


<div style="display: flex; justify-content: space-between; gap: 10px;">
  <img src="https://github.com/KsenyaVasilchenko/Practicum_projects/blob/main/EDA_project2/images_project2/price_distance.png" alt="Анализ стоимости по расстоянию" width="45%">
  <img src="https://github.com/KsenyaVasilchenko/Practicum_projects/blob/main/EDA_project2/images_project2/price_locality.png" alt="Анализ стоимости по локации" width="45%">
</div>

<div style="display: flex; justify-content: center; margin-top: 10px;">
  <img src="https://github.com/KsenyaVasilchenko/Practicum_projects/blob/main/EDA_project2/images_project2/price_citycenters.png" alt="Анализ стоимости по локации до центра" width="50%">
</div>

Анализ помог определить ключевые факторы ценообразования и выявить аномалии, что делает его полезным для оценки рыночной стоимости и принятия решений в сфере недвижимости.


## Стек
- Python для анализа данных
- Pandas и NumPy для обработки данных
- Matplotlib и Seaborn для визуализации результатов