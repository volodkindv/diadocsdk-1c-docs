﻿ExtendedInvoiceItem
===================

Объект предназначен для редактирования строки табличной части счета-фактуры.


Свойства объекта
----------------

- **Product** (строка, чтение/запись, обязательно для заполнения, строка длиной не более 1000 символов) - наименование товара

- **UnitCode** (строка, чтение/запись, числовая строка длиной 3 символа) - код единицы измерения товара. Код должен содержаться в Общероссийском классификаторе единиц измерения.
  Если единицы измерения нет в классификаторе, требуется указать в качестве кода значение "0000" и указать наименование единицы измерения товара (поле **UnitName**). В этом случае поле **UnitName**
  будет обязательным для заполнения

- **UnitName** (строка, чтение/запись) - наименование единицы измерения товара. Обязательно для заполнения в случае, если в качестве значения поля **UnitCode** указано "0000"

- **Quantity** (число с плавующей запятой, чтение/запись) - количество единиц товара

- **Price** (число с плавующей запятой, чтение/запись) - цена за единицу товара без НДС

- **Excise** (строка, чтение/запись) - акциз

- **TaxRate** (строка, чтение/запись, обязательно для заполнения) - ставка НДС

- **SubtotalWithVatExcluded** (число с плавующей запятой, чтение/запись) - сумма без учета НДС

- **Vat** (число с плавующей запятой, чтение/запись) - сумма НДС

- **Subtotal** (число с плавующей запятой, чтение/запись, обязательно для заполнения) - сумма всего

- **ItemMark** (строка, чтение/запись) - признак товар-работа-услуга

- **AdditionalProperty** (строка, чтение/запись, строка длиной не более 4 символов) - дополнительная информация о признаке

- **VendorCode** (строка, чтение/запись, строка длиной не более 255 символов) - характеристика/код/артикул/сорт товара

- **ToRelease** (число с плавующей запятой, чтение/запись) - количество товара, которое надлежит отпустить

- **AccountDebit** (строка, чтение/запись, числовая строка длиной не более 9 символов) - корреспондирующие счета: дебет

- **AccountCredit** (строка, чтение/запись, числовая строка длиной не более 9 символов) - корреспондирующие счета: кредит

- **CustomDeclarations** (:doc:`коллекция <Collection>` объектов :doc:`CustomDeclaration <CustomDeclaration>`, чтение) - номера таможенных деклараций

- **StructedAdditionalInfos** (:doc:`коллекция <Collection>` объектов :doc:`StructedAdditionalInfo <StructedAdditionalInfo>`, чтение) - информационное поле документа


Свойство **TaxRate** принимает одно из следующих значений:

-  "10/110" - ставка налога 10/110 (дробь)
-  "18/118" - ставка налога 18/118 (дробь)
-  "без НДС" - без НДС
-  "0" - ставка налога 0%
-  "10" - ставка налога 10%
-  "18" - ставка налога 18%


Свойство **ItemMark** принимает одно из следующих значений:

-  "NotSpecified" - не указано
-  "Property" - имущество
-  "Job" - работа
-  "Service" - услуга
-  "PropertyRights" - имущественные права
-  "Other" - иное


Методы объекта
--------------

-  :doc:`AddCustomDeclaration <AddCustomDeclaration>` - добавляет основание отгрузки

-  :doc:`AddStructedAdditionalInfo <AddStructedAdditionalInfo-(ExtendedInvoiceItem)>` - добавляет строку дополнительных сведений


.. toctree::
   :name: Auto
   :hidden:

   AddCustomDeclaration <AddCustomDeclaration>
   AddStructedAdditionalInfo <AddStructedAdditionalInfo-(ExtendedInvoiceItem)>
