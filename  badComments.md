***1. Неочевидные комментарии***

Комментарий `// Инициализация живых и мёртвых ветвей дерева`
неочевидный, т.к. непонятно, почему используются символы `+` и `.`
На мой взгляд нужно улучшить описание констант 
`Символы для обозначения живых (+) и мёртвых (.) ветвей дерева` 
[TreeofLifeAndrassil](https://github.com/deionnle/Survivor/blob/main/TreeofLifeAndrassil.java#L5)

Комментарий `// Меняю цвет каждого пикселя на красный`
может оказаться неочевидным, если позже цвет будет изменен.
Улучшение - комментарий удален.
[Image](https://github.com/deionnle/Test/blob/main/Image.java)

***2. Бормотание***

Комментарий `// Удаляем старые ветви дерева`
не помогает в понимании кода. Гораздо лучше придумать хорошее
название метода.
Улучшение - метод `delMatrix` переименовал в `removeDeadBranches`
[TreeofLifeAndrassil](https://github.com/deionnle/Survivor/blob/main/TreeofLifeAndrassil.java#L66)

***3. Недостоверные комментарии***

Комментарий `// Проверка высоты дерева.`
На самом деле это проверка длины массива, а не высоты дерева
Улучшил: `Проверка соответствия количества строк дерева заданной высоте H"`
[TreeofLifeAndrassil](https://github.com/deionnle/Survivor/blob/main/TreeofLifeAndrassil.java#L11)

Комментарий `// Проверка ширины дерева.`
На самом деле это ширина строк, а не дерева.
Улучшил: `Проверка, что каждая строка дерева имеет длину W`
[TreeofLifeAndrassil](https://github.com/deionnle/Survivor/blob/main/TreeofLifeAndrassil.java#L15)

***4. Шум***

Комментарий `// Удаляем ветви по координатам` и `// Удаляем соседние ветви`
лишь утверждают очевидное, не предоставляя никакой новой информации.
Улучшение - комментарии удалены. А так же было бы не плохо вынести логику в отдельный метод.
[TreeofLifeAndrassil](https://github.com/deionnle/Survivor/blob/main/TreeofLifeAndrassil.java)

Комментарии `// Запускаем обновления дерева` и
`// Если нечётный цикл, удаляем старые ветви` обозначают очевидное
Улучшение - изменил комментарий перед циклом на `Обновляем состояние дерева в N циклах роста и удаления`
но также в качестве улучшения можно вынести в отдельную функцию.
[TreeofLifeAndrassil](https://github.com/deionnle/Survivor/blob/main/TreeofLifeAndrassil.java#L34)

Комментарий `// Добавляем строку в результирующий массив`
слишком очевиден.
Улучшение - комментарий удален.
[TreeofLifeAndrassil](https://github.com/deionnle/Survivor/blob/main/TreeofLifeAndrassil.java)

Комментарий `// Цикл по всем файлам` для цикла `for (File file : files)`
описывает очевидное.
Улучшение - комментарий удален.
[Image](https://github.com/deionnle/Test/blob/main/Image.java)

Комментарий `// Если список файлов не пустой` для условия `if (files != null)`
повторяет смысл условия.
Улучшение - комментарий удален.
[Image](https://github.com/deionnle/Test/blob/main/Image.java)

***7. Избыточные комментарии***

Комментарий `// Заполняем массив: живая ветвь —  1, мертвая — 0`
избыточен. Это и так понятно после появления константы `DEAD_BRANCH` в цикле.
Улучшение - комментарий удален.
[TreeofLifeAndrassil](https://github.com/deionnle/Survivor/blob/main/TreeofLifeAndrassil.java)

Комментарий `// Преобразуем матрицу обратно в строковый массив`
избыточен. И так очевидно что происходит преобразование.
Улучшение - комментарий удален.
[TreeofLifeAndrassil](https://github.com/deionnle/Survivor/blob/main/TreeofLifeAndrassil.java)

Комментарий `// Увеличиваем возраст каждой ветки дерева`
избыточен. Намного лучше придумать хорошее имя для метода.
Улучшение - метод `getMatrix` переименовал в `updateBranchAge`.
[TreeofLifeAndrassil](https://github.com/deionnle/Survivor/blob/main/TreeofLifeAndrassil.java#L57)

Комментарий `// Задаю цвет и добавляю текст` для метода `g.setColor(Color.black);`избыточен
Улучшение - комментарий удален.
[Image](https://github.com/deionnle/Test/blob/main/Image.java#L25)

***12. Не используйте комментарии там, где можно использовать функцию или переменную***

Комментарий `// Меняю цвет каждого пикселя на красный` для цикла `for (int x = 0; x < img.getWidth(); x++) ...`
не нужен. Лучше перенести код в отдельную функцию `paintImageRed`
[Image](https://github.com/deionnle/Test/blob/main/Image.java#L16)