Касательно пункта *1. Минимизируйте область видимости каждой переменной* - мне не
удалось найти ситуаций в коде, когда область видимости переменной можно уменьшить.

Поэтому я сделал упор на п.2 и постарался минимизировать окна уязвимости переменных, сгруппировать операции и вынести логики в отдельные функции.

1.  Для переменной `candidateVotingResult` логику расчета результатов голосования для каждого кандидата
вынес в отдельный метод [calculateVotingResults](https://github.com/deionnle/Survivor/blob/main/Voting.java#L25)

2. Для переменной `candidateVotingResult` логику поиска победителя вынес в отдельную функцию
[findWinner](https://github.com/deionnle/Survivor/blob/main/Voting.java#L34)

3. В результате изменений ограничил область видимости переменных
`count` и `winnerIndex` (бывш n и K). методом [findWinner](https://github.com/deionnle/Survivor/blob/main/Voting.java#L34)

4. В результате изменений ограничил область видимости переменной `resultValueMax`
функциями [findWinner](https://github.com/deionnle/Survivor/blob/main/Voting.java#L34) и
[getVictoryType](https://github.com/deionnle/Survivor/blob/main/Voting.java#L46)

5. В результате изменений ограничил область видимости переменной `totalNumbersOfVotes` методом
[calculateVotingResult](https://github.com/deionnle/Survivor/blob/main/Voting.java#L25)

6. В задании [UFOSignal](https://github.com/deionnle/Survivor/blob/main/UFOSignal.java) 
ограничил область видимости констант `OCTAL_SYSTEM = 8` и `HEXADECIMAL_SYSTEM = 16` вынеся их в отдельный метод
[getCurrentSystem](https://github.com/deionnle/Survivor/blob/main/UFOSignal.java#L11)

7. Область видимости переменной `currentSystem` ограничил функцией
[convertToDecimal](https://github.com/deionnle/Survivor/blob/main/UFOSignal.java#L17)

8. В задании [SumNumbers](https://github.com/deionnle/Survivor/blob/main/SumNumbers.java)
сгруппировал операции над переменной `total` в отдельную функцию
[findMatchingElement](https://github.com/deionnle/Survivor/blob/main/SumNumbers.java#L10)
 Также это позволило упростить переменную `res`

9. В задании [Squirrel](https://github.com/deionnle/Survivor/blob/main/Squirrel.java)
добавил метод вычисления факториала [calculateFactorial](https://github.com/deionnle/Survivor/blob/main/Squirrel.java#L7) что позволило уменьшить окно уязвимости
переменной `factorial`

10. Также уменьшил окно уязвимости переменной `factorial` переместив логику извлечения первой цифры
в функцию [extractFirstDigit](https://github.com/deionnle/Survivor/blob/main/Squirrel.java#L15)

11. В задании [SherlockHolmes](https://github.com/deionnle/Survivor/blob/main/SherlockHolmes.java) 
реализовал метод [buildFrequencyMap](https://github.com/deionnle/Survivor/blob/main/SherlockHolmes.java#L19)
который собирает частоты символов в строке. Это сокращает количество 
повторяющихся операций с `countMap` в основном методе.

12. Метод [checkEqualFrequency](https://github.com/deionnle/Survivor/blob/main/SherlockHolmes.java#L28) проверяющий, равны ли все значения в 
`countMap` также позволил уменьшить ее окно уязвимости.

13. Уменьшил область видимости переменной `delValue` переместив ее в метод
[checkEqualFrequency](https://github.com/deionnle/Survivor/blob/main/SherlockHolmes.java#L41) 

14. Переменные `ch` и `val` в методе [checkAfterRemoval](https://github.com/deionnle/Survivor/blob/main/SherlockHolmes.java#L42) ограничены только этим методом 
и создаются непосредственно перед изменением значений в `delValue`,
что уменьшает окно их уязвимости

15. Область переменной `firstValue` ограничена только методом [checkEqualFrequency](https://github.com/deionnle/Survivor/blob/main/SherlockHolmes.java#L28)
и она используется лишь для одной операции проверки частоты.