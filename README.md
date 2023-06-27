# Формирование XML пакетов #

# Включение позиции в опубликованный в ЕИС план-график #

Исходящий файл: 1.xml (должен соответствовать схеме fcsIntegration.xsd)  
Входящий файл: tenderPlan2020_202203722002539001_8053457.xml (должен соответствовать схеме fcsExport.xsd)

    Действия с тегами во входящем файле:

    Атрибуты "schemeVersion" тегов <ns2:tenderPlan2020> входящего файла и <ns:data> исходящего файл должны быть одинаковые

    <ns5:id> - последние 4 цифры текста тега меняем на 4 случайные цифры   
    <ns5:externalId> - текст тега меняем на текст тега <externalId> исходящего файла   
    <ns5:planNumber> - текст тега меняем на текст тега <planNumber> исходящего файла

    /ns2:export/ns2:tenderPlan2020/ns5:positions/ns5:position/ns5:commonInfo/ - xpath для поиска обычной закупки

    <ns5:positionNumber> - последние 4 цифры текста тега меняем на 4 случайные цифры   
    <ns5:extNumber> - текст тега меняем на текст тега <extNumber> исходящего файла   
    <ns5:IKZ> - текст тега меняем на текст тега <IKZ> исходящего файла   
    <ns5:publishYear> - текст тега меняем на текст тега <publishYear> исходящего файла   
    <ns5:IKU> - текст тега меняем на текст тега <IKU> исходящего файла   
    <ns5:purchaseNumber> - текст тега меняем на текст тега <purchaseNumber> исходящего файла    
    <ns5:purchaseObjectInfo> - текст тега меняем на текст тега <purchaseObjectInfo> исходящего файла   
    <ns5:publicDiscussion> - текст тега меняем на текст тега <publicDiscussion> исходящего файла

    После внесения изменений входящий файл необходимо сохранить и отправить*!

### Ожидаемый результат: ###

Плана-графика находится в реестре: Планирование -> Планы-графики (с 2020 года) -> Мои планы-графики (с 2020 года)  
Статус плана-графика: "Идет отправка на контроль" -> "Опубликован в ЕИС"  
Статус позиции плана-графика: "Ожидает публикации в плане-графике ЕИС" -> "Включена в опубликованный в ЕИС план-график"
***

# Формирование извещения (Электронный аукцион) #

## 1. Стадия "Ожидание публикации" ##

Исходящий файл: 2.xml (должен соответствовать схеме fcsIntegration.xsd)  
Входящий файл: 5975222_oosconfirm_xml.xml (должен соответствовать схеме fcsIntegration.xsd)

    Действия с тегами во входящем файле:

    Атрибуты "schemeVersion" тегов <data> входящего файла и <main:data> исходящего файл должны быть одинаковые

    <id> - последние 4 цифры текста тега меняем на 4 случайные цифры
    <ns2:loadId> - последние 4 цифры текста тега меняем на 4 случайные цифры
    <ns2:refId> - текст тега меняем на текст тега <main:id> исходящего файла

    После внесения изменений входящий файл необходимо сохранить и отправить*!

### Ожидаемый результат: ###

Извещение находится в реестре: Определение поставщика -> Извещения о размещении -> В работе  
Статус позиции: "Идет отправка в ЕИС (извещение)" -> "Ожидание публикации"

## 2. Стадия "Подача ценовых предложений" ##

Исходящий файл: 2.xml (должен соответствовать схеме fcsIntegration.xsd)  
Входящий файл: 1427epNotificationEF2020_0372200000923000013_31563898.xml (должен соответствовать схеме fcsExport.xsd)

    Действия с тегами во входящем файле:

    Атрибуты "schemeVersion" тегов <ns2:epNotificationEF2020> входящего файла и <main:data> исходящего файл должны быть одинаковые

    <ns9:id> - последние 4 цифры текста тега меняем на 4 случайные цифры
    <ns9:externalId> - текст тега меняем на текст тега <externalId> исходящего файла   
    <ns9:purchaseNumber>[первый тег сначала] - последние 4 цифры текста тега меняем на 4 случайные цифры
    <ns9:docNumber> - последние 4 цифры текста тега меняем на 4 случайные цифры
    <ns9:plannedPublishDate> - текст тега меняем на текущую дату в исходном формате
    <ns9:publishDTInEIS> - текст тега меняем на текущую дату в исходном формате
    <ns9:purchaseObjectInfo> - текст тега меняем на текст тега <purchaseObjectInfo> исходящего файла  
    <ns3:docDate> - текст тега меняем на текущую дату в исходном формате
    <ns3:docDate> - текст тега меняем на текущую дату в исходном формате
    <ns9:endDT> - текст тега меняем на текст тега <endDT> исходящего файла 
    <ns9:summarizingDate> - текст тега меняем на текст тега <summarizingDate> исходящего файла 
    <ns9:sid> - последние 4 цифры текста тега меняем на 4 случайные цифры
    <ns9:externalSid> - текст тега меняем на текст тега <externalSid> исходящего файла 

    После внесения изменений входящий файл необходимо сохранить и отправить*!

