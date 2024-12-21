3.1

1. В задании [FootballTeam](https://github.com/deionnle/Survivor/blob/main/FootballTeam.java#L9) добавил комментарий `
// Проверяем возможность упорядочить массив, поменяв местами два элемента`
к циклу `for (int i = 0; i < N - 1; i ++)`. На мой взгляд комментарий уместен, т.к. теперь не требуется вникать
для чего нужен этот цикл. Конечно, правильнее было сделать функцию.

2. В задании [FootballTeam](https://github.com/deionnle/Survivor/blob/main/FootballTeam.java#L20) добавил комментарий
`// Проверяем возможность упорядочить массив, изменив порядок последовательной цепочки`
к циклу `for (int i = 0; i < N - 2; i ++)`. По сути комментариями обозначена логика работы циклов.

3. В задании [Matrix](https://github.com/deionnle/Survivor/blob/main/Matrix.java#L17) добавил комментарий
`// Если разность уже встречалась, проверяем длину подстроки`
перед условием ` if (StorageOfDifference.containsKey(difference) && i - StorageOfDifference.get(difference) > endIndexOfSubstr - 1) `
Это позволяет намного быстрее понять условие.

4. В задании [MissionImposible](https://github.com/deionnle/Survivor/blob/main/MissionImpossible.java#L25)
комментарием `// Разбиваем строку на подстроки длиной m и добавляем в список`
объясняю логику работы цикла `for (int i = 0; i < n; i++)`. Опять же этого комментария можно было бы избежать, вынеся
логику в отдельную функцию.

5. В задании [MissionImposible](https://github.com/deionnle/Survivor/blob/main/MissionImpossible.java#L35)
комментарием `// Формируем зашифрованный текст, перебирая столбцы`
объясняю логику работы цикла ` for (int i = 0; i < list.get(0).length(); i ++)`.

6. В задании [SalesReport](https://github.com/deionnle/Survivor/blob/main/SalesReport.java#L8)
при помощи комментария 
`// Создаём HashMap для хранения общего количества продаж каждого товара`
объясняю логику работы цикла `for (int i = 0; i < N; i ++)`.

7. В задании [Paratroopers](https://github.com/deionnle/Survivor/blob/main/Paratroopers.java#L5)
комментарием `// Установка начальных позиций высадки десантников`
объясняю логику работы цикла `for (int i = 0; i < L * 2 - 1; i += 2)` 

3.2

В задании `Dictionary` курса "с нуля" я писал комментарий к каждой строчке кода, например:
` // Цикл по элементам списка` `list for (Integer i : list)` или
`// Создаю словарь` `HashMap<Integer, String> NumbersList = new HashMap<>();`
Конечно, так делать нельзя, но в тот момент это было необходимо для понимания.

Удалил 11 комментариев и сделал код более наглядным: [Dictionary](https://github.com/deionnle/Test/blob/main/Dictionary.java)




