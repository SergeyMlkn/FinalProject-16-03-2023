Итоговая проверочная работа

Задача: Написать программу, которая из имеющегося массива строк формирует новый массив из строк, длина которых меньше, либо равна 3 символам. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.

Примеры: 
[“Hello”, “2”, “world”, “:-)”] → [“2”, “:-)”] 
[“1234”, “1567”, “-2”, “computer science”] → [“-2”] 
[“Russia”, “Denmark”, “Kazan”] → []

Описание решения: 
Pадан массив строк array string[] array = { "[“Hello”, “2”, “world”, “:-)”]}; 
Создаем массив result, в который будем записывать строки из массива array, длина которых меньше, либо равна 3 символам. 
Размер массива result принимаем равным размеру array. строка[] результат = новая строка[массив.Длина]; 
С помощью цикла проверяем следующие условия if (array[i].Length <= 3) result[i] = array[i]; else result[i] = string.Empty; if (result[i] != string.Empty) Console.Write($"{result[i]} "); 
Если длина строки массива array меньше, либо равна 3 символам, то записываем данную строку в массив result. 
Иначе записываем в массив result пустую строку (string.Пусто). 
Если строка массива result не является пустой, то выводим ее на экран. 
Результат выполнения программы выглядит следующим образом: [“2”, “:-)”]