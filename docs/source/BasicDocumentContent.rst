﻿BasicDocumentContent
====================

Объект представляет собой содержание акта о выполнении работ в неформализованном виде, ТОРГ-12 в неформализованном виде или счета на оплату.
Является производным объектом от :doc:`BaseContent <BaseContent>`.

Свойства объекта
----------------


- **Date** (дата, чтение/запись) - дата документа

- **Number** (строка, чтение/запись) - номер документа

- **Total** (число с плавающей точкой, чтение/запись) - сумма с учетом НДС

- **Vat** (число с плавающей точкой, чтение/запись) - сумма НДС

- **Grounds** (строка, чтение/запись) - основание документа

- **NeedRecipientSignature** (булево, чтение/запись) - флаг, обозначающий запрос подписи получателя под отправляемым документом

- **Type** (строка, чтение) - тип документа. Используется всеми типами содержимого. Может возвращать значения:

  - "AcceptanceCertificatey" -- для акта о выполнении работ
  - "NonformalizedProforma" -- для счета на оплату
  - "Torg12" -- для ТОРГ-12


Методы отсутствуют
