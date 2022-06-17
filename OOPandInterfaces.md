**Задание 3.1:**
*За свой код принял решения 28 задач и как-бы это могло выглядеть*

MadMax - добавим поле телеметрической последовательности в виде целочисленного массива, тогда можно сделать два конструктора-фабрики:
MadMax madmax = new MadMax.getStartImpulseFromNums(); // как в оригинале
MadMax madmax = new MadMax.getStartImpulseFromString("5 6 10 12 3 9"); // метод преобразует строку в целочисленный массив


PatternUnlock - добавим поле последовательности в виде целочисленного массива, тогда можно сделать два конструктора-фабрики:
PatternUnlock pattern = new PatternUnlock.getHackSequenceFromNums() // как в оригинале - массив чисел
PatternUnlock pattern = new PatternUnlock.getHackSequenceFromString("1234562789") // метод преобразует строку в целочисленный массив

Keymaker - добавим поле для кол-ва дверей и преобразований, тогда можно сделать три конструктора-фабрики:
Keymaker currentState = new Keymaker.doorsStatementFromInt(); // на вход подаем целое число, как в оригинале
Keymaker currentState = new Keymaker.doorsStatementFromReal(); // округляем вход до целого числа
Keymaker currentState = new Keymaker.doorsStatementFromString(); // преобразуем строку в целое число

**Задание 3.2:**
*Для реализации классической игры FizzBuzz без условных операторов я как раз использовал интерфейс и его реализации (вот уж не думал что пригодится мой код):
PrintFactory - интерфейс // фабрика печати

Реализации интерфейсов:
DivBy3Print - реализация когда число делится только на 3
DivBy5Print - реализация когда число делится только на 5
DivBy3And5Print - реализация когда число делится только и на 3 и на 5
NotDivPrint - реализация когда число не делится ни 3 ни на 5

Код самой игры находится [здесь](https://github.com/Starbreaker84/Ideas/blob/main/FizzBuzz/FizzBuzzWithoutConditions.java). 