### Ожидаемый результат: ###

Извещение находится в реестре: Определение поставщика -> Извещения о размещении -> В работе  
Статус позиции: "Ожидание публикации" -> "Подача ценовых предложений"

## 3. Стадия "Заключение контракта" ##

Исходящий файл: 2.xml (должен соответствовать схеме fcsIntegration.xsd)  
Входящий файл: 1051epProtocolEF2020Final_0372200280322000019_37810684.xml (должен соответствовать схеме fcsExport.xsd)

    Действия с тегами во входящем файле:

    Атрибуты "schemeVersion" тегов <data> входящего файла и <main:data> исходящего файл должны быть одинаковые

    <ns9:id> - последние 4 цифры текста тега меняем на 4 случайные цифры
    <ns9:externalId> - текст тега меняем на текст тега <externalId> исходящего файла   
    <ns9:purchaseNumber> - текст тега меняем на текст тега <<ns9:purchaseNumber> входящего файла на стадии 2
    <ns9:publishDTInEIS> - текст тега меняем на текущую дату в исходном формате
    <ns9:publishDTInETP> - текст тега меняем на текущую дату в исходном формате
    <ns9:procedureDT> - текст тега меняем на текущую дату в исходном формате
    <ns9:signDT> - текст тега меняем на текущую дату в исходном формате
    <ns3:docDate> - текст тега меняем на текущую дату в исходном формате
    <ns3:docDate> - текст тега меняем на текущую дату в исходном формате

    После внесения изменений входящий файл необходимо сохранить и отправить*!

### Ожидаемый результат: ###

Контракт находится в реестре: Исполнение -> Регистрация контрактов -> Контракты на этапе заключения  
Статус позиции: "Подача ценовых предложений" -> "Заключение контракта"
***

# Исполнение контракта #

## 1. Стадия "Ожидание публикации (контракт)" ##

Исходящий файл: 3.xml (должен соответствовать схеме fcsIntegration.xsd)  
Входящий файл: 5975222_oosconfirm_xml.xml >!(должен соответствовать схеме fcsIntegration.xsd)

    Действия с тегами во входящем файле:

    Атрибуты "schemeVersion" тегов <data> входящего файла и <ext:data> исходящего файл должны быть одинаковые

    <id> - последние 4 цифры текста тега меняем на 4 случайные цифры
    <createDateTime> - текст тега меняем на текущую дату в исходном формате
    <ns2:loadId> - последние 4 цифры текста тега меняем на 4 случайные цифры
    <ns2:refId> - текст тега меняем на текст тега <ext:id> исходящего файла

    После внесения изменений входящий файл необходимо сохранить и отправить*!

### Ожидаемый результат: ###

Контракт находится в реестре: Исполнение -> Регистрация контрактов -> Контракты на этапе заключения  
Статус позиции: "Заключение контракта" -> "Ожидание публикации (контракт)"

## 2. Стадия "Исполнение контракта. Часть 1" ##

