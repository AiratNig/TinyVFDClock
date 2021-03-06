# TinyVFDClock

Часы на вакуумно-люминесцентных индикаторах ИВ-12 и ИВ15.

<img src="https://github.com/AiratNig/TinyVFDClock/blob/main/img/IMG_3808.JPG" width="30%"> <img src="https://github.com/AiratNig/TinyVFDClock/blob/main/img/IMG_3806.JPG" width="30%"> <img src="https://github.com/AiratNig/TinyVFDClock/blob/main/img/IMG_4371.JPG" width="30%"> <img src="https://github.com/AiratNig/TinyVFDClock/blob/main/img/IMG_4372.JPG" width="30%"> <img src="https://github.com/AiratNig/TinyVFDClock/blob/main/img/IMG_4374.JPG" width="30%"> <img src="https://github.com/AiratNig/TinyVFDClock/blob/main/img/IMG_4373.JPG" width="30%">

Список элементов:
|ID|Name|Designator|Footprint|Quantity|
|--|----|----------|---------|--------|
|1|0.1u|C1, C2, C5, C6, C8 `*`, C9 `*`, C13, C16, C17, C18, C19, C20, C25|SMD 0603|13|
|2|100u|C3, C4|SMD CASE B|2|
|3|0.22u 50V|C7|SMD 0805|1|
|4|1u 50V|C10, C15|SMD 0805|2|
|5|10u 35V|C11, C12|SMD CASE C|2|
|6|0.01u|C14|SMD 0603|1|
|7|10u|C21, C22|SMD CASE A|2|
|8|20|C23, C24|SMD 0603|2|
|9|BAV99|D1|SOT-23-3|1|
|10|BZV55C5V1|D2|SOD80|1|
|11|LT1617|DA1|SOT-23-5|1|
|12|LM9022M|DA2|SO8|1|
|13|ATTINY44A-SSUR|DD1|SOP-14|1|
|14|PT6313S|DD2|SOP-28|1|
|15|DS3231MZ+|DD3|SO8|1|
|16|DS1339AU+ `*`|DD4|MSOP-8|1|
|17|ASMD0805-100|F1|SMD 0805|1|
|18|Keystone 3001|G1| |1|
|19|IV-12|HG1, HG2, HG3, HG4| |4|
|20|IV-15|HG5| |1|
|21|WS2812D-F5|HL1, HL2, HL3, HL4| |4|
|22|SPM4020T-100M-LR|L1| |1|
|23|10k|R1, R9, R10, R12, R13, R14, R17, R18, R19, R20, R24, R27, R28|SMD 0603|13|
|24|68k|R2|SMD 0603|1|
|25|10|R3, R4, R29, R30|SMD 1210|4|
|26|47|R5|SMD 1210|1|
|27|39|R6|SMD 1210|1|
|28|560k|R7|SMD 0603|1|
|29|24k|R8|SMD 0603|1|
|30|2.2k|R11|SMD 0603|1|
|31|200|R15, R16|SMD 0603|2|
|32|100|R21, R22, R23, R26|SMD 0603|4|
|33|GL5528|R25| |1|
|34|TS-1145A-C-B|SB1, SB2, SB3| |3|
|35|U-F-M5DD-Y-L|X1| |1|
|36|SM04B-SRSS-TB|X2| |1|
|37|32.768KHz `*`|ZQ1| |1|
|38|16MHz|ZQ2|SMD 3225|1|

 `*` - Данные элементы устанавливаются для часов реального времени DS1339AU+.

Фьюзы ATtiny44: low: `0xFF`, high: `0xDF`, extended: `0xFF`
Проект для Atmel Studio 7 в папке firmware/VFDClockTiny44_src.zip, там же две собранные прошивки для RTC DS3231M и DS1339.
Датчик температуры - LM75, адрес датчика - `0x4F`.

Настройка часов: нажатием кнопки `MENU` выбирается необходимый пункт.
`HR` - установка часов, 
`MN` - установка минут, 
`SC` - установка секунд, 
`BL` - установка подсветки,  
`LS` - вкл/выкл датчика освещенности, 
`ST` - вкл/выкл показа температуры, 
`ES` - выход. 
Кнопками `UP`/`DOWN` выставляются необходимые значения.


