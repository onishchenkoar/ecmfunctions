# toUpper

---

Возвращает копию строкового аргумента со всеми символами в верхнем регистре.
Если аргумент имеет значение `null`, возвращается `null`.
Если аргумент не является строкой, он преобразуется в строку и затем в верхний регистр.

#### Возвращает:

`String`

## Аргументы

|  | Имя аргумента | Описание | Тип значения |
| --- | --- | --- | --- |
| 1 | string | Преобразование строки в верхний регистр | any |

## Примеры

**Пример 1:** Тестирование переменной TEMP с кодом типа из источника, который может вернуть значение в нижнем регистре, с известным значением.
```xml
<if test="toUpper(TEMP.CODE) = 'FOO'"/>
```



[На главную](./)