__Предсказание рыночной стоимости б\у автомобиля.__

Описание:

Сервису по продаже автомобиля необходимо предоставить модель для определения стоимости автомобиля. Метрикой качества выбрать RMSE. Заказчику важны качество предсказания, скорость предсказания и время обучения.

Очищены незначащие признаки. Проанализированы признаки и на основе их закономерностей очищены пропуски. Выбросы обработаны с помощью диаграммы размаха. Категориальные признаки для моделей случайный лес и линейная регрессия обработаны техникой порядкового кодирования OrdinalEncoder. Обучение проводилось на алгоритмах линейной регрессии, случайном лесе и на градиентном спуске, реализованном в двух библиотеках lightgbm и catboost. Подбор гипперпараметров производился поиском по сетке GridSearch. В результате выявлено три модели с соответствующей метрикой качества: случайный лес, lightgbm и catboost. Однако, так как время предсказания является важным параметром для заказчика, то выбрана модель обученная на градиентном спуске, реализованном в библиотеке lightgbm

Используемые библиотеки:

pandas, copy, matplotlib, numpy, sklearn, catboost,array,lightgbm,timeit

Статус проекта: __завершен__
