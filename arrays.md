1. В задании [KeyMaster](https://github.com/deionnle/Survivor/blob/main/KeyMaster.java#L18)
изменил цикл `for` который собирает результат в строку
на `for-each` так как он просто перебирает элементы массива и 
добавляет их в `StringBuilder`.


2. В задании [SumNumbers](https://github.com/deionnle/Survivor/blob/main/SumNumbers.java#L11) при помощи цикла `for-each`
ушел от прямой индексации массива `int[] data`


3. В задании [SavePrinterToner](https://github.com/deionnle/Survivor/blob/main/SavePrinterToner.java#L43) использовал словарь место двух массивов.
Изменил цикл `for` на `for-each` при работе со словарем, упростил логику и избавился от вложенного цикла.


4. В задании [SearchWord](https://github.com/deionnle/Survivor/blob/main/SearchWord.java#L36) вместо массива `int[] res` можно было бы использовать список `List<Integer>`
Это позволило бы не указывать заранее размер массива, и добавлять элементы динамически.
Не стал переделывать код, т.к. пришлось бы изменить сам тип данных, возвращаемый методом `WordSearch`
и уйти от условия задачи.


5. В задании [Hogwarts](https://github.com/deionnle/Survivor/blob/main/Hogwarts.java#L7)
можно было бы использовать вместо массива `char[] ch` список `List<Character`.
