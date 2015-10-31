### При установке **Apache**:

Был добавлен **path** для **Apache**:

    ;d:\server\apache;d:\server\apache\bin;d:\server\php; 

Был добавлен файл **MSVCR110.dll**

Был установлен сервис **Apache**:

    d:\server\apache\bin\httpd.exe -k install 

Был создан на рабочем столе ярлык для `d:\server\apache\bin\ApacheMonitor.exe` 
и помещён в автозагрузку.

### При установке **PHP**:

Ничего системного.

### При установке **MySQL**:

Работал `.msi`.

## **Удаление**:

+ Из **Программы и компоненты** удалить **MySQL Installer** и **MySQL Server**.
+ Остановить **Apache**.
+ Закрыть **ApacheMonitor**.
+ Удалить **ApacheMonitor** из **Автозагрузки**.
+ Удалить ярлык **ApacheMonitor** с **Рабочего стола**.
+ В **Консоли** под Администратором удалить службу **Apache**:

~~~
        sc delete Apache2.4
~~~


