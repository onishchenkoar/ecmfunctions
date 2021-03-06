# willGenericEntityGridRowBeUnique

---

Эта функция используется для проверки уникальности одной или нескольких колонок в GenericEntityGrid.
Она может использоваться только в блоке `<validation>` на странице, используемой для добавления/редактирования строки GenericEntityGrid.
Функция принимает любое число имен колонок и проверяет, что в GenericEntityGrid нет ни одной строки с такими же значениями.
Функция не проверяет отсутствие дубликатов в данных таблице до добавления или удаления строк.
Предполагается, что этот критерий применяется принудительно для каждого сохранения сущности.

#### Возвращает:

`Boolean`

Указывает, будет ли добавленная строка содержать уникальный набор значений для указанны колонок после
сохранения модальных данных.

## Аргументы

|  | Имя аргумента | Описание | Тип значения |
| --- | --- | --- | --- |
| 1 | col1 | Полное имя колонки в GenericEntityGrid, в форме строки. | `String` |
| 2...n | coln | При необходимости, вы можете указатьт любое число дополнительных полных имен колонок. | `String` |

## Примеры

**Пример 1:** В этом примере демонстрируется использование блока `<finalize>` на странице добавления/редактирования GenericEntityGrid,
где эта функция используется для проверки, что все строки содержат уникальные значения для комбинации двух колонок.
```xml
<finalize>
   <validation test='not WillGenericEntityGridRowBeUnique("X_TRANSACTION.X_INSTITUTION_ID", "X_TRANSACTION.X_TRANSACTION_ID")'>
      <errmsg><message key='transaction.row.not.unique.txt'/></errmsg>
   </validation>
</finalize>
```



[На главную](./)