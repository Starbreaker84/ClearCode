**Задание 3.1:**<br/>
етод ConquestCampaign.<br/>
```
//высадка десанта с захватом начальных точек
if (i % 2 != 0) battlefield[battalion[i - 1] - 1][battalion[i] - 1] = 1;
```

- метод ShopOLAP.<br/>
```
//возвращаем массив неповторяющихся проданных товаров
String mergedItems = Arrays.stream(items)
    .filter(string -> !string.equals(""))
    .collect(Collectors.joining("-"));
return mergedItems.split("-");
```

- метод LineAnalysis.<br/>
```
//интервал завершился и не соответствует паттерну
boolean isNotPattern = line.charAt(i) == '*' && !lineForAnalyse.toString().equals(pattern);
```

- метод Football<br/>
```
//можно ли улучшить расстановку игроков?
if (!sorted) return way1(F, N, indexForSwap) || way2(F, N, indexForSwap);
```

- метод TransformTransform.<br/>
```
//дважды трансформируем массив 
int[] S = transform(transform(A, N), transform(A, N).length);
```

- метод ConquestCampaign.<br/>
```
//размечаем клетки для завоевания
for (int j = 0; j < M; j++) {
    boolean isConquered = battlefield[i][j] == 1;
    if (isConquered) {
        if ((i - 1) >= 0 && battlefield[i - 1][j] == 0) battlefield[i - 1][j] = 2;
        if ((i + 1) < N && battlefield[i + 1][j] == 0) battlefield[i + 1][j] = 2;
        if ((j - 1) >= 0 && battlefield[i][j - 1] == 0) battlefield[i][j - 1] = 2;
        if ((j + 1) < M && battlefield[i][j + 1] == 0) battlefield[i][j + 1] = 2;
    }
}
```

- метод UFO.<br/>
```
//поразрядно переводим число из одной системы в другую
for (int i = 0; i < currentDigitIndex; i++) {
    convertedData += Character.getNumericValue(stringOfNumbers.charAt(i)) * pow(radix, currentDigitIndex - i);
}
```

**Задание 3.2:**
- в методе PrintingCosts убрал комментарий `//проверяем есть ли символ в таблице и находим его индекс` перед циклом поиска символа, заменил сам цикл и проверку на символ, которого нет в таблице:
```
int indexOfCharInTable = characterTable.indexOf(Line.charAt(i));
totalPrintingCost += indexOfCharInTable < 0 ? DEFAULT_COST : characterPrintingCosts[indexOfCharInTable];
```

- в методе Unmanned убрал комментарий `//цикл работы светофора` так как после переименования переменных надобность в нём отпала и код стал выглядеть так: `int trafficLightCycle = greenLightTime + redLightTime;`

- в методе PatternUnlock убрал комментарий `//проверяем, является ли линия диагональю` перед условным оператором, после переименования переменных надобность в нём отпала, а код теперь выглядит так:
```
boolean isDiagonal = (sumOfBesideDigits == 6 || sumOfBesideDigits == 8) || ((sumOfBesideDigits == 9 || sumOfBesideDigits == 11) && (hits[i] >= 7 || hits[i - 1] >= 7));
if (isDiagonal) {
...
```

- в методе ConquestCampaign убрал комметарий `//проверяем, завоёвана ли область` перед условным оператором, после добавления логической переменной надобность отпала, код выглядит так:
```
boolean isConquered = battlefield[i][j] == 1;
if (isConquered) {
...
```

- в методе TheRabbitsFoot изначально я всю программу записал в одном методе, и перед кодированием и декодированием стояли соответствующие комментарии. После того как добваил два закрытых метода (первый на кодировку и второй на расшифровку) да сделал читаемыми все переменные, надобность в комментариях отпала.
