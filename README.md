# st-examples
Tasks for trainees

## Как данные хранятся в RAM?

RAM можно представить как большое количество ячеек, каждая из которых имеет свой номер (адрес) и может хранить небольшую единицу данных (байт). Эти ячейки последовательно пронумерованы.

- **Пример**: Представь, что у тебя есть длинная лента с ячейками, каждая из которых подписана цифрами 0, 1, 2, 3, 4 и так далее. В каждую ячейку ты можешь положить бумажку с одной цифрой или буквой.

## 3. Как хранятся строки в памяти?

**Строка** — это последовательность символов. Компьютер хранит каждый символ как набор чисел (обычно по стандарту **ASCII**). Например, символ 'A' в памяти будет представлен числом 65, а 'B' — 66.

- **Пример хранения строки**:
  Допустим, у нас есть строка "HELLO". В памяти это будет выглядеть так:
```yaml
Адрес:  | 1000 | 1001 | 1002 | 1003 | 1004 | 1005 |
Данные: | 'H'  | 'E'  | 'L'  | 'L'  | 'O'  | '\0' |
ASCII:  | 72   | 69   | 76   | 76   |  79  | 0 |


```

Здесь каждый символ хранится в отдельной ячейке, а специальный символ `\0` обозначает конец строки.

- **Пример**: Если ты пишешь текстовое сообщение, то каждая буква или символ хранится в RAM в виде последовательности чисел, а когда текст отправляется или сохраняется, компьютер знает, что строка заканчивается на `\0`.

### ASCII-коды некоторых часто используемых символов:
```yaml
Символ: | 'A' | 'B' | 'C' | 'D' | 'E' | 'F' | 'G' | 'H' | 
ASCII:  | 65  | 66  | 67  | 68  | 69  | 70  | 71  | 72  |

Символ: | 'I' | 'J' | 'K' | 'L' | 'M' | 'N' | 'O' | 'P' |
ASCII:  | 73  | 74  | 75  | 76  | 77  | 78  | 79  | 80  |

Символ: | 'Q' | 'R' | 'S' | 'T' | 'U' | 'V' | 'W' | 'X' |
ASCII:  | 81  | 82  | 83  | 84  | 85  | 86  | 87  | 88  |


Символ: | 'Y' | 'Z' | 'a' | 'b' | 'c' | 'd' | 'e' | 'f' |
ASCII:  | 89  | 90  | 97  | 98  | 99  | 100 | 101 | 102 |

Символ: | 'g' | 'h' | 'i' | 'j' | 'k' | 'l' | 'm' | 'n' |
ASCII:  | 103 | 104 | 105 | 106 | 107 | 108 | 109 | 110 |

Символ: | 'o' | 'p' | 'q' | 'r' | 's' | 't' | 'u' | 'v' |
ASCII:  | 111 | 112 | 113 | 114 | 115 | 116 | 117 | 118 |

Символ: | 'w' | 'x' | 'y' | 'z' | ' ' (space) | '\0' (null) |
ASCII:  | 119 | 120 | 121 | 122 | 32          | 0           |
```
## Как хранятся массивы в памяти?


**Массив** — это последовательность одинаковых элементов (чисел, символов и т. д.), которые хранятся в памяти один за другим.

- **Пример хранения массива**:
Если у нас есть массив чисел:

```cpp
int arr[5] = {10, 20, 30, 40, 50};
```
```yaml
Адрес:  | 2000 | 2004 | 2008 | 2012 | 2016 |
Данные: |  10  |  20  |  30  |  40  |  50  |
```
Каждый элемент массива занимает несколько ячеек (в данном случае 4 байта, потому что это тип данных int, который занимает 4 байта).

