# Anagram Detection

### What we must do?
An anagram is the result of rearranging the letters of a word to produce a new word (see wikipedia).

Note: anagrams are case insensitive

Complete the function to return true if the two arguments given are anagrams of each other; return false otherwise.

Examples
```
"foefet" is an anagram of "toffee"
"Buckethead" is an anagram of "DeathCubeK"
```
### What we did?
1. Преобразовали строчки в нижний регистр для того, что бы не было не совпадений, из-за наличия верхнего регистра.
2. Создали переменную, которую в будущем будем использовать как счётчик совпадений.
3. Разбили наши строки на символы и сохранили эти символы в массивах.
4. Делаем проверку на равность количества символов в данных нам строках через оператор "ЕСЛИ". Если количество разное - возвращаем false. Если количество символов совпадает - идём дальше.
5. Делаем цикл, который будет проверять совпадение символов. <br/>
(Параметры: <br/>
        1. Мы создали переменную, которая с каждым кругом будет увеличивается и тем самым менять элемент в массиве, у которого мы запрашиваем нужный нам символ на сравнение со строкой;<br/>
        2. Цикл будет действовать пока переменная, которую мы создали ранее для изменения элемента в массиве, меньше чем длина данной нам строки)
6. Мы создали оператор "ЕСЛИ" с таким условие, что если в строке используется символ, находящийся в массиве (который в свою очередь меняет этот символ с каждым кругом), то мы в нашу переменную, которую используем как счетчик совпадений, добавляем 1.
7. Мы создаем еще один оператор "ЕСЛИ" вне наших 2х таких же операторов. Он проверяет, если количество символов данной нам строки равняется количеству счётчика совпадении, то мы возвращаем true; В противном случаи - возвращаем false.
