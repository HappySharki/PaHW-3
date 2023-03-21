# Основы языка Python для аналитиков (семинары)
## Домашнее задание к уроку 3. Изменение таблиц в Pandas

Условие 1: Задача 1
Скачать данные из прошлого семинара(дома)
Считать данные с помощью pandas
Вывести на экран первые 5 строк
1.2 Создать новый признак delta_renovated, который будет содержать разницу в годах между годом реновацией дома и годом постройки дома
Если реновации дома не было, то в новом признаке поставьте 0
1.3 Создайте признаки года продажи, месяца продажи
1.4 Удалите признаки date, zipcode, lat, long

Условие 2: 2 задача
Создайте датафрейм с клиентами:
clients = pd.DataFrame({
'client_id': [1459, 4684, 3498, 3942, 4535, 2308, 2866, 2765, 1472, 4236, 2295,
939, 3840, 280, 20, 4332, 3475, 4213, 3113, 4809, 2134, 2242,
2068, 4929, 1384, 1589, 3317, 2260, 1727, 1764, 1611, 1474],
'house_id': [8965450190, 6823100225, 5104540330, 2131701075, 1522700060,
1189000207, 6821600300, 7137950720, 9510920050, 6131600255,
5428000070, 1788800910, 8100400160, 3123049142, 6306800010,
5083000375, 7920100025, 1951600150, 809001400, 339600110,
1622049154, 1099600250, 8563000110, 2768100205, 3995700435,
8861700030, 3303980210, 7731100066, 8146100580, 825069097,
3889100029, 9524100196]
})
2.1 Присоедините к таблице clients данные по домам через метод join
2.2 Присоедините к таблице clients данные по домам через метод merge
Это нужно, чтобы понимать, какие дома покупались клиентами
house_id - это индексы датафрейма с домами
Условие 3: 3 задача
Составьте несколько сводных таблиц
3.1 Найдите среднюю стоимость домов в зависимости от количества спален
Отсортируйте от меньшей стоимости к большей
3.2 Найдите минимальную, среднюю и максимальную стоимости домов в зависимости от состояния дома
3.3 Постройте таблицу с подсчетом количества домов в данных в зависимости от вида на набережную и оценкой вида
3.4 Каких домов в зависимости от этажности и количества спален больше?
3.5 Постройте таблицу с подсчетом медианной стоимости домов в данных в зависимости от состояния дома и оценки дома
