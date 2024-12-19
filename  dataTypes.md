1. Заменил магические символы `````' * ' и ' . '````` на константы ```STAR``` и `DOT` в задании [PatternAnalysis](https://github.com/deionnle/Survivor/blob/main/PatternAnalysis.java#L3)

2. В задании [SavePrinterToner](https://github.com/deionnle/Survivor/blob/main/SavePrinterToner.java#L5) заменил магическое число `23`
на константу `COSTS_FOR_UNKNOWN_SYMBOL = 23;`

3. В задании [WhiteWalkers](https://github.com/deionnle/Survivor/blob/main/WhiteWalkers.java#L4)
вместо магических чисел добавлены константы `TARGET_SUM = 10` и `REQUIRED_EQUALS = 3.`
   
4. [WhiteWalkers](https://github.com/deionnle/Survivor/blob/main/WhiteWalkers.java#L13) 
Вместо магических чисел `48` и `57` используется `Character.isDigit.`

5. Вместо `Character.toString()` в `Integer.parseInt()` использовал `Character.getNumericValue` для получения численного значения символа [WhiteWalkers](https://github.com/deionnle/Survivor/blob/main/WhiteWalkers.java#L23)

6. Добавил проверку `if (totalNumbersOfVotes == 0)` для предупреждения ошибки деления на ноль в задании [Voting](https://github.com/deionnle/Survivor/blob/main/Voting.java#L10)

7. В задании [MissionImpossible](https://github.com/deionnle/Survivor/blob/main/MissionImpossible.java#L15)
заменил сравнение на равенство вещественного числа `(sq % n == 0)` на сравнение с погрешностью `(Math.abs(sq - n) < EPSILON)`
создав при этом константу `double EPSILON = 1e-9`

8. Добавил константы  `String SPACE = " "` и  `String NO_SPACE = ""` вместо магических строк [MissionImpossible](https://github.com/deionnle/Survivor/blob/main/MissionImpossible.java#L15)

9. Добавил логическую переменную `isSubstring = s1.length() < m && s1.length() > 0` для улучшения читаемости условия
   [MissionImpossible](https://github.com/deionnle/Survivor/blob/main/MissionImpossible.java#L28)

10. В функции вычисления факториала изменил целочисленный тип `int` на `long` [Hogwarts](https://github.com/deionnle/Survivor/blob/main/Hogwarts.java#L80)

11. Магическая строка заменена на константу `DEFAULT_RESULT = "0 0 2"` в [Cyberpunk1995](https://github.com/deionnle/Survivor/blob/main/Cyberpunk1995.java#L3)

12. Для улучшения читаемости добавил логическую переменную `isFirstIteration = (x == 0 && y == 0 && m == 2)` в [Cyberpunk1995](https://github.com/deionnle/Survivor/blob/main/Cyberpunk1995.java#L25)