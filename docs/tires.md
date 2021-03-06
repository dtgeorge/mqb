# Настройка профилей шин

### Настройка системы контроля давления в шинах через Individual профиль

!!! tip
    В старых версиях OBD11 был перепутан перевод (обычный - полный)
    
Настройки для обычной нагрузки

    Блок 65 → Адаптация

    > НОМ. давление для передней оси, обычный
    Старое значение: 255
    Новое значение: 22 (если нужно 2.2 бара)
    → Применить
    
    > НОМ. давление для задней оси, обычный
    Старое значение: 255
    Новое значение: 22 (если нужно 2.2 бара)
    → Применить

Настройки для полной нагрузки

    > НОМ. давление Полная загрузка передней оси
    Старое значение: 255
    Новое значение: 26 (если нужно 2.6 бара)
    → Применить
    
    > НОМ. давление Полная загрузка задней оси
    Старое значение: 255
    Новое значение: 26 (если нужно 2.6 бара)
    → Применить

### Создание собственно профиля шин

+ [Online генератор TMPS](generator.html)

Поддерживающиеся блоки:   
3AA907273D; 3AA907273F; 3AA907273H; 5Q0907273; 5Q0907273B; 7P6907273H; 7P6907273L.

Для генерации необходимо выбрать нужный формат (какой утилитой будет проводиться загрузка) и правильный блок шин. 
Потом надо создать/наполнить таблицу давлений для него. 
В качестве названий может быть что угодно - размерность шин, названия Зима-Лето и т.д.

Готовый файл заливается с помощью ODIS E или VCDS в блок 65:

> Diagnostic function - Write Data Record

![Screenshot](../images/odis-e-tires.png) 

После загрузки данных меню настроек будет выглядить так:
![Screenshot](../images/tires.jpg) 
    
!!! warning
    После записи машина на некоторое время станет новогодней ёлкой - будут ошибки и отказы по всем блокам.   
    Беспокоиться не надо - в течение 10 минут все само починится.