### Strings in C
![string in C](https://simplesnippets.tech/wp-content/uploads/2018/03/c-c-style-strings.jpg)

### Containers
![container structure](https://www.educative.io/api/edpresso/shot/6445167638740992/image/6388045848772608)


# Control Flow


### IF
```
if (condition) 
 
   # statements to be executed 
 
end
```
![if block](https://media.geeksforgeeks.org/wp-content/uploads/rubyif-statement.png)
![if](https://github.com/ErrorSoul/st-examples/blob/5dbd7b40cb595a202dd2653f1b0b443864dc5a3b/if.png)

### IF/ELSE
```
if(condition)  

    # code if the condition is true  

else  

   # code if the condition is false  
end 
```
![if/else block](https://media.geeksforgeeks.org/wp-content/uploads/if-else-statementruby.jpg)
![if/else code](https://github.com/ErrorSoul/st-examples/blob/936c69b786b2abf47b1853fbf2ed18049b3362eb/if_else.png)


### IF/ELSIF/ELSE

```
if(condition1)  

# code to be executed if condition1is true
  
elsif(condition2)
  
# code to be executed if condition2 is true  

else(condition3)  

# code to be executed if condition3 is true  
end  
```

![if/else/elsif block](https://media.geeksforgeeks.org/wp-content/uploads/if-else-if-statementruby.jpg)
![if/else/elsif code](https://github.com/ErrorSoul/st-examples/blob/032d0e04ba1ed10541157f9866d2b1e79ab63b0e/if_elsif_else.png)

### Case

```
case expression

when expression 1
  # your code

when expression 2
  # your code
.
.

else
  # your code
end
```

![case block](https://media.geeksforgeeks.org/wp-content/uploads/ruby-case.jpg)
![case code](https://github.com/ErrorSoul/st-examples/blob/326cb65df098543ae9b8ba31332ac2ced7f443a8/%D1%81ase.png)

### While

```
while conditional [do]

 # code to be executed

end
```

![while](https://media.geeksforgeeks.org/wp-content/uploads/rubyWhile-loop.jpg)
![while](https://github.com/ErrorSoul/st-examples/blob/ea27644624fccf3c25e949fe7f9afecfa59d34c3/while.png)

#### Output
```
Foo
Foo
Foo
Foo
```


### for c in 

```
for variable_name[, variable...] in expression [do]

   # code to be executed

end
```

![for c in ](https://github.com/ErrorSoul/st-examples/blob/637cf2d729f91d2caba745e996f7af71a8abbb44/forin.png)

#### Output
```
GFG
G4G
Geeks
Sudo
```

### loop

```
loop do

 # code to be executed

break if Boolean_Expression

end
```

![loop](https://github.com/ErrorSoul/st-examples/blob/9fc3aa5b2bb89a3fb908bcd0ef3d8445fa1034fe/loop.png)


#### Output
```
GeeksforGeeks
```

### until

```
until conditional [do]

 # code to be executed

end
```

![until](https://github.com/ErrorSoul/st-examples/blob/9fc3aa5b2bb89a3fb908bcd0ef3d8445fa1034fe/until.png)


#### Output
```
70
80
90
100
```

### each

```
arr.each do |elem|

 # code to be executed 

end
```

![each](https://github.com/ErrorSoul/st-examples/blob/2933336dcf611fdfd0b94919864a39c9c272443f/each.png)


#### Output
```
1
2
3
4
5
```
# Задачи

1) Вывести числа от 1 до 10 (все делать через while, until, for c in range, each)
2) На вход дается строка, например, `"Hello"` . Программа по очереди выводит каждую букву в верхнем регистре. Второй вариант в нижнем регистре
3) Берется массив цифр , выводится по очереди строка, где написано "element -> index". Такое же для строки
4) Написать аналоги `first` and `last` для строк и для массивов
5) Программа для сравнения двух строк
6) Напишите программу для перевода дней недели с английского на русский. `Monday -> понедельник` итд (через `if/else` и `сase`)
7) Вывести таблицу умножения для числа 3 (while, until, for c in range, each)
```
1 x 3 = 3
2 x 3 = 6
.......
```
8) Сделать программу, которая выводит 
```
*
* *
* * *
* * * *
* * * * *
```
9) Сделать программу, которая выводит
```
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```


10) Напишите программу для перевода названия месяца в цифру . `May -> 5` итд (через `if/else` и `сase`)
11) На вход дается строка, нужно поменять в ней первую и последнюю букву 
12) Найти средний элемент в строке (если строка имеет нечетную длину). Если строка имеет четную длину, то брать более левый элемент (первый из двух средних)
13) Вводим число от 1 до 9. Программа выводит пирамиду нужной длины из звездочек. 
14) Вводим число от 1 до 9. Программа выводит пирамиду нужной длины из цифр. 
15) A leap year is exactly divisible by 4 except for century years (years ending with 00). The century year is a leap year only if it is perfectly divisible by 400.

For example,
```
1999 is not a leap year
2000 is a leap year
2004 is a leap year
```

16) Написать fizz/buzz 
17) На вход приходит список с разными словами `["apple", "banana", "age"......]` (допишите сами) . Программа выводит все слова с введенной буквы
18) Написать аналог reverse для строк
19) Написать программу для поиска палиндромов
20) На вход приходит список чисел`[1, -1, 0......]` (допишите сами) . Программа выводит для каждой цифры "number is positeve/negative/zero" )
21) Сделать функцию `range(num1, num2)`  которая по очереди выводит числа от num1 до num2. Учитывайте, что числа могут быть отрицательные etc)
22) На вход дается массив чисел, написать метод sum, который считает сумму всех чисел
23) Написать полную пирамиду из чисел и звездочек
24) Дается массив из цифр [1, 2, 3, 1, 1, 1, 2, 2, 4, 5, 6, 5, 5] - найти наибольшую последовательность из цифр без прерывания. То есть, здесь будет три "1" 
25) Дается строка, найти наибольшую последовательность из букв без прерывания. 
26) Написать итератор по 3 элемента для массива и строк
27) написать камень/ножницы/бумагу
28) написать бомбочку , вводишь число , она выводит обратный отсчет. Перед цифрой 3 выводит предупреждение, что скоро взрыв, когда доходит до нуля - "Boom"
29) написать калькулятор , принимает три значения (a, b, operator) operator +/-/*/% . Он должен сгенерить выражение и он должен вывести результат.
30) Загадай число. Комп загадывает число от 1 до 100. У вас три попытки. Комп ждем ваши вариант, если угадал - игра заканчивается. Комп говорит больше / меньше


