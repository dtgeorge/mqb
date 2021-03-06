# Параметры омывателя фар и дворников

### Настройка омывателя фар

Отключение срабатывания омывателей фар при каждом 10 включении омывателей ветрового стекла
```
Блок 09 → Адаптация
> Scheinwerferreinigung - Anzahl Betaetigungen Frontwaschanlage pro SRA Aktivierung
Старое значение: 10
Новое значение: 0
→ Применить
```

Аналог:
```[VO]_Scheinwerferreinigunglage -> неактив```
    
Cрабатывание после долгого удержания рычага омывания стекла
```
Блок 09 → Адаптация
> Scheinwerferreinigung - SRA Verzoegerungszeit
Старое значение: 0 мс
Новое значение: 2500 мс
→ Применить
```

Отключение второго "пшика" на фары (не рекоммендуется)
```
Блок 09 → Адаптация
> Scheinwerferreinigung - SRA Nachwaschzeit
Старое значение: 10
Новое значение: 0 ms
→ Применить
```

> логин-пароль 31347

### Сервисное положение дворников

	Блок 09  → Адаптация
	> Service position → вводим нужное значение
	→ Применить
	> Alternative position 2 (позиция дворников при выключенном зажигании)
	→ Применить
	
	Меню в магнитоле
    > Front wiper
    > Menuesteuerung Frontwischer — active
    → Применить

> логин-пароль 31347

!!! info
    Service position: по умолчанию 166.505329 градусов, меняем в меньшую сторону.  
    Меню в ГУ появляется не на всех машинах

### Дотирка капель – Лобовое стекло

	Блок 09 → Адаптация
	> Front_wiper 
	> Traenenwischen Front Status → активировать
	→ Применить

> логин-пароль 31347

### Работа заднего дворника во время дождя

    Блок 09 → Адаптация
    > Задний стеклоочиститель (Rear Wiper / Heckwischersteuerung)
    > Automatisches Heckwischen  → активировать
    > Einzelansteuerung Heckintervallwischen Zeitintervall 1
    Поменять с 7s на 15s
	→ Применить
	
	ODIS E:
	IDE02711-ENG116690-Rear Window Wiper-Automatisches Heckwischen
	
> логин-пароль 31347
