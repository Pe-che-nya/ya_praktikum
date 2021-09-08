__Определение возраста покупателей.__

Описание:

Крупному сетевому супермаркету необходимо автоматизировать процесс рекомендаций товаров для конкретной возрастной группы, а также контроль возраста при продаже алкоголя. Предполагается, что для этого будет проводиться автоматическая фотофиксация, а за  обработку фотографии будет отвечать модель, обученная нейросетью.

Необходимо разработать модель для определения возраста покупателя. В качестве метрики использовать MAE. Итоговое значение не должно превышать 8. 

Для обучения выбрана модель с архитектурой ResNet50.  Проанализированы изображения для обучения по возрастам. По диаграмме распределения возрастов выявлено, что существует недостаток изображений людей в возрасте больше 75. Проанализировав данные, а так же исходную задачу, выявлено, что недостаток в данных не повлияет на решение задачи. 

В результате обучения выбрана модель архитектурой ResNet50 c 1 нейроном в выходном слое с функцией активации ReLu. Алгоритм обучения применялся Adam. Количество эпох для обучения 10. В качестве итоговой метрики выбрана MAE с результатом 6,163

Используемые библиотеки:

Pandas, tensorflow, keras, matplotlib, seaborn

Статус проекта: __завершен__