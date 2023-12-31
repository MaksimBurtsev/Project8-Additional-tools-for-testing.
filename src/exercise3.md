# Что такое лог?
```Лог (log)``` — это текстовый файл, куда автоматически записывается важная информация о работе системы или программы. Чаще всего говорят о логах сервера. Их записывает программное обеспечение, которое управляет внутренней частью сайта или онлайн-системы. Логи являются важным элементом мониторинга работоспособности IT-систем. Они позволяют быстро выявлять проблемы и ошибки, упрощают процесс их анализа и устранения. 
Например, логи серверов могут содержать информацию о том, какие запросы к серверу были сделаны, какие ошибки возникли в процессе выполнения запросов, а также данные о трафике и нагрузке на сервер. Логи баз данных могут содержать информацию о совершенных операциях с базами данных, а логи почтовых сервисов содержат информацию об отправленных и полученных письмах. 
Чтение логов может быть сложным и требовательным к времени процессом, поэтому существуют специализированные инструменты для их анализа и управления, которые значительно облегчают работу с логами и позволяют быстро находить и устранять ошибки.
___
# Какие существуют типы и уровни логов?


## Типы логов
Для удобства обработки логов их делят на типы:

| ```Тип логов```           | ```Описание```                                       |
|---------------------------|------------------------------------------------------|
| Системные                 | Отслеживают системные события, такие как запуск и выключение системы, ошибки в работе операционной системы и драйверов устройств. |
| Серверные                 | Фиксируют процессы обращения к серверу, ошибки при доступе к ресурсам, работу сетевых протоколов, обработку запросов и передачу данных. |
| Почтовые                  | Отражают процессы отправления и доставки электронной почты, ошибки в работе почтовых серверов, фильтрацию спама. |
| Логи баз данных           | Содержат информацию о процессах обращения к базам данных, ошибки в работе SQL-запросов, изменения в структуре таблиц и другую важную информацию. |
| Авторизационные и         | Фиксируют процесс входа, выхода из системы, смены пароля, восстановления доступа и другие действия, связанные с безопасностью. |
  аутентификационные        |                                                      |
___
## Уровни логов

Хотя логи должны записываться на протяжении работы всех IT-систем, их беспорядочное сбора, без фильтрации и группировки, может создать ненужный шум и лишить их практической пользы. Чтобы снять максимальную выгоду из логов, им необходима настройка фильтров и упорядочение их по уровням, что обеспечит быстрый поиск информации и проблем. 

### Чтобы упростить поиск и чтение логов, их делят на уровни. Основных четыре:

| **```Уровень логов```** | **```Описание```**  |
|---------------|------------------------------------------------------|
| ```Debug```   | Этот уровень фиксирует события, связанные с масштабными переходами состояний системы, например, обращение к базе данных, старт/пауза сервиса, успешная обработка записи и т.д. Уровень Debug применяется во время разработки, тестирования программного обеспечения, но может быть полезен и на продакшен-серверах при поиске причин нештатных ситуаций. |
|```Warning```  | Этот уровень логов сообщает о потенциальной проблеме, которая еще не вызвала ошибку в работе системы. Например, запись Warning может указывать на странный формат запроса или некорректный параметр вызова. |
| ```Error```   | Этот уровень логов фиксирует типичные ошибки, которые могут возникнуть во время работы системы. Это могут быть ошибки в работе с базой данных, сетевых протоколов, файловых систем и других компонентов. |
| ```Fatal```   | Этот уровень логов предназначен для фиксации тотального сбоя работоспособности системы. Он сообщает о ситуациях, когда нет доступа к базе данных или сети, сервису не хватает места на жестком диске и других серьезных проблемах, которые блокируют работу системы. |

### Дополнительно файл логирования может расширяться записями еще двух уровней:
|               |                                                                                                                                                                  |
|---------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ```Trace```   | Trace-логирование используется для фиксации пошаговых записей процесса и может быть полезно при поиске причин нештатных ситуаций.                                       |
| ```Info```    | Уровень логов Info содержит общую информацию о работе службы или сервиса. Сюда относятся сообщения о запуске и остановке приложения, успешной инициализации, изменениях конфигурации и других действиях, которые не требуют дополнительного анализа. |
___

# Какое расширение имеет файл с логами?

Лог-файлы имеют различные расширения в зависимости от ПО, которое записывает эти логи. Существует множество расширений, но наиболее часто встречаемые:

|**```Название```** |**```Описание```**|
|---------|-------------------------------------------|
|```.log```|Это наиболее распространенное расширение для файлов логов. Оно используется во многих приложениях и системах для сохранения текстовых записей о событиях и действиях.|
|```.txt```|Хотя расширение .txt обычно ассоциируется с обычными текстовыми файлами, оно также может быть использовано для файлов логов, особенно если логи представлены в текстовом формате.|
|```.syslog```|Расширение .syslog обычно используется для файлов логов в формате системного журнала в операционных системах Unix или Linux.|

# Какие программы используются для просмотра логов?

Для просмотра логов можно использовать текстовые редакторы такие как:
| **```Программа```**   | **```Описание```**                                                                                                                                                                                                                                                                                                                                                  |
|-------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ```Notepad++```   | Бесплатный редактор кода и текста, с поддержкой многих языков программирования и форматов документов. Он может читать и отображать большие файлы логов, делая его полезным для просмотра и анализа записей логов в списках.                                                                                                          |
| ```TextPad```     | Платный текстовый редактор, работающий с текстовыми файлами различных размеров и типов. Несмотря на то, что TextPad не имеет специфической функциональности для работы с лог-файлами, с помощью соответствующих настроек комментариев и подсветки синтаксиса, он может быть использован для удобного просмотра и анализа лог-файлов. |
| ```Atom```        | Бесплатный редактор кода и текста с множеством плагинов для настройки и улучшения функциональности. Atom имеет встроенные возможности для работы с лог-файлами, в частности, он может автоматически проанализировать формат файла и подсветить значения дат, времени или других ключевых слов, что делает просмотр и анализ записей логов более удобным и понятным. |
___
А так же можно использовать различные инструменты анализа логов, например:
___
| **```Название сервиса```** | **```Описание```**                                                                                                                                                                                   |
|------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ```Papertrail```       | Облачный сервис для работы с лог-файлами и инструментальным анализом. Бесплатный план позволяет хранить 100 МБ данных в месяц, использовать готовые решения, такие как сортировка, фильтрация, агрегация, мониторинг состояния, оповещения и т. д. |
| ```Loggly```           | Онлайн-сервис для сбора лог-файлов. Бесплатная пробная версия позволяет загружать до 200 МБ данных ежедневно и хранить их в течение 7 дней. Позволяет глубоко анализировать журналы и настраивать мгновенные оповещения.                                 |
| ```Datadog```          | Онлайн-сервис для сбора, поиска и анализа лог-файлов. Поддерживает множество типов логов, позволяет создавать динамические дашборды и настраивать мгновенные уведомления. Бесплатная версия планировщика позволяет загружать до 5 ГБ данных в месяц.           |
___