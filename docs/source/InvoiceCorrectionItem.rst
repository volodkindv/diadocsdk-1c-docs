﻿InvoiceCorrectionItem
=====================

Сведения о товаре (работе, услуге) корректировочной счета-фактуры

Свойства объекта
----------------


- **Product** (строка, чтение/запись, обязательно для заполнения. Длина строка не более 1000 символов) - наименование товара

- **OriginalValues** (объект :doc:`InvoiceItemFields <InvoiceItemFields>`, чтение, обязательно для заполнения) - значения до корректировки

- **CorrectedValues** (объект :doc:`InvoiceItemFields <InvoiceItemFields>`, чтение, обязательно для заполнения) - значения после корректировки

- **AmountsInc** (объект :doc:`AmountsDiff <AmountsDiff>`, чтение) - суммы к увеличению

- **AmountsDec** (объект :doc:`AmountsDiff <AmountsDiff>`, чтение) - суммы к уменьшению

- **StructedAdditionalInfos** (:doc:`коллекция <Collection>` объектов :doc:`StructedAdditionalInfo <StructedAdditionalInfo>`, чтение/запись) - дополнительные сведения


Методы объекта
--------------

-  :doc:`AddStructedAdditionalInfo <AddStructedAdditionalInfo-(InvoiceCorrectionItem)>` - добавляет строку дополнительных сведений


.. toctree::
   :name: Auto
   :hidden:

   AddStructedAdditionalInfo <AddStructedAdditionalInfo-(InvoiceCorrectionItem)>