# getReportField

---

Эта функция возвращает определенное поле отчета в том виде, в котором он хранится в базе данных.
Эта функция может принимать два различных набора аргументов.
Если первый аргумент является числовым, он обрабатывается как ключ отчета, поле которого требуется получить,
а второй ключ как имя целевого поля. Ниже приводится пример такого сценария.
Если первый аргумент это строка, предполагается, что первые два аргумента являются ID и кодом исходной системы отчета, а третий аргумент это имя целевого поля

#### Возвращает:

Неизвестно

## Аргументы

|  | Имя аргумента | Описание | Тип значения |
| --- | --- | --- | --- |
| 1 | reportKey | Поле report_rk. | `Long` |
| 2 | destFieldName | Имя поля в отчете. | `String` |

## Примеры

**Пример 1:** Пример использования приводится в описании компонента GetPartyField.