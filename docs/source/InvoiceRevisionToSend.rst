﻿InvoiceRevisionToSend
=====================

Объект представляет собой документ "исправление счета-фактуры" на отправку 
и является производным объектом от :doc:`DocumentToSend <DocumentToSend>`.

Свойства объекта
----------------

- **Content** (чтение/запись) - содержимое документа, объект :doc:`InvoiceContent <InvoiceContent>`

- **Type** (строка, чтение) - тип документа (возвращает строку "InvoiceRevision")

- **Comment** (строка, чтение/запись) - комментарий к документу

- **CustomDocumentId** (строка, чтение/запись) - внешний идентификатор документа


Методы отсутствуют.