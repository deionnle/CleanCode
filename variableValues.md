1. В задании [MaxDiscount](https://github.com/deionnle/Survivor/blob/main/MaxDiscount.java#L7) перенес переменную `discount` непосредственно к циклу.

2. Переименовал и перенес переменную `daysPassed` непосредственно к циклу [Paratroopers](https://github.com/deionnle/Survivor/blob/main/Paratroopers.java#L11)

3. В задании [PhoneUnlock](https://github.com/deionnle/Survivor/blob/main/PhoneUnlock.java#L4) изменил имя переменной(акумулятора) с `sum` на `unlockLineLength`, упростил переменную `String
res` перед `return`, т.к. в ней не было необходимости.

4. Добавил утверждение для проверки корректности входных данных: выбрасывается исключение если истинно: ``if (track == null || track.length != N)``
[TrafficOptimization](https://github.com/deionnle/Survivor/blob/main/TrafficOptimization.java#L4)

5. Добавил утверждение для проверки корректности значений в массиве: исключение если истинно условие: `if (redTrafficLightTime <= 0 || greenTrafficLightTime <= 0)`
   [TrafficOptimization](https://github.com/deionnle/Survivor/blob/main/TrafficOptimization.java#L22)

6. После завершения работы с переменными `redTrafficLightTime` и `greenTrafficLightTime` присвоил им значения `-1`
   [TrafficOptimization](https://github.com/deionnle/Survivor/blob/main/TrafficOptimization.java#L43)

7. В задании [TreeofLifeAndrassil.java](https://github.com/deionnle/Survivor/blob/main/TreeofLifeAndrassil.java#L10)
добавил утверждения для проверки корректности входных данных (размера матрицы)
   `if (tree.length != H) и if (row.length() != W)`

8. В задаче [Cyberpunk1991](https://github.com/deionnle/Survivor/blob/main/Cyberpunk1991.java#L3) 
добавил проверку на корректность входных данных  `if (arr == null || arr.length == 0)`

9. Аналогично, добавил проверку входных данных `if (activate == null || activate.length == 0)`
[Cyberpunk1992](https://github.com/deionnle/Survivor/blob/main/Cyberpunk1992.java#L5)

10. Изменил имя переменной `res` на `summaryLine` и перенес непосредственно к месту использования [MissionImpossible](https://github.com/deionnle/Survivor/blob/main/MissionImpossible.java#L22)

11. Перенес инициализацию переменной `currentValue`(бывш. val) непосредственно в цикл `while`, т.к. за пределами цикла
она не используется [MrRobot](https://github.com/deionnle/Survivor/blob/main/MissionImpossible.java#L22)

12. Убрал избыточную инициализацию переменных `max = 0` и `premax = 0` т.к. значения переменным присваиваются в цикле. Задача [Recursion4](https://github.com/deionnle/Survivor/blob/main/Recursion4.java#L6)

13. Добавил проверку корректности входных данных  `if (ids == null || salary == null || ids.length != salary.length || N <= 0)` [SalaryTable](https://github.com/deionnle/Survivor/blob/main/SalaryTable.java#L6)

14. В задании [Mileage](https://github.com/deionnle/Survivor/blob/main/Mileage.java#L3) добавил проверку корректности входных данных
    `if (oksana == null || oksana.length == 0)` а также корректности показаний скорости `if (oksana[speed] < 0)`

15. В задании [MadMax](https://github.com/deionnle/Survivor/blob/main/MadMax.java#L5) добавил проверку корректности входных данных
    `if (Tele == null || Tele.length != N || (N < 1 || N > 127) || N % 2 == 0)`

16. В задании [SalesReport](https://github.com/deionnle/Survivor/blob/main/SalesReport.java)
    упростил временную переменную ```String str = items[i];``` добавил проверку на
    инварианты для [входных данных](https://github.com/deionnle/Survivor/blob/main/SalesReport.java#L5) `if (N < 1 || items == null || items.length != N)` и [выходных](https://github.com/deionnle/Survivor/blob/main/SalesReport.java#L45) `if (salesSummary.length > N)`