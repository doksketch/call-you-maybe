# Uplift - моделирование
Отранжировать клиентов в порядке эффективности коммуникации. Провести A/B тестирование и реализовать Rest-Api сервис.

### Целевая метрика ###
 - uplift_at_@30

### Дополнительная метрика ###
  - ROC-AUC

### Структура проекта ###
  - корень проекта - Теоретическая часть об uplift моделировании и XGBoost
  - AB modelling - моделирование определения статистически значимой разницы между влияниями на бизнес-показатели двух версий модели
  - app - Rest-Api сервис c запуском локального сервера и примером запроса
  - sandbox - прототипирование с небольшим eda, пайплайнами feature engineering и feature selection
  - models - финальные модели для Rest-Api

### Используемые статистические тесты и техники ###
  - тест Колмогорова-Смирнова
  - тест Манна-Уитни
  - множественное сравнение с поправкой Холма-Бонферонни

### Используемые алгоритмы и модели ###
  - XGBoost
  - Solo модель
  - Сlass Transformation
  - Two Models

### Best score ###
  - Two Models uplift_at_@30 = 0.079
  - ROC AUC = 0.689

### Запуск на локальной машине ###

 - ```git clone https://github.com/doksketch/call-you-maybe.git```
 - ```python -m pip install requirements.txt```
 - скачать и распаковать [архив с данными](https://drive.google.com/file/d/1kUwVfjlptJLHx37cRUSQwpZsYXMgkHA7/view?usp=sharing)
 - выбрать нужный блокнот

Данные взяты из хакатона X5Retailhero

