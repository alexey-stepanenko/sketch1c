# Идея

Только **поведение**! 

Прототип должен быть свободен от объектов метаданных (справочник или регистр сведений, дерево значений или динамический список с группировками - решает разработчик). В то же время ожидаю, что ограничение в элементах управления (только элементы управления 1С) даст экономию времени как на само прототипирование так и на разработку, а так же снизит нагрузку на систему.

# Заметки

## Свойства форм и элементов управления

* Свойства должны быть уникальными, а вот данные выбора может быть много, т.е. сколько нужно для разных типов. Пример: свойство **Группировка** есть и у группу и у группы колонок но данные выбора у них разные, поэтому ДанныеВыбора оставил как есть но добавил ДанныеВыбора_ГруппаКолонок специально для группы колонок.
* Для свойств, которые нужно выбирать из выпадающего списка (Булево в том числе), нажно заполнять данные выбора и для новых элементов управления (только что добавленных) из этих данных выбора брать первый элемент в списке как значение по умолчанию.

# Поддерживаемые типы реквизитов формы

* Число
* Строка
* Дата
* Булево
* ТаблицаЗначений
* ДеревоЗначений
* ТабличныйДокумент
* ТекстовыйДокумент
* ФорматированнаяСтрока
* ФорматированныйДокумент
* Картинка
* СтандартныйПериод