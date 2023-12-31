## Журнал событий Windows 10

# Открытие журнала событий для Windows 10

Существует несколько способов открытия журнала событий:

**```Первый способ```**

1. Нажмите ПКМ на кнопку "Пуск" в левом нижнем углу экрана.
2. В выпадающем списке выберите "Просмотр событий". Это откроет окно "Журнал событий".

**```Второй способ```**

1. Нажмите на кнопку "Поиск" в левом нижнем углу экрана. 
2. Введите в поле поиска "Просмотр событий" и нажмите Enter. 
3. В списке результатов поиска выберите "Просмотр событий". Откроется окно "Журнал событий".

**```Третий способ```**

1. Нажмите комбинацию клавиш Win+R на своей клавиатуре. Это откроет окно "Выполнить".
2. В поле ввода "Выполнить" введите "eventvwr" без кавычек.
3. Нажмите Enter или нажмите кнопку "ОК". Откроется окно "Журнал событий".

Эти три способа позволяют открыть журнал событий на компьютере с операционной системой Windows 10. Журнал событий - это инструмент, который позволяет просматривать информацию о состоянии компьютера, производительности, приложениях и системных событиях. 
___

В **```«Журналах Windows»```** содержатся:

 ```Журнал``` | ```Содержание``` | ```Примеры событий``` | ```Используется группами``` |
| --- | --- | --- | --- |
| **Приложения** | События, связанные с работой конкретных приложений, не системо-генерированные | Ошибки в работе сервера базы данных, сбои в резервном копировании базы данных | Разработчики программ, администраторы |
| **Безопасность** | События, связанные с безопасностью системы, такие как попытки входа в аккаунты системы, изменение прав доступа к ресурсам и управление учетными записями | Записи об успешных и неуспешных попытках входа, изменение прав доступа к папкам | Администраторы безопасности, специалисты по информационной безопасности, цифровые эксперты |
| **Система** | События, связанные с операционной системой и её компонентами, системо-генерированные | Ошибки при инициализации драйверов, запуске служб и отказы драйверов | Системные администраторы, технические специалисты |
___
Журналы событий в операционной системе Windows являются важными инструментами для администрирования и обслуживания системы. Они содержат информацию о различных событиях, которые происходят в системе, таких как ошибки, предупреждения, уведомления и другие. В Windows есть три основных журнала событий: Приложения, Безопасность и Система.

Журнал событий Приложений содержит информацию о событиях, связанных с работой конкретных приложений. Эти события неявляются системно-генерированными, так как различные приложения имеют различные функции и возможности. В журнале событий Приложений могут быть записаны ошибки, предупреждения и сообщения о работе приложений. Например, сервер базы данных может записывать ошибки, возникающие при его работе в журнал приложений. Разработчики программ сами решают, какие события имеет смысл протоколировать в журнале событий Приложения. При этом события, сгенерированные разными приложениями, попадают в единый журнал приложений. Приложения идентифицируются как разные "источники" в базовом свойстве событий.

Журнал событий Безопасности содержит информацию о попытках входа в аккаунты системы, изменении прав доступа к ресурсам и управлении учетными записями. Эти события, в отличие от журнала Приложений, являются системно-генерированными и строго контролируются администратором системы. Например, посредством настройки журнала Безопасности можно отслеживать активность пользователей и принимать меры для обеспечения безопасности системы. Стоит отметить, что настройка журнала Безопасности может быть достаточно сложной задачей, так как его настройка требует особое внимание к конфигурации системы и компетентность в области безопасности.

Журнал событий Системы содержит информацию о событиях, связанных с операционной системой и её компонентами. Эти события, как и в журнале Приложений, являются не системно-генерированными и могут содержать информацию об ошибке запуска сервисов или драйверов, отказах и других проблемах, возникающих в процессе работы системы. Журнал событий Системы является важным инструментом для диагностики проблем в системе и помогает устранять неполадки.

Таким образом, журналы событий в Windows являются неотъемлемой частью системы и позволяют администраторам следить за работой приложений, обеспечивать безопасность системы и диагностировать проблемы в системе. Каждый журнал содержит информацию, необходимую для определения причины возникновения события и принятия соответствующих мер. Однако настройка журналов может быть сложной задачей, требующей определенных знаний и компетенций.
___

## Команды в cmd

Команда **```arp -a```** отображает таблицу соответствия IP и MAC адресов для данного компьютера (текущую таблицу ARP)

Команда **```driverquery```** позволяет администратору просмотреть список установленных драйверов устройств. Отображаемые данные могут быть представлены в виде списка, таблицы, или CSV ( Comma-Separated Values - значения, разделённые запятыми).
