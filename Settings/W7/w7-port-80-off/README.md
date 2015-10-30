Освободить  порт 80 занятый system в windows 7 
удалось следующим путем.

1. Win+R вводим “regedit” (без  ковычек).
2. Ищем ветку «HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\HTTP»
3. Меняем значение ключа “start” с 3 на 4…до этого встречал советы ставить 0. Так вот мне ноль не помог.
4. Перезапускаем компьютер.

http://myhelpit.ru/index.php?id=163
