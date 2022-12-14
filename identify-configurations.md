# План управления конфигурацией

## Идентификация конфигураций

Цель мероприятия по идентификации конфигурации – однозначно определить каждую единицу конфигурации (и её последовательные версии) так, чтобы обеспечить основу для управления единицами конфигурации и ссылки на них.

В данном разделе описывается подход к процессу идентификации следующих элементов конфигурации:
* документов;
* сообщений о проблемах;
* запросов на изменения;
* программного кода.

### Идентификация документа

Версии документов идентифицируются по их названию. Название имеет составную структуру: имя, отражающее суть документа, нижнее подчеркивание, дата изменения в формате год, месяц, день, час, минута. Итоговый формат названия можно описать в виде следующего шаблона: \<Name\>\_\<YYYYMMdd\_hhmm\>. Пример: План\_20220930_1830.

Уникальность идентификации обеспечивается его связью с временем изменения.

### Идентификация сообщения о проблеме

Сообщения о проблемах регистрируются в issue соответствующего репозитория проекта на Github (см. описание инструментария). 

Сообщения о проблемах идентифицируются уникальным номером, который работает по инкрементному принципу, его функционирование обеспечивается сервисом Github (см. описание инструментария).

### Идентификация запроса на изменения

Запросы на применение изменений регистрируются в соответствующем репозитории проекта на Github (см. описание инструментария).

Идентификация запросов обеспечивается присваиванием уникального номера, который работает по инкрементному принципу, его функционирование обеспечивается сервисом Github (см. описание инструментария). 

### Идентификация программного кода

Программный код идентифицируется при помощи возможности проставлять теги (tags), реализованной в системе Github (см. описание инструментария). Теги для базовых версий и производных от них проставляются путем использования github-actions после успешной сборки версии проекта. 

Уникальность обеспечивается инкрементной логикой работы тегов.
