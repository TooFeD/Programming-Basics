# Клас - Автомобіль

### Параметри: 
+ наявність коліс;
+ кузов;
+ двигун;
+ руль.
---
*Об'єкти класу "Автомобіль":*
1. Легковий автомобіль
2. Вантажний автомобіль
---
*Наслідування*
1. Легковий автомобіль: 
    + седан;
    + хеджбек;
    + універсал;	
    * механічна коробка передач(кп); 
    * автоматична кп;

2. Вантажний автомобіль: 
    * Газон; 
    * Камаз; 
    * Фура.
---
*Поліморфізм*
1. У автомобіля руль може бути справа чи зліва, але функція його не зміниться, якщо повернути вправо, то і автомобіль поверне вправо.
2. Механічна коробка передач може мати різну кількість положень (4-ступеньчата, 5-ступеньчата ...)
---
*Інкапсуляція*
1. Людина не повинна знати як працює двигун, щоб керувати автомобілем, вона має свій інтерфейс для цього.
---

## SOLID:
1. S - руль повинен визначати напрям руху автомобіля, КП - перемикати передачі, педаль тормоза - тормозити.

2. O - додати ГБО на авто, встановити сигналізацію, додати склопідіймачі.

3. L - для того щоб дістатися з пункта А у пункт В можна використати будь-який автомобіль, для перевезення багажу можна застосувати будь-яке авто.

4. I - для керування автомобілем виведено в окремий інтерфейс - руль, педалі(зчеплення, тормоз, газ), для перепрошивки чи діагностики автомобіля виділено окремий спец-інтерфейс.

5. D - **автомобіль** - це **транспортний засіб(ТЗ)**, який виконує функцію "Їздити" і не важливо, що це за ТЗ велосипед, автомобіль, скейт.