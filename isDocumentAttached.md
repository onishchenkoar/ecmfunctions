# isDocumentAttached

---

Возвращает значение `true` если дело содержит один или несколько документов, в противном случае возвращает `false`.

#### Возвращает:

Неизвестно

## Аргументы

|  | Имя аргумента | Описание | Тип значения |
| --- | --- | --- | --- |
| 1 | caseRk | Указывает дело, для которого нужно искать вложенные документ (необязательно). Если этот параметр пропущен, предполагается, что эта функция используется со страницей Дело и будет применяться к данному делу. | `String` |

## Примеры

**Пример 1:** Присваивает параметру значение true если текущее дело содержит прикрепленные документы.
```xml
<param name="hasAttachments" value="IsDocumentAttached()" />
```



[На главную](./)