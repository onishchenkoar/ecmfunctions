# addMapListValue

---

Добавление нового поля для каждой Карты в списке карт (напр. добавление новой "колонки" в данных DataGrid). Эта функция используется в случаях, когда в источнике данных для DataGrid не содержит всех нужных вам колонок, но с помощью выражения CPB вы можете вычислить значения для отсутствующих колонок.

#### Возвращает:

`List<Map<String, Object>>`

Модифицированный список карт, передаваемый как первый аргумент.  Используется для передачи в
функцию DataStore.

## Аргументы

|  | Имя аргумента | Описание | Тип значения |
| --- | --- | --- | --- |
| 1 | listOfMaps | Список карт, например, данные для функции DataStore. | `List<Map<String, Object>>` |
| 2 | newFieldName | Имя для каждого нового поля, в форме строки. | `String` |
| 3 | expression | Выражение, которое нужно вычислить для каждой строки для получения значения для каждого нового поля. | `String` |

## Примеры

**Пример 1:** В этом примере демонстрируется использование этой функции для копирования поля 'CASE.CASE_STATUS_CD' в даннных DataGrid в новое поле с именем 'TEMP.CASE_STATUS_CD_COPY'
```xml
<datastore id="TEMP.CASES_GRID.store"
           data="AddMapListValue(GetEntityListAsMapList(GetEntities('case')),
                                 'TEMP.CASE_STATUS_CD_COPY',
                                 'CASE.CASE_STATUS_CD'
                                )"
/>
```



[На главную](./)