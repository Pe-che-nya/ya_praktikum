__Предсказание рыночной стоимости б\у автомобиля.__

Описание:

Сервису по продаже автомобиля необходимо предоставить модель для определения стоимости автомобиля. Метрикой качества выбрать RMSE. Заказчику важны качество предсказания, скорость предсказания и время обучения.

На этапе предобработка, данные очищены от незначащих признаков. Проанализированы технические характеристики автомобилей и на основе их закономерностей очищены пропуски. Выбросы обработаны с помощью диаграммы размаха. Категориальные данные для моделей случайный лес и линейная регрессия обработаны техникой порядкового кодирования OrdinalEncoder. Обучение проводилось на линейной регрессии, случайном лесе и на градиентном спуске, реализованном в двух библиотеках lightgbm и catboost. Подбор гипперпараметров производился с помощью поиска по сетке GridSearch. В результате выявлено три модели с соответствующей метрикой качества: случайный лес, lightgbm и catboost. Однако, так как время предсказания является важным параметром для заказчика, то лучшей выбрана модель обученная на градиентном спуске, реализованном в библиотеке lightgbm

Используемые библиотеки:

pandas, copy, matplotlib, numpy, sklearn, catboost,array,lightgbm,timeit