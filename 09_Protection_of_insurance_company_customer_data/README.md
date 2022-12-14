# Защита данных клиентов страховой компании
## Описание проекта
Задача: Разработать такой метод преобразования данных, чтобы по ним было сложно восстановить персональную информацию.

## Цель проекта
- Защитить данные, чтобы при преобразовании качество моделей машинного обучения не ухудшилось.

## Ход выполнения проекта
Для анализа данных и построения модели предоставлен датасет, содержащий информацию о клиентах страховой компании. Датасет состоит из 5 столбцов с данными и 5000 строк. 
Пропуски в данных отсутствуют, подготовка данных не требуется.

**Для обучения модели выделены - **
<br>**Признаки:** пол, возраст и зарплата застрахованного, количество членов его семьи.
<br>**Целевой признак:** количество страховых выплат клиенту за последние 5 лет.

Поскольку качество модели не уменьшится при умножении признаков на квадратную обратимую матрицу, был составлен алгоритм преобразования.
<br>Для защиты данных клиентов исходный датасет был преобразован путем умножения признаков на квадратную обратимую матрицу.
<br>Далее проведены стандартные шаги по разделению датасетов на обучающие и тестовые выборкт, обучение моделей и сравнение метрик R2 для обеих.
<br>Поскольку эксперимент показал равенство метрик для обоеих моделей, следовательно качество предсказаний не изменится, а личные данные клиентов теперь более надежно защищены.

## Итоги проекта
- Найден метод защиты данных клиентов страховой компании.

В проекте использованы библиотеки:
- pandas
- sklearn
- numpy