Исходящий файл: 3.xml (должен соответствовать схеме fcsIntegration.xsd)  
Входящий файл: contract_2780804383319000083_41655568_admin_1201 (должен соответствовать схеме fcsExport.xsd)

    Действия с тегами во входящем файле:

    Атрибуты "schemeVersion" тегов <ns2:epNotificationEF2020> входящего файла и <main:data> исходящего файл должны быть одинаковые

    <id> - последние 4 цифры текста тега меняем на 4 случайные цифры
    <externalId> - текст тега меняем на текст тега <externalId> исходящего файла 
    <placementDate> - текст тега меняем на текущую дату в исходном формате
    <publishDate> - текст тега меняем на текст тега <publishDate> исходящего файла 
    <foundation> - тега меняем на тег <foundation> исходящего файла 
    <customer> - тега меняем на тег <customer> исходящего файла 
    <placer> - тега меняем на тег <placer> исходящего файла 
    <finances> - тега меняем на тег <finances> исходящего файла 
    <cmn:plan2020Number> - название тега меняем на <ns3:plan2020Number>
    <cmn:position2020Number> - название тега меняем на <ns3:position2020Number>
    <protocolDate> - текст тега меняем на текст тега <protocolDate> исходящего файла 
    <documentCode> - последние 4 цифры текста тега меняем на 4 случайные цифры
    <signDate> - текст тега меняем на текст тега <signDate> исходящего файла 
    <regNum> - последние 4 цифры текста тега меняем на 4 случайные цифры
    <number> - текст тега меняем на текст тега <number> исходящего файла 
    <contractSubject> - текст тега меняем на текст тега <contractSubject> исходящего файла 
    <priceInfo> - тега меняем на тег <finances> исходящего файла 
    <executionPeriod> - тега меняем на тег <executionPeriod> исходящего файла 
    <products> - тега меняем на тег <products> исходящего файла 
    <docRegNumber> - текст тега меняем на текст тега <regNum> входящего файла 
    <docRegNumber> - текст тега меняем на текст тега <regNum> входящего файла 
    <docRegNumber> - текст тега меняем на текст тега <regNum> входящего файла 

    После внесения изменений входящий файл необходимо сохранить и отправить*!

### Ожидаемый результат: ###

Контракт находится в реестре: Исполнение -> Реестр контрактов -> Контракты на этапе исполнения (последняя страница)  
Статус позиции: "Ожидание публикации (контракт)" -> "Исполнение контракта"

## 3. Стадия "Исполнение контракта. Часть 2" ##

Исходящий файл: 4.xml (должен соответствовать схеме fcsIntegration.xsd)  
Входящий файл: contractProcedure_2781148800721000013_181831266.xml (должен соответствовать схеме fcsExport.xsd)

    Действия с тегами во входящем файле:

    Атрибуты "schemeVersion" тегов <ns2:contractProcedure> входящего файла и <ext:data> исходящего файл должны быть одинаковые

    <ns2:id> - последние 4 цифры текста тега меняем на 4 случайные цифры
    <ns2:regNum> - текст тега меняем на текст тега <regNum> исходящего файла   
    <ns2:publishDate> - текст тега меняем на текущую дату в исходном формате
    <endDate> - текст тега меняем на текст тега <endDate> исходящего файла

    <fulfilledCost> - текст тега меняем на текст тега <fulfilledCost> исходящего файла   
    <docRegNumber> (все теги) - текст тега меняем на текст тега <regNum> исходящего файла   

    <executions>
        <execution>
            <docAcceptance> - меняеем текс теги у всех документов
                <sid> - добавить новый тег с текстом (любое число)
                <code> - текст тега меняем на текст тега <code> исходящего файла   
                <name> - текст тега меняем на текст тега <name> исходящего файла   
                <documentDate> - текст тега меняем на текст тега <documentDate> исходящего файла           
                <documentNum> - текст тега меняем на текст тега <documentNum> исходящего файла   
                <deliveryAcceptDate> - текст тега меняем на текст тега <deliveryAcceptDate> исходящего файла

    После внесения изменений входящий файл необходимо сохранить и отправить*!

### Ожидаемый результат: ###

Контракт находится в реестре: Исполнение -> Реестр контрактов -> Контракты на этапе исполнения (последняя страница)  
Статус позиции: "Ожидание публикации (контракт)" -> "Исполнение контракта"

***

#       * Отправка файла (пакета xml) #

    1. Авторизоваться на тестовом стенде по логину "Semenova1"
    2. В панели пользователя выбрать: Администрирование -> Контент -> Загрузка файлов во входящие
    3. Нажать кнопку "Выбрать и загрузить файл" и выбрать входящий файл
    4. Нажать кнопку "Принять и очистить"

#       Глоссарий тегов #

    <finalStageExecution> - закроет контракт (True/False)
    <regNum> - реестровый номер контракта (int)