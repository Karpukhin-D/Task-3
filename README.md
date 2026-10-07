# Практическая работа №3: Управляющие конструкции и операторы ветвления в C# (if, else if, else, switch)
## Выполнил студент группы П25-2.1 Карпухин Дмитрий

### Раздел 1. Базовые условия if и if-else
---
> * №1. Пользователь вводит целое число. Проверить, является ли оно положительным.
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());
        if (number > 0)
        {          
            Console.WriteLine("Число положительное"); 
        }
        else
        {
            Console.WriteLine("Число отрицательное");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.1.png">
</picture>

> * №2. Пользователь вводит целое число. Проверить, является ли оно четным.
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());
        if (number % 2 == 0)
        {          
            Console.WriteLine("Число четное"); 
        }
        else
        {
            Console.WriteLine("Число нечетное");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.2.png">
</picture>

> * №3. Даны два целых числа. Вывести наибольшее из них.
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите первое число: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите второе число: ");
        int b = int.Parse(Console.ReadLine());

        if (a > b)
        {          
            Console.WriteLine($"Наибольшее число: {a}");
        }
        else
        {
            Console.WriteLine($"Наибольшее число: {b}");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.3.png">
</picture>

> * №4. Даны два числа с плавающей точкой. Вывести наименьшее.
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите первое число: ");
        double a = double.Parse(Console.ReadLine());

        Console.Write("Введите второе число: ");
        double b = double.Parse(Console.ReadLine());

        if (a < b)
        {          
            Console.WriteLine($"Наименьшее число: {a}");
        }
        else
        {
            Console.WriteLine($"Наименьшее число: {b}");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.4.png">
</picture>

> * №5. Проверить, делится ли введенное число нацело на 5.
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());
        if (number % 5 == 0)
        {
            Console.WriteLine($"Число {number} делится нацело на 5");
        }
        else
        {
            Console.WriteLine($"Число {number} не делится нацело на 5");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.5.png">
</picture>

> * №6. Проверить, оканчивается ли введенное целое число нулем.
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());
        if (number % 10 == 0)
        {
            Console.WriteLine($"Число {number} оканчивается нулём");
        }
        else
        {
            Console.WriteLine($"Число {number} не оканчивается нулём");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.6.png">
</picture>

> * №7. Пользователь вводит температуру воздуха. Если она ниже нуля, вывести: «На улице мороз, наденьте шапку».
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int temper = int.Parse(Console.ReadLine());
        if (temper < 0)
        {
            Console.WriteLine($"На улице мороз, наденьте шапку");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.7.png">
</picture>

> * №8. Дано число. Если оно больше 100, уменьшить его на 20, иначе увеличить на 10.
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());
        if (number > 100)
        {
            number = number - 20; ;
        }
        else
        {
            number = number + 10;
        }
        Console.WriteLine($"Результат: {number}");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.8.png">
</picture>

> * №9. Ввести два числа. Если они равны, вывести «Числа равны», иначе вывести их произведение.
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите первое число: ");
        double a = double.Parse(Console.ReadLine());

        Console.Write("Введите второе число: ");
        double b = double.Parse(Console.ReadLine());

        if (a == b)
        {
            Console.WriteLine($"Числа равны");
        }
        else
        {
            Console.WriteLine($"Произведение чисел: {a*b}");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.9.png">
</picture>

> * №10. Пользователь вводит свой возраст. Если возраст от 18 и старше, вывести «Доступ разрешен», иначе «Доступ запрещен».
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите свой возраст: ");
        int age = int.Parse(Console.ReadLine());
        if (age >= 18)
        {
            Console.WriteLine("Доступ разрешен");
        }
        else
        {
            Console.WriteLine("Доступ запрещён");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.10.png">
</picture>

> * №11. Ввести число. Если оно трехзначное, вывести «Да», иначе «Нет».
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());
        if (number >= 100 && number <= 999 || number <= -100 && number >= -999)
        {
            Console.WriteLine("Число трёхзначное");
        }
        else
        {
            Console.WriteLine("Число не трёхзначное");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.11.png">
</picture>

> * №12. Проверить, делится ли число на 3 без остатка.
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number % 3 == 0)
        {
            Console.WriteLine("Число делится на 3 без остатка");
        }
        else
        {
            Console.WriteLine("Число не делится на 3 без остатка");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.12.png">
</picture>

> * №13. Даны координаты точки на числовой прямой X. Определить, лежит ли точка правее нуля.
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите координаты точки: ");
        int x = int.Parse(Console.ReadLine());

        if (x > 0)
        {
            Console.WriteLine("Точка лежит правее нуля");
        }
        else
        {
            Console.WriteLine("Точка лежит левее нуля");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.13.png">
</picture>

> * №14. Ввести баланс счета. Если баланс отрицательный, вывести «Задолженность!».
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите баланс счета: ");
        double balance = double.Parse(Console.ReadLine());

        if (balance < 0)
        {
            Console.WriteLine("Задолженность!");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.14.png">
</picture>
> * №15. Пользователь вводит пароль (целое число). Если введен 1234, вывести «Вход выполнен», иначе «Неверный пароль».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите пароль: ");
        int password = int.Parse(Console.ReadLine());

        if (password == 1234)
        {
            Console.WriteLine("Вход выполнен");
        }
        else
        {
            Console.WriteLine("Неверный пароль");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.15.png">
</picture>

> * №16. Проверить, является ли введенное число отрицательным.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int numb = int.Parse(Console.ReadLine());

        if (numb < 0)
        {
            Console.WriteLine("Число отрицательное");
        }
        else
        {
            Console.WriteLine("Число не отрицательное");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.16.png">
</picture>

> * №17. Даны два числа. Вывести разность большего и меньшего числа.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите первое число: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите второе число: ");
        int b = int.Parse(Console.ReadLine());

        if (a > b)
        {
            Console.WriteLine($"Разность: {a - b}");
        }
        else
        {
            Console.WriteLine($"Разность: {b - a}");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.17.png">
</picture>

> * №18. Ввести сумму покупки. Если сумма превышает 1000 рублей, предоставить скидку 5% и вывести итоговую цену.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите сумму покупки: ");
        double price = double.Parse(Console.ReadLine());

        if (price > 1000)
        {
            price = price * 0.95;
        }

            Console.WriteLine($"Итоговая цена: {price}");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.18.png">
</picture>

> * №19. Ввести число. Если оно четное, разделить его на 2, если нечетное — умножить на 3.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number % 2 == 0)
        {
            number = number / 2;
        }
        else
        {
            number = number * 3;
        }
        Console.WriteLine($"Результат: {number}");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.19.png">
</picture>

> * №20. Пользователь вводит скорость движения. Если скорость выше 90 км/ч, вывести сообщение о нарушении.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите скорость движения: ");
        int speed = int.Parse(Console.ReadLine());

        if (speed > 90)
        {
            Console.WriteLine($"Превышена скорость!");
        }
        else
        {
            Console.WriteLine($"Скорость в норме!");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.20.png">
</picture>

> * №21. Дано целое число. Проверить, равно ли оно нулю.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number == 0)
        {
            Console.WriteLine("Число равно нулю");
        }
        else
        {
            Console.WriteLine("Число не равно нулю");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.21.png">
</picture>

> * №22. Ввести два вещественных числа. Проверить, равны ли они с точностью до 0.001.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите первое число: ");
        double a = double.Parse(Console.ReadLine());

        Console.Write("Введите второе число: ");
        double b = double.Parse(Console.ReadLine());

        if (Math.Abs(a - b) < 0.001)
        {
            Console.WriteLine($"Числа равны");
        }
        else
        {
            Console.WriteLine($"Числа не равны");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.22.png">
</picture>

> * №23. Проверить, делится ли число A на число B без остатка.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите первое число: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите второе число: ");
        int b = int.Parse(Console.ReadLine());

        if (b == 0)
        {
            Console.WriteLine($"На ноль делить нельзя!");
        }
        else if (a % b == 0)
        {
            Console.WriteLine($"a делится на b без остатка");
        }
        else
        {
            Console.WriteLine($"a не делится на b без остатка");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.23.png">
</picture>

> * №24. Даны два угла треугольника в градусах. Проверить, существует ли такой треугольник (сумма меньше 180).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите первый угол: ");
        double a = double.Parse(Console.ReadLine());

        Console.Write("Введите второй угол: ");
        double b = double.Parse(Console.ReadLine());

        if (a > 0 && b > 0 && a + b < 180)
        {
            Console.WriteLine($"Такой треугольник существует.");
        }
        else
        {
            Console.WriteLine($"Такой треугольник не существует");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.24.png">
</picture>

> * №25. Ввести радиус круга и сторону квадрата. Определить, у какой фигуры площадь больше.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите радиус круга: ");
        double rad = double.Parse(Console.ReadLine());

        Console.Write("Введите сторону квадрата: ");
        double side = double.Parse(Console.ReadLine());

        double circle = Math.PI * rad * rad;
        double square = side * side;

        if (circle > square)
        {
            Console.WriteLine($"Площадь круга больше");
        }
        else if (square > circle)
        {
            Console.WriteLine($"Площадь квадрата больше");
        }
        else 
        {
            Console.WriteLine($"Площади равны");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.25.png">
</picture>

> * №26. Ввести два числа. Вывести частное большего на меньшее (предусмотреть проверку деления на 0).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите первое число: ");
        double a = double.Parse(Console.ReadLine());

        Console.Write("Введите второе число: ");
        double b = double.Parse(Console.ReadLine());

        double bigger;
        double smaller;

        if (a > b)
        {
            bigger = a;
            smaller = b;
        }
        else
        {
            bigger = b;
            smaller = a;
        }
        if (smaller == 0)
        {
            Console.WriteLine($"Делить на ноль нельзя");
        }
        else
        {
            Console.WriteLine($"Частное: {bigger / smaller}");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.26.png">
</picture>

> * №27. Проверить, является ли последняя цифра числа семеркой.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number % 10 == 7)
        {
            Console.WriteLine("Последняя цифра числа - 7");
        }
        else
        {
            Console.WriteLine("Последняя цифра числа не равна 7");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.27.png">
</picture>

> * №28. Дано число. Если оно нечетное и положительное, вывести «Да».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number % 2 != 0 && number > 0)
        {
            Console.WriteLine("Да");
        }
        else
        {
            Console.WriteLine("Нет");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.28.png">
</picture>

> * №29. Ввести объем свободного места на диске (в ГБ). Если места меньше 5 ГБ, вывести предупреждение.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите объем свободного места на диске: ");
        int m = int.Parse(Console.ReadLine());

        if (m < 5)
        {
            Console.WriteLine("Мало свободного места!");
        }
        else
        {
            Console.WriteLine("Свободного места достаточно");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.29.png">
</picture>

> * №30. Пользователь вводит оценку (2, 3, 4, 5). Если оценка 4 или 5, вывести «Молодец», иначе «Нужно подтянуться».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите оценку: ");
        int grade = int.Parse(Console.ReadLine());

        if (grade == 4 || grade == 5)
        {
            Console.WriteLine("Молодец");
        }
        else
        {
            Console.WriteLine("Нужно подтянуться");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.30.png">
</picture>

> * №31. Даны два символа. Проверить, совпадают ли они.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите первый символ: ");
        char a = char.Parse(Console.ReadLine());

        Console.Write("Введите второй символ: ");
        char b = char.Parse(Console.ReadLine());

        if (a == b)
        {
            Console.WriteLine($"Символы совпадают");
        }
        else
        {
            Console.WriteLine($"Символы не совпадают");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.31.png">
</picture>

> * №32. Ввести число. Если оно кратно и 2, и 7, вывести «Кратно 14».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number % 2 == 0 && number % 7 == 0)
        {
            Console.WriteLine($"Кратно 14");
        }
        else
        {
            Console.WriteLine($"Не кратно 14");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.32.png">
</picture>

> * №33. Ввести массу груза. Если масса превышает допустимые 3.5 тонны, вывести «Перегруз!».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        double massa = double.Parse(Console.ReadLine());

        if (massa > 3.5)
        {
            Console.WriteLine($"Перегруз!");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.33.png">
</picture>

> * №34. Ввести текущее время (часы от 0 до 23). Если время от 6 до 12, вывести «Доброе утро».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите текущее время: ");
        int time = int.Parse(Console.ReadLine());

        if (time >= 6 && time <= 12)
        {
            Console.WriteLine($"Доброе утро!");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.34.png">
</picture>

> * №35. Ввести рост человека в см. Если рост больше 200 см, вывести «Очень высокий».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите рост человека: ");
        double height = double.Parse(Console.ReadLine());

        if (height > 200)
        {
            Console.WriteLine($"Очень высокий");
        }
        else
        {
            Console.WriteLine($"Рост не превышает 200 см");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.35.png">
</picture>

> * №36. Дано двузначное число. Определить, какая из его цифр больше.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите двухзначное число: ");
        int number = int.Parse(Console.ReadLine());

        int a = Math.Abs(number) / 10;
        int b = Math.Abs(number) % 10;

        if (a > b)
        {
            Console.WriteLine($"Первая цифра больше: {a}");
        }
        else if (b > a)
        {
            Console.WriteLine($"Вторая цифра больше: {b}");
        }
        else
        {
            Console.WriteLine($"Цифры равны");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.36.png">
</picture>

> * №37. Ввести стоимость товара. Если товар бесплатный (цена 0), вывести «Акция!».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите стоимость товара: ");
        double price = double.Parse(Console.ReadLine());

        if (price == 0)
        {
            Console.WriteLine($"Акция!");
        }
        else
        {
            Console.WriteLine($"Товар платный");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.37.png">
</picture>

> * №38. Проверить, содержит ли введенное двузначное число одинаковые цифры.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите двухзначное число: ");
        int number = int.Parse(Console.ReadLine());

        int a = Math.Abs(number) / 10;
        int b = Math.Abs(number) % 10;

        if (a == b)
        {
            Console.WriteLine($"Цифры одинаковые");
        }
        else 
        {
            Console.WriteLine($"Цифры не одинаковые");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.38.png">
</picture>

> * №39. Ввести уровень громкости (0–100). Если громкость превышает 80, вывести «Слишком громко для слуха».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите уровень громкости: ");
        int volume = int.Parse(Console.ReadLine());

        if (volume > 80)
        {
            Console.WriteLine($"Слишком громко для слуха");
        }
        else
        {
            Console.WriteLine($"Уровень громкости в норме.");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.39.png">
</picture>

> * №40. Даны два числа. Если их сумма четная, вывести сумму, иначе вывести их разность.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите первое число: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите второе число: ");
        int b = int.Parse(Console.ReadLine());

        if ((a+b)%2==0)
        {
            Console.WriteLine($"Сумма чисел: {a+b}");
        }
        else
        {
            Console.WriteLine($"Разность чисел: {a-b}");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.40.png">
</picture>

> * №41. Ввести количество страниц в документе. Если страниц больше 100, включить двухстороннюю печать.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите количество страниц: ");
        int pages = int.Parse(Console.ReadLine());

        if (pages > 100)
        {
            Console.WriteLine($"Включить двухстороннюю печать");
        }
        else
        {
            Console.WriteLine($"Односторонняя печать");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.41.png">
</picture>

> * №42. Проверить, является ли введенное целое число полным квадратом (для проверки использовать Math.Sqrt).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number >= 0 && Math.Sqrt(number) % 1 == 0)
        {
            Console.WriteLine($"Число является полным квадратом.");
        }
        else
        {
            Console.WriteLine($"Число не является полным квадратом.");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.42.png">
</picture>

> * №43. Ввести атмосферное давление. Если давление ниже 740 мм рт. ст., вывести «Пониженное давление».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите давление: ");
        double davlenie = double.Parse(Console.ReadLine());

        if (davlenie < 740)
        {
            Console.WriteLine($"Пониженное давление");
        }
        else
        {
            Console.WriteLine($"Давление не понижено");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.43.png">
</picture>

> * №44. Ввести количество забитых мячей командами А и Б. Вывести победителя или сообщить о ничьей.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите голы команды А: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите голы команды Б: ");
        int b = int.Parse(Console.ReadLine());

        if (a > b)
        {
            Console.WriteLine($"Победила команда А");
        }
        else if (b > a)
        {
            Console.WriteLine($"Победила команда Б");
        }
        else
        {
            Console.WriteLine($"Ничья");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.44.png">
</picture>

> * №45. Дано число. Заменить его на абсолютную величину (модуль) без использования Math.Abs.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number < 0)
        {
            number = -number;
        }

        Console.WriteLine($"Модуль числа: {number}");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.45.png">
</picture>

> * №46. Ввести показатель уровня сахара в крови. Если показатель выше 6.1 ммоль/л, вывести «Выше нормы».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите уровень сахара: ");
        double sugar = double.Parse(Console.ReadLine());

        if (sugar > 6.1)
        {
            Console.WriteLine($"Выше нормы");
        }
        else
        {
            Console.WriteLine($"Не выше нормы");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.46.png">
</picture>

> * №47. Проверить, хватит ли пользователю средств на счете для оплаты проезда стоимостью 35 рублей.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите баланс счета: ");
        double bal = double.Parse(Console.ReadLine());

        if (bal >= 35)
        {
            Console.WriteLine($"Средств хватает на проезд");
        }
        else
        {
            Console.WriteLine($"Недостаточно средств");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.47.png">
</picture>

> * №48. Ввести номер текущего этажа. Если этаж выше 10, вывести «Высотный этаж».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер этажа: ");
        int floor = int.Parse(Console.ReadLine());

        if (floor > 10)
        {
            Console.WriteLine($"Высотный этаж");
        }
        else
        {
            Console.WriteLine($"Обычный этаж");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.48.png">
</picture>

> * №49. Ввести два слова. Проверить, одинаковы ли они по длине.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите первое слово: ");
        string a = Console.ReadLine();

        Console.Write("Введите второе слово: ");
        string b = Console.ReadLine();

        if (a.Length == b.Length)
        {
            Console.WriteLine($"Слова одинаковы по длине");
        }
        else
        {
            Console.WriteLine($"Слова разной длины");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.49.png">
</picture>

> * №50. Пользователь вводит целое число. Вывести строковое сообщение: «Число четное» либо «Число нечетное».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number % 2 == 0)
        {
            Console.WriteLine($"Число четное");
        }
        else
        {
            Console.WriteLine($"Число нечетное");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.50.png">
</picture>

---
### Раздел 2. Множественные ветвления else if и диапазоны
---
> * №51. Ввести балл за тест (0–100). Вывести оценку по шкале ECTS: A (90-100), B (80-89), C (70-79), D (60-69), F (менее 60).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите балл: ");
        int score = int.Parse(Console.ReadLine());

        if (score >= 90)
            Console.WriteLine($"Оценка: A");
        else if (score >= 80)
            Console.WriteLine($"Оценка: B");
        else if (score >= 70)
            Console.WriteLine($"Оценка: C");
        else if (score >= 60)
            Console.WriteLine($"Оценка: D");
        else
            Console.WriteLine($"Оценка: F");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.51.png">
</picture>

> * №52. Ввести возраст человека. Определить категорию: ребенок (0-12), подросток (13-17), взрослый (18-64), пожилой (65+).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите возраст: ");
        int age = int.Parse(Console.ReadLine());

        if (age <= 12)
            Console.WriteLine($"Ребенок");
        else if (age <= 17)
            Console.WriteLine($"Подросток");
        else if (age <= 64)
            Console.WriteLine($"Взрослый");
        else
            Console.WriteLine($"Пожилой");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.52.png">
</picture>

> * №53. Ввести температуру воды. Вывести ее агрегатное состояние: «Лед» (≤0), «Жидкость» (0<t<100), «Пар» (≥100).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите температуру воды: ");
        double t = double.Parse(Console.ReadLine());

        if (t <= 0)
            Console.WriteLine($"Лед");
        else if (t < 100)
            Console.WriteLine($"Жидкость");
        else
            Console.WriteLine($"Пар");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.53.png">
</picture>

> * №54. Ввести уровень заряда аккумулятора смартфона (в %). Вывести: «Критический» (<10), «Низкий» (10-20), «Нормальный» (21-80), «Полный» (81-100).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите заряд: ");
        int battery = int.Parse(Console.ReadLine());

        if (battery < 10)
            Console.WriteLine($"Критический");
        else if (battery <= 20)
            Console.WriteLine($"Низкий");
        else if (battery <= 80)
            Console.WriteLine($"Нормальный");
        else
            Console.WriteLine($"Полный");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.54.png">
</picture>

> * №55. Ввести число оборотов двигателя в минуту (RPM). Вывести режим: «Заглушен» (0), «Холостой ход» (1-900), «Рабочий» (901-3500), «Красная зона» (3501+).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите RPM: ");
        int rpm = int.Parse(Console.ReadLine());

        if (rpm == 0)
            Console.WriteLine($"Заглушен");
        else if (rpm <= 900)
            Console.WriteLine($"Холостой ход");
        else if (rpm <= 3500)
            Console.WriteLine($"Рабочий");
        else
            Console.WriteLine($"Красная зона");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.55.png">
</picture>

> * №56. Ввести сумму дохода за год. Рассчитать подоходный налог: до 2.4 млн — 13%, до 5 млн — 15%, выше 5 млн — 18%.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите доход за год: ");
        double sum = double.Parse(Console.ReadLine());

        double tax;

        if (sum <= 2400000)
            tax = sum * 0.13;
        else if (sum <= 5000000)
            tax = sum * 0.15;
        else
            tax = sum * 0.18;

        Console.WriteLine($"Налог: {tax} руб.");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.56.png">
</picture>

> * №57. По введенной координате X точки на плоскости (при Y=0) определить ее положение: на нуле, в положительной или отрицательной полуоси.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите X: ");
        double x = double.Parse(Console.ReadLine());

        if (x == 0)
            Console.WriteLine($"Точка находится на нуле");
        else if (x > 0)
            Console.WriteLine($"Положительная полуось");
        else
            Console.WriteLine($"Отрицательная полуось");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.57.png">
</picture>

> * №58. Ввести индекс массы тела (ИМТ). Вывести категорию: дефицит веса (<18.5), норма (18.5-24.9), избыток (25-29.9), ожирение (30+).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите ИМТ: ");
        double imt = double.Parse(Console.ReadLine());

        if (imt < 18.5)
            Console.WriteLine($"Дефицит веса");
        else if (imt < 25)
            Console.WriteLine($"Норма");
        else if (imt < 30)
            Console.WriteLine($"Избыток");
        else
            Console.WriteLine($"Ожирение");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.58.png">
</picture>

> * №59. Ввести скорость ветра (м/с). Вывести категорию по шкале: штиль (<0.2), легкий ветерок (0.2-5), умеренный (5.1-14), шторм (14.1-24), ураган (>24).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите скорость ветра: ");
        double wind = double.Parse(Console.ReadLine());

        if (wind < 0.2)
            Console.WriteLine($"Штиль");
        else if (wind <= 5)
            Console.WriteLine($"Легкий ветерок");
        else if (wind <= 14)
            Console.WriteLine($"Умеренный");
        else if (wind <= 24)
            Console.WriteLine($"Шторм");
        else
            Console.WriteLine($"Ураган");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.59.png">
</picture>

> * №60. Ввести стаж работы сотрудника (в годах). Вывести размер надбавки: <1 года — 0%, 1-5 лет — 5%, 6-10 лет — 10%, >10 лет — 15%.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите стаж работы сотрудника: ");
        int stazh = int.Parse(Console.ReadLine());

        if (stazh < 1)
            Console.WriteLine($"Надбавка: 0%");
        else if (stazh <= 5)
            Console.WriteLine($"Надбавка: 5%");
        else if (stazh <= 10)
            Console.WriteLine($"Надбавка: 10%");
        else
            Console.WriteLine($"Надбавка: 15%");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.60.png">
</picture>

> * №61. Пользователь вводит текущий час (0–23). Вывести: «Ночь» (0-5), «Утро» (6-11), «День» (12-17), «Вечер» (18-23).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите час: ");
        int hour = int.Parse(Console.ReadLine());

        if (hour <= 5)
            Console.WriteLine($"Ночь");
        else if (hour <= 11)
            Console.WriteLine($"Утро");
        else if (hour <= 17)
            Console.WriteLine($"День");
        else
            Console.WriteLine($"Вечер");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.61.png">
</picture>

> * №62. Ввести толщину льда на водоеме (см). Вывести: «Выход запрещен» (<7), «Одиночный пешеход» (7-12), «Группа людей» (13-20), «Транспорт» (>20).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите толщину льда на водоёме: ");
        int ice = int.Parse(Console.ReadLine());

        if (ice < 7)
            Console.WriteLine($"Выход запрещен");
        else if (ice <= 12)
            Console.WriteLine($"Одиночный пешеход");
        else if (ice <= 20)
            Console.WriteLine($"Группа людей");
        else
            Console.WriteLine($"Транспорт");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.62.png">
</picture>

> * №63. Даны три целых числа A, B, C. Найти максимальное из них, используя каскадное условие.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите A: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите B: ");
        int b = int.Parse(Console.ReadLine());

        Console.Write("Введите C: ");
        int c = int.Parse(Console.ReadLine());

        int max;

        if (a >= b && a >= c)
            max = a;
        else if (b >= a && b >= c)
            max = b;
        else
            max = c;

        Console.WriteLine($"Максимальное число: {max}");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.63.png">
</picture>

> * №64. Даны три числа. Найти минимальное из них.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите A: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите B: ");
        int b = int.Parse(Console.ReadLine());

        Console.Write("Введите C: ");
        int c = int.Parse(Console.ReadLine());

        int min;

        if (a <= b && a <= c)
            min = a;
        else if (b <= a && b <= c)
            min = b;
        else
            min = c;

        Console.WriteLine($"Минимальное число: {min}");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.64.png">
</picture>

> * №65. Даны три числа. Определить, сколько из них положительных (0, 1, 2 или 3).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите A: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите B: ");
        int b = int.Parse(Console.ReadLine());

        Console.Write("Введите C: ");
        int c = int.Parse(Console.ReadLine());

        int count = 0;

        if (a > 0)
            count++;

        if (b > 0)
            count++;

        if (c > 0)
            count++;

        Console.WriteLine($"Положительных чисел: {count}");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.65.png">
</picture>

> * №66. Ввести средний балл диплома. Вывести: «Без отличия» (<4.5), «Претендент на красный диплом» (4.5-4.74), «Красный диплом» (≥4.75).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите средний балл: ");
        double grade = double.Parse(Console.ReadLine());

        if (grade < 4.5)
            Console.WriteLine($"Без отличия");
        else if (grade < 4.75)
            Console.WriteLine($"Претендент на красный диплом");
        else
            Console.WriteLine($"Красный диплом");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.66.png">
</picture>

> * №67. Ввести значение артериального давления (систолическое). Вывести: гипотония (<90), норма (90-120), предгипертензия (121-139), гипертензия (≥140).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите давление: ");
        int pressure = int.Parse(Console.ReadLine());

        if (pressure < 90)
            Console.WriteLine($"Гипотония");
        else if (pressure <= 120)
            Console.WriteLine($"Норма");
        else if (pressure <= 139)
            Console.WriteLine($"Предгипертензия");
        else
            Console.WriteLine($"Гипертензия");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.67.png">
</picture>

> * №68. Ввести рейтинг шахматиста (Эло). Вывести ранг: любитель (<1400), разрядник (1400-1999), мастер (2000-2399), гроссмейстер (≥2400).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите рейтинг Эло: ");
        int elo = int.Parse(Console.ReadLine());

        if (elo < 1400)
            Console.WriteLine($"Любитель");
        else if (elo < 2000)
            Console.WriteLine($"Разрядник");
        else if (elo < 2400)
            Console.WriteLine($"Мастер");
        else
            Console.WriteLine($"Гроссмейстер");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.68.png">
</picture>

> * №69. Ввести число и определить, сколькизначным оно является (однозначное, двузначное, трехзначное или более).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        number = Math.Abs(number);

        if (number < 10)
            Console.WriteLine($"Однозначное");
        else if (number < 100)
            Console.WriteLine($"Двузначное");
        else if (number < 1000)
            Console.WriteLine($"Трехзначное");
        else
            Console.WriteLine($"Более трехзначного");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.69.png">
</picture>

> * №70. Ввести дальность поездки на такси (км). Рассчитать тариф: до 5 км — 200 руб, от 5 до 15 км — 200 + 25 руб/км, свыше 15 км — 200 + 20 руб/км.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите расстояние: ");
        double km = double.Parse(Console.ReadLine());

        double price;

        if (km <= 5)
            price = 200;
        else if (km <= 15)
            price = 200 + (km - 5) * 25;
        else
            price = 200 + 10 * 25 + (km - 15) * 20;

        Console.WriteLine($"Стоимость поездки: {price} руб.");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.70.png">
</picture>

> * №71. Ввести количество осадков за сутки (мм). Определить: без осадков (0), слабый дождь (0.1-4), умеренный (4.1-15), сильный ливень (>15).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите количество осадков: ");
        double rain = double.Parse(Console.ReadLine());

        if (rain == 0)
            Console.WriteLine($"Без осадков");
        else if (rain <= 4)
            Console.WriteLine($"Слабый дождь");
        else if (rain <= 15)
            Console.WriteLine($"Умеренный");
        else
            Console.WriteLine($"Сильный ливень");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.71.png">
</picture>

> * №72. Ввести процент выполнения плана продаж. Вывести статус: план сорван (<70), удовлетворительно (70-99%), выполнен (100-119%), перевыполнен (≥120).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите процент выполнения плана: ");
        int percent = int.Parse(Console.ReadLine());

        if (percent < 70)
            Console.WriteLine($"План сорван");
        else if (percent < 100)
            Console.WriteLine($"Удовлетворительно");
        else if (percent < 120)
            Console.WriteLine($"Выполнен");
        else
            Console.WriteLine($"Перевыполнен");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.72.png">
</picture>

> * №73. Даны три числа. Упорядочить их по возрастанию и вывести на консоль.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите A: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите B: ");
        int b = int.Parse(Console.ReadLine());

        Console.Write("Введите C: ");
        int c = int.Parse(Console.ReadLine());

        if (a > b)
        {
            int temp = a;
            a = b;
            b = temp;
        }

        if (a > c)
        {
            int temp = a;
            a = c;
            c = temp;
        }

        if (b > c)
        {
            int temp = b;
            b = c;
            c = temp;
        }

        Console.WriteLine($"По возрастанию: {a}, {b}, {c}");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.73.png">
</picture>

> * №74. Дано число X. Вычислить значение кусочно-заданной функции: f(x)=x^2, если x>0; f(x)=0, если x=0; f(x)=−x, если x<0.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите X: ");
        double x = double.Parse(Console.ReadLine());

        double f;

        if (x > 0)
            f = x * x;
        else if (x == 0)
            f = 0;
        else
            f = -x;

        Console.WriteLine($"f(x) = {f}");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.74.png">
</picture>

> * №75. Ввести октановое число бензина. Классифицировать: <92 — несоответствие стандарту, 92 — АИ-92, 95 — АИ-95, 98-100 — АИ-98/100, >100 — спорт/авиатопливо.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите октановое число бензина: ");
        int octane = int.Parse(Console.ReadLine());

        if (octane < 92)
            Console.WriteLine($"Несоответствие стандарту");
        else if (octane == 92)
            Console.WriteLine($"АИ-92");
        else if (octane == 95)
            Console.WriteLine($"АИ-95");
        else if (octane <= 100)
            Console.WriteLine($"АИ-98/100");
        else
            Console.WriteLine($"Спорт/авиатопливо");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.75.png">
</picture>

> * №76. Ввести сумму покупок за месяц для начисления кешбэка: до 10 000 руб — 1%, до 50 000 руб — 3%, свыше 50 000 руб — 5%. Вывести сумму кешбэка.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите сумму покупок: ");
        double sum = double.Parse(Console.ReadLine());

        double cashback;

        if (sum <= 10000)
            cashback = sum * 0.01;
        else if (sum <= 50000)
            cashback = sum * 0.03;
        else
            cashback = sum * 0.05;

        Console.WriteLine($"Кешбэк: {cashback} руб.");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.76.png">
</picture>

> * №77. Ввести глубину погружения аквалангиста (метры). Вывести зону: рекреационная (<40), техническая (40-100), глубоководная (>100).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите глубину погружения аквалангиста: ");
        double depth = double.Parse(Console.ReadLine());

        if (depth < 40)
            Console.WriteLine($"Рекреационная зона");
        else if (depth <= 100)
            Console.WriteLine($"Техническая зона");
        else
            Console.WriteLine($"Глубоководная зона");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.77.png">
</picture>

> * №78. Ввести количество штрафных баллов водителя. Вывести: «Предупреждение» (1-5), «Временное ограничение» (6-10), «Лишение прав» (>10).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите количество штрафных баллов: ");
        int points = int.Parse(Console.ReadLine());

        if (points >= 1 && points <= 5)
            Console.WriteLine($"Предупреждение");
        else if (points <= 10)
            Console.WriteLine($"Временное ограничение");
        else if (points > 10)
            Console.WriteLine($"Лишение прав");
        else
            Console.WriteLine($"Нарушений нет");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.78.png">
</picture>

> * №79. Ввести уровень кислотности почвы (pH). Определить: кислая (<6.0), нейтральная (6.0-7.2), щелочная (>7.2).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите pH: ");
        double ph = double.Parse(Console.ReadLine());

        if (ph < 6.0)
            Console.WriteLine($"Кислая");
        else if (ph <= 7.2)
            Console.WriteLine($"Нейтральная");
        else
            Console.WriteLine($"Щелочная");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.79.png">
</picture>

> * №80. Ввести количество набранных очков в компьютерной игре. Присвоить медаль: Бронзовая (1000-2499), Серебряная (2500-4999), Золотая (5000+), иначе без медали.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите количество набранных очков: ");
        int points = int.Parse(Console.ReadLine());

        if (points >= 1000)
            Console.WriteLine($"Бронзовая медаль");
        else if (points >= 2500)
            Console.WriteLine($"Серебряная медаль");
        else if (points >= 5000)
            Console.WriteLine($"Золотая медаль");
        else
            Console.WriteLine($"Без медали");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.80.png">
</picture>

> * №81. Ввести крепость напитка в градусах. Классифицировать: безалкогольный (0), слабоалкогольный (0.1-8), среднеалкогольный (8.1-25), крепкий (>25).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите крепость: ");
        double degree = double.Parse(Console.ReadLine());

        if (degree == 0)
            Console.WriteLine($"Безалкогольный");
        else if (degree <= 8)
            Console.WriteLine($"Слабоалкогольный");
        else if (degree <= 25)
            Console.WriteLine($"Среднеалкогольный");
        else
            Console.WriteLine($"Крепкий");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.81.png">
</picture>

> * №82. Ввести показатель уровня шума в децибелах (дБ). Вывести вердикт: тихо (<40), норма (40-60), шумно (61-80), вредно для здоровья (>80).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите уровень шума: ");
        int noise = int.Parse(Console.ReadLine());

        if (noise < 40)
            Console.WriteLine($"Тихо");
        else if (noise <= 60)
            Console.WriteLine($"Норма");
        else if (noise <= 80)
            Console.WriteLine($"Шумно");
        else
            Console.WriteLine($"Вредно для здоровья");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.82.png">
</picture>

> * №83. Ввести вес почтовой посылки (кг). Рассчитать категорию отправления: мелкий пакет (<2), стандартная (2-10), тяжеловесная (10.1-31.5), крупногабарит (>31.5).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите вес почтовой посылки: ");
        double weight = double.Parse(Console.ReadLine());

        if (weight < 2)
            Console.WriteLine($"Мелкий пакет");
        else if (weight <= 10)
            Console.WriteLine($"Стандартная");
        else if (weight <= 31.5)
            Console.WriteLine($"Тяжеловесная");
        else
            Console.WriteLine($"Крупногабарит");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.83.png">
</picture>

> * №84. Ввести количество комнат в квартире. Вывести: студия/однокомнатная (1), двухкомнатная (2), трехкомнатная (3), многокомнатная (4+).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите количество комнат: ");
        int rooms = int.Parse(Console.ReadLine());

        if (rooms == 1)
            Console.WriteLine($"Студия/однокомнатная");
        else if (rooms == 2)
            Console.WriteLine($"Двухкомнатная");
        else if (rooms == 3)
            Console.WriteLine($"Трехкомнатная");
        else
            Console.WriteLine($"Многокомнатная");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.84.png">
</picture>

> * №85. Ввести процент заряда повербанка. Вывести количество светящихся светодиодов на корпусе (1, 2, 3 или 4).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите заряд повербанка: ");
        int charge = int.Parse(Console.ReadLine());

        if (charge <= 25)
            Console.WriteLine($"Светодиодов: 1");
        else if (charge <= 50)
            Console.WriteLine($"Светодиодов: 2");
        else if (charge <= 75)
            Console.WriteLine($"Светодиодов: 3");
        else
            Console.WriteLine($"Светодиодов: 4");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.85.png">
</picture>

> * №86. Ввести выслугу лет военнослужащего. Вывести процент пенсионной надбавки.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите выслугу лет: ");
        int years = int.Parse(Console.ReadLine());

        if (years < 5)
            Console.WriteLine($"Надбавка: 5%");
        else if (years <= 10)
            Console.WriteLine($"Надбавка: 10%");
        else
            Console.WriteLine($"Надбавка: 15%");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.86.png">
</picture>

> * №87. Ввести время отклика сервера (пинг в мс). Вывести: идеальный (<20), хороший (20-60), посредственный (61-120), плохой (>120).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите пинг: ");
        int ping = int.Parse(Console.ReadLine());

        if (ping < 20)
            Console.WriteLine($"Идеальный");
        else if (ping <= 60)
            Console.WriteLine($"Хороший");
        else if (ping <= 120)
            Console.WriteLine($"Посредственный");
        else
            Console.WriteLine($"Плохой");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.87.png">
</picture>

> * №88. Ввести концентрацию CO2 в помещении (ppm). Вывести вердикт: норма (<800), душно (800-1200), проветрить немедленно (>1200).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите концентрацию CO2: ");
        int co2 = int.Parse(Console.ReadLine());

        if (co2 < 800)
            Console.WriteLine($"Норма");
        else if (co2 <= 1200)
            Console.WriteLine($"Душно");
        else
            Console.WriteLine($"Проветрить немедленно");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.88.png">
</picture>

> * №89. Ввести количество пройденных шагов за день. Вывести: гиподинамия (<5000), норма (5000-9999), активный день (10000-14999), рекорд (>15000).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите количество шагов: ");
        int steps = int.Parse(Console.ReadLine());

        if (steps < 5000)
            Console.WriteLine($"Гиподинамия");
        else if (steps < 10000)
            Console.WriteLine($"Норма");
        else if (steps < 15000)
            Console.WriteLine($"Активный день");
        else
            Console.WriteLine($"Рекорд");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.89.png">
</picture>

> * №90. Ввести диаметр автомобильного колесного диска в дюймах. Определить класс: малолитражки (13-14), компактные авто (15-16), кроссоверы/бизнес (17-19), внедорожники/спорт (20+).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите диаметр диска: ");
        int disk = int.Parse(Console.ReadLine());

        if (disk <= 14)
            Console.WriteLine($"Малолитражки");
        else if (disk <= 16)
            Console.WriteLine($"Компактные авто");
        else if (disk <= 19)
            Console.WriteLine($"Кроссоверы/бизнес");
        else
            Console.WriteLine($"Внедорожники/спорт");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.90.png">
</picture>

> * №91. Ввести значение влажности воздуха (%). Вывести: сухой воздух (<30), комфорт (30-60), повышенная влажность (>60).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите влажность: ");
        int vlazh = int.Parse(Console.ReadLine());

        if (vlazh < 30)
            Console.WriteLine($"Сухой воздух");
        else if (vlazh <= 60)
            Console.WriteLine($"Комфорт");
        else
            Console.WriteLine($"Повышенная влажность");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.91.png">
</picture>

> * №92. Даны три числа. Проверить, сколько из них равны между собой (все разные, два равны, все три равны).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите A: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите B: ");
        int b = int.Parse(Console.ReadLine());

        Console.Write("Введите C: ");
        int c = int.Parse(Console.ReadLine());

        if (a == b && b == c)
            Console.WriteLine($"Все три равны");
        else if (a == b || a == c || b == c)
            Console.WriteLine($"Два числа равны");
        else
            Console.WriteLine($"Все разные");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.92.png">
</picture>

> * №93. Ввести номер четверти координатной плоскости (1–4) и вывести диапазоны знаков для координат X и Y.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер четверти: ");
        int quarter = int.Parse(Console.ReadLine());

        if (quarter == 1)
            Console.WriteLine($"X положительный, Y положительный");
        else if (quarter == 2)
            Console.WriteLine($"X отрицательный, Y положительный");
        else if (quarter == 3)
            Console.WriteLine($"X отрицательный, Y отрицательный");
        else if (quarter == 4)
            Console.WriteLine($"X положительный, Y отрицательный");
        else
            Console.WriteLine($"Такой четверти нет");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.93.png">
</picture>

> * №94. Ввести температуру процессора компьютера. Вывести: холодный (<45), нормальная нагрузка (45-75), троттлинг/перегрев (>75).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите температуру процессора: ");
        int temperat = int.Parse(Console.ReadLine());

        if (temperat < 45)
            Console.WriteLine($"Холодный");
        else if (temperat <= 75)
            Console.WriteLine($"Нормальная нагрузка");
        else
            Console.WriteLine($"Троттлинг/перегрев");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.94.png">
</picture>

> * №95. Ввести остаток срока годности продукта в днях. Вывести: «Срочно употребить» (≤2), «Нормально» (3-30), «Длительное хранение» (>30).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите остаток срока годности: ");
        int days = int.Parse(Console.ReadLine());

        if (days <= 2)
            Console.WriteLine($"Срочно употребить");
        else if (days <= 30)
            Console.WriteLine($"Нормально");
        else
            Console.WriteLine($"Длительное хранение");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.95.png">
</picture>

> * №96. Ввести сумму кредита и срок. Рассчитать процентную ставку в зависимости от срока (до года, до трех лет, свыше трех лет).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите сумму кредита: ");
        double credit = double.Parse(Console.ReadLine());

        Console.Write("Введите срок в годах: ");
        int years = int.Parse(Console.ReadLine());

        double stavka;

        if (years <= 1)
            stavka = 10;
        else if (years <= 3)
            stavka = 15;
        else
            stavka = 25;

        Console.WriteLine($"Сумма кредита: {credit} руб.");
        Console.WriteLine($"Процентная ставка: {stavka}%");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.96.png">
</picture>

> * №97. Ввести частоту обновления монитора (Гц). Определить: офис (60-75), базовый игровой (120-144), киберспорт (165+).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите частоту монитора: ");
        int hz = int.Parse(Console.ReadLine());

        if (hz >= 60 && hz <= 75)
            Console.WriteLine($"Офис");
        else if (hz >= 120 && hz <= 144)
            Console.WriteLine($"Базовый игровой");
        else if (hz >= 165)
            Console.WriteLine($"Киберспорт");
        else
            Console.WriteLine($"Другая частота");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.97.png">
</picture>

> * №98. Ввести расход топлива автомобиля на 100 км пути. Вывести вердикт: экономичный (<6 л), средний (6-10 л), прожорливый (>10 л).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите расход топлива: ");
        double fuel = double.Parse(Console.ReadLine());

        if (fuel < 6)
            Console.WriteLine($"Экономичный");
        else if (fuel <= 10)
            Console.WriteLine($"Средний");
        else
            Console.WriteLine($"Прожорливый");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.98.png">
</picture>

> * №99. Ввести количество страниц книги. Классифицировать: брошюра (<48), повесть (48-150), роман (151-600), фолиант (>600).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите количество страниц: ");
        int pages = int.Parse(Console.ReadLine());

        if (pages < 48)
            Console.WriteLine($"Брошюра");
        else if (pages <= 150)
            Console.WriteLine($"Повесть");
        else if (pages <= 600)
            Console.WriteLine($"Роман");
        else
            Console.WriteLine($"Фолиант");
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.99.png">
</picture>

> * №100. Ввести число и проверить, попадает ли оно в интервалы [0;10], [20;30] или [50;100].

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if ((number >= 0 && number <= 10) ||
            (number >= 20 && number <= 30) ||
            (number >= 50 && number <= 100))
        {
            Console.WriteLine($"Число попадает в один из интервалов");
        }
        else
        {
            Console.WriteLine($"Число не попадает в интервалы");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/Karpukhin-D/Task-3/blob/main/task%203/1.1.100.png">
</picture>

---
### Раздел 3. Составные логические условия &&, ||, !
---

> * №101. Дано целое число. Проверить, принадлежит ли оно числовому отрезку [10;50].

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number >= 10 && number <= 50)
            Console.WriteLine($"Число принадлежит отрезку");
        else
            Console.WriteLine($"Число не принадлежит отрезку");
    }
}
```

> * №102. Проверить, является ли введенное целое число положительным и четным одновременно.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number > 0 && number % 2 == 0)
            Console.WriteLine($"Число положительное и четное");
        else
            Console.WriteLine($"Условие не выполнено");
    }
}
```

> * №103. Проверить, лежит ли число вне диапазона [−10;10].

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number < -10 || number > 10)
            Console.WriteLine($"Число вне диапазона");
        else
            Console.WriteLine($"Число внутри диапазона");
    }
}
```

> * №104. Ввести логин и пароль пользователя. Вывести «Успех», если логин равен admin и пароль secret.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите логин: ");
        string login = Console.ReadLine();

        Console.Write("Введите пароль: ");
        string password = Console.ReadLine();

        if (login == "admin" && password == "secret")
            Console.WriteLine($"Успех");
        else
            Console.WriteLine($"Ошибка");
    }
}
```

> * №105. Проверить, является ли введенный год високосным (делится на 4, но не на 100, либо делится на 400).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите год: ");
        int year = int.Parse(Console.ReadLine());

        if ((year % 4 == 0 && year % 100 != 0) || year % 400 == 0)
            Console.WriteLine($"Год високосный");
        else
            Console.WriteLine($"Год не високосный");
    }
}
```

> * №106. Даны координаты точки (X,Y). Определить, попадает ли точка в I координатную четверть (X>0 и Y>0).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите X: ");
        int x = int.Parse(Console.ReadLine());

        Console.Write("Введите Y: ");
        int y = int.Parse(Console.ReadLine());

        if (x > 0 && y > 0)
            Console.WriteLine($"Точка находится в I четверти");
        else
            Console.WriteLine($"Точка не находится в I четверти");
    }
}
```

> * №107. Определить, попадает ли точка (X,Y) во II четверть плоскости.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите X: ");
        int x = int.Parse(Console.ReadLine());

        Console.Write("Введите Y: ");
        int y = int.Parse(Console.ReadLine());

        if (x < 0 && y > 0)
            Console.WriteLine($"Точка находится во II четверти");
        else
            Console.WriteLine($"Точка не находится во II четверти");
    }
}
```

> * №108. Определить, попадает ли точка (X,Y) в III четверть плоскости.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите X: ");
        int x = int.Parse(Console.ReadLine());

        Console.Write("Введите Y: ");
        int y = int.Parse(Console.ReadLine());

        if (x < 0 && y < 0)
            Console.WriteLine($"Точка находится в III четверти");
        else
            Console.WriteLine($"Точка не находится в III четверти");
    }
}
```

> * №109. Определить, попадает ли точка (X,Y) в IV четверть плоскости.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите X: ");
        int x = int.Parse(Console.ReadLine());

        Console.Write("Введите Y: ");
        int y = int.Parse(Console.ReadLine());

        if (x > 0 && y < 0)
            Console.WriteLine($"Точка находится в IV четверти");
        else
            Console.WriteLine($"Точка не находится в IV четверти");
    }
}
```

> * №110. Даны три стороны A, B, C. Проверить, является ли треугольник прямоугольным (теорема Пифагора).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите A: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите B: ");
        int b = int.Parse(Console.ReadLine());

        Console.Write("Введите C: ");
        int c = int.Parse(Console.ReadLine());

        if (a * a + b * b == c * c ||
            a * a + c * c == b * b ||
            b * b + c * c == a * a)
            Console.WriteLine($"Треугольник прямоугольный");
        else
            Console.WriteLine($"Треугольник не прямоугольный");
    }
}
```

> * №111. Даны три стороны. Проверить, является ли треугольник равнобедренным.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите A: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите B: ");
        int b = int.Parse(Console.ReadLine());

        Console.Write("Введите C: ");
        int c = int.Parse(Console.ReadLine());

        if (a == b || a == c || b == c)
            Console.WriteLine($"Треугольник равнобедренный");
        else
            Console.WriteLine($"Треугольник не равнобедренный");
    }
}
```

> * №112. Ввести возраст и стаж вождения. Разрешить аренду каршеринга бизнес-класса, если возраст ≥23 лет И стаж ≥3 лет.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите возраст: ");
        int age = int.Parse(Console.ReadLine());

        Console.Write("Введите стаж: ");
        int stazh = int.Parse(Console.ReadLine());

        if (age >= 23 && stazh >= 3)
            Console.WriteLine($"Аренда разрешена");
        else
            Console.WriteLine($"Аренда запрещена");
    }
}
```

> * №113. Проверить, делится ли число одновременно на 3 и на 5 без остатка.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number % 3 == 0 && number % 5 == 0)
            Console.WriteLine($"Число делится на 3 и 5");
        else
            Console.WriteLine($"Число не подходит");
    }
}
```

> * №114. Проверить, является ли число трехзначным и оканчивается ли оно на цифру 5.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number >= 100 && number <= 999 && number % 10 == 5)
            Console.WriteLine($"Условие выполнено");
        else
            Console.WriteLine($"Условие не выполнено");
    }
}
```

> * №115. Даны три числа. Проверить, упорядочены ли они строго по возрастанию (A<B<C).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите A: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите B: ");
        int b = int.Parse(Console.ReadLine());

        Console.Write("Введите C: ");
        int c = int.Parse(Console.ReadLine());

        if (a < b && b < c)
            Console.WriteLine($"Числа упорядочены по возрастанию");
        else
            Console.WriteLine($"Числа не упорядочены");
    }
}
```

> * №116. Проверить, верно ли, что среди трех введенных чисел есть хотя бы одно четное.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите A: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите B: ");
        int b = int.Parse(Console.ReadLine());

        Console.Write("Введите C: ");
        int c = int.Parse(Console.ReadLine());

        if (a % 2 == 0 || b % 2 == 0 || c % 2 == 0)
            Console.WriteLine($"Есть хотя бы одно четное число");
        else
            Console.WriteLine($"Четных чисел нет");
    }
}
```

> * №117. Проверить, верно ли, что среди трех чисел ровно одно равно нулю.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите A: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите B: ");
        int b = int.Parse(Console.ReadLine());

        Console.Write("Введите C: ");
        int c = int.Parse(Console.ReadLine());

        if ((a == 0 && b != 0 && c != 0) ||
            (a != 0 && b == 0 && c != 0) ||
            (a != 0 && b != 0 && c == 0))
            Console.WriteLine($"Ровно одно число равно нулю");
        else
            Console.WriteLine($"Условие не выполнено");
    }
}
```

> * №118. Ввести температуру и влажность. Вывести предупреждение о гололедице, если температура ≤0∘C И влажность >85.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите температуру: ");
        double temperature = double.Parse(Console.ReadLine());

        Console.Write("Введите влажность: ");
        double humidity = double.Parse(Console.ReadLine());

        if (temperature <= 0 && humidity > 85)
            Console.WriteLine($"Предупреждение: Возможна гололедица!");
        else
            Console.WriteLine($"Условие гололедицы не выполнено");
    }
}
```

> * №119. Даны координаты точки (X,Y). Проверить, лежит ли точка внутри круга радиуса R с центром в начале координат (x2+y2≤R2).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите X: ");
        double x = double.Parse(Console.ReadLine());

        Console.Write("Введите Y: ");
        double y = double.Parse(Console.ReadLine());

        Console.Write("Введите R: ");
        double r = double.Parse(Console.ReadLine());

        if (x * x + y * y <= r * r)
            Console.WriteLine($"Точка находится внутри круга");
        else
            Console.WriteLine($"Точка находится вне круга");
    }
}
```

> * №120. Даны координаты точки (X,Y). Проверить, лежит ли точка внутри прямоугольника со сторонами, параллельными осям, заданного углами (X1,Y1) и (X2,Y2).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите X точки: ");
        double x = double.Parse(Console.ReadLine());

        Console.Write("Введите Y точки: ");
        double y = double.Parse(Console.ReadLine());

        Console.Write("Введите X1: ");
        double x1 = double.Parse(Console.ReadLine());

        Console.Write("Введите Y1: ");
        double y1 = double.Parse(Console.ReadLine());

        Console.Write("Введите X2: ");
        double x2 = double.Parse(Console.ReadLine());

        Console.Write("Введите Y2: ");
        double y2 = double.Parse(Console.ReadLine());

        double minX = Math.Min(x1, x2);
        double maxX = Math.Max(x1, x2);
        double minY = Math.Min(y1, y2);
        double maxY = Math.Max(y1, y2);

        if (x >= minX && x <= maxX &&
            y >= minY && y <= maxY)
            Console.WriteLine($"Точка находится внутри прямоугольника");
        else
            Console.WriteLine($"Точка находится вне прямоугольника");
    }
}
```

> * №121. Ввести день и месяц рождения. Проверить, корректна ли дата (например, день от 1 до 31, месяц от 1 до 12, с учетом длины месяцев).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите день: ");
        int day = int.Parse(Console.ReadLine());

        Console.Write("Введите месяц: ");
        int month = int.Parse(Console.ReadLine());

        int daysInMonth = 0;

        if (month == 2)
            daysInMonth = 28;
        else if (month == 4 || month == 6 || month == 9 || month == 11)
            daysInMonth = 30;
        else if (month >= 1 && month <= 12)
            daysInMonth = 31;

        if (day >= 1 && day <= daysInMonth)
            Console.WriteLine($"Дата корректна");
        else
            Console.WriteLine($"Дата некорректна");
    }
}
```

> * №122. Ввести номер месяца. Проверить, относится ли он к зимнему периоду (12, 1 или 2).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер месяца: ");
        int month = int.Parse(Console.ReadLine());

        if (month == 12 || month == 1 || month == 2)
            Console.WriteLine($"Это зимний месяц");
        else
            Console.WriteLine($"Это не зимний месяц");
    }
}
```

> * №123. Проверить, является ли четырехзначное число «счастливым билетом» (сумма первых двух цифр равна сумме двух последних).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите четырехзначное число: ");
        int number = int.Parse(Console.ReadLine());

        if (number >= 1000 && number <= 9999)
        {
            int first = number / 1000;
            int second = number / 100 % 10;
            int third = number / 10 % 10;
            int fourth = number % 10;

            if (first + second == third + fourth)
                Console.WriteLine($"Билет счастливый");
            else
                Console.WriteLine($"Билет не счастливый");
        }
        else
        {
            Console.WriteLine($"Число не четырехзначное");
        }
    }
}
```

> * №124. Ввести три числа. Проверить истинность высказывания: «Хотя бы одна пара чисел взаимно противоположна (A=−B)».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите A: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите B: ");
        int b = int.Parse(Console.ReadLine());

        Console.Write("Введите C: ");
        int c = int.Parse(Console.ReadLine());

        if (a == -b || a == -c || b == -c)
            Console.WriteLine($"Есть взаимно противоположная пара");
        else
            Console.WriteLine($"Такой пары нет");
    }
}
```

> * №125. Пользователь вводит показания двух датчиков аварии. Сформировать тревогу, если сработал хотя бы один датчик И при этом включен тумблер защиты.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Сработал первый датчик? ");
        bool sensor1 = bool.Parse(Console.ReadLine());

        Console.Write("Сработал второй датчик? ");
        bool sensor2 = bool.Parse(Console.ReadLine());

        Console.Write("Тумблер защиты включен? ");
        bool tumbler = bool.Parse(Console.ReadLine());

        if ((sensor1 || sensor2) && tumbler)
            Console.WriteLine($"ТРЕВОГА");
        else
            Console.WriteLine($"Тревоги нет");
    }
}
```

> * №126. Проверить, лежит ли число X строго между числами A и B (учесть, что A может быть больше B).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите A: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите B: ");
        int b = int.Parse(Console.ReadLine());

        Console.Write("Введите X: ");
        int x = int.Parse(Console.ReadLine());

        if ((x > a && x < b) || (x > b && x < a))
            Console.WriteLine($"X находится между A и B");
        else
            Console.WriteLine($"X не находится между A и B");
    }
}
```

> * №127. Даны два целых числа. Проверить, имеют ли они одинаковый знак (оба положительные или оба отрицательные).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите A: ");
        int a = int.Parse(Console.ReadLine());

        Console.Write("Введите B: ");
        int b = int.Parse(Console.ReadLine());

        if ((a > 0 && b > 0) || (a < 0 && b < 0))
            Console.WriteLine($"Числа имеют одинаковый знак");
        else
            Console.WriteLine($"Числа имеют разные знаки");
    }
}
```

> * №128. Даны шахматные координаты двух клеток (x1,y1) и (x2,y2) от 1 до 8. Определить, угрожает ли ладья с первой клетки фигуре на второй клетке (совпадает либо строка, либо столбец).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите X1: ");
        int x1 = int.Parse(Console.ReadLine());

        Console.Write("Введите Y1: ");
        int y1 = int.Parse(Console.ReadLine());

        Console.Write("Введите X2: ");
        int x2 = int.Parse(Console.ReadLine());

        Console.Write("Введите Y2: ");
        int y2 = int.Parse(Console.ReadLine());

        if (x1 == x2 || y1 == y2)
            Console.WriteLine($"Ладья угрожает фигуре");
        else
            Console.WriteLine($"Ладья не угрожает фигуре");
    }
}
```

> * №129. Для двух клеток шахматной доски определить, угрожает ли слон (разность координат по модулю одинакова).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите X1: ");
        int x1 = int.Parse(Console.ReadLine());

        Console.Write("Введите Y1: ");
        int y1 = int.Parse(Console.ReadLine());

        Console.Write("Введите X2: ");
        int x2 = int.Parse(Console.ReadLine());

        Console.Write("Введите Y2: ");
        int y2 = int.Parse(Console.ReadLine());

        if (Math.Abs(x1 - x2) == Math.Abs(y1 - y2))
            Console.WriteLine($"Слон угрожает фигуре");
        else
            Console.WriteLine($"Слон не угрожает фигуре");
    }
}
```

> * №130. Для двух клеток шахматной доски определить, угрожает ли ферзь (объединение логики ладьи и слона).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите X1: ");
        int x1 = int.Parse(Console.ReadLine());

        Console.Write("Введите Y1: ");
        int y1 = int.Parse(Console.ReadLine());

        Console.Write("Введите X2: ");
        int x2 = int.Parse(Console.ReadLine());

        Console.Write("Введите Y2: ");
        int y2 = int.Parse(Console.ReadLine());

        if (x1 == x2 || y1 == y2 ||
            Math.Abs(x1 - x2) == Math.Abs(y1 - y2))
            Console.WriteLine($"Ферзь угрожает фигуре");
        else
            Console.WriteLine($"Ферзь не угрожает фигуре");
    }
}
```

> * №131. Для двух клеток определить, может ли конь пойти с одной на другую.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите x1: ");
        int x1 = int.Parse(Console.ReadLine());

        Console.Write("Введите y1: ");
        int y1 = int.Parse(Console.ReadLine());

        Console.Write("Введите x2: ");
        int x2 = int.Parse(Console.ReadLine());

        Console.Write("Введите y2: ");
        int y2 = int.Parse(Console.ReadLine());

        if ((Math.Abs(x1 - x2) == 1 && Math.Abs(y1 - y2) == 2) ||
            (Math.Abs(x1 - x2) == 2 && Math.Abs(y1 - y2) == 1))
            Console.WriteLine($"Конь может пойти");
        else
            Console.WriteLine($"Конь не может пойти");
    }
}
```

> * №132. Для двух клеток шахматной доски проверить, одинакового ли они цвета.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите x1: ");
        int x1 = int.Parse(Console.ReadLine());

        Console.Write("Введите y1: ");
        int y1 = int.Parse(Console.ReadLine());

        Console.Write("Введите x2: ");
        int x2 = int.Parse(Console.ReadLine());

        Console.Write("Введите y2: ");
        int y2 = int.Parse(Console.ReadLine());

        if ((x1 + y1) % 2 == (x2 + y2) % 2)
            Console.WriteLine($"Клетки одного цвета");
        else
            Console.WriteLine($"Клетки разных цветов");
    }
}
```

> * №133. Ввести рост и вес кандидата в космонавты. Проверить соответствие: рост от 160 до 190 см И вес от 50 до 90 кг.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите рост: ");
        int height = int.Parse(Console.ReadLine());

        Console.Write("Введите вес: ");
        int weight = int.Parse(Console.ReadLine());

        if (height >= 160 && height <= 190 &&
            weight >= 50 && weight <= 90)
            Console.WriteLine($"Кандидат подходит");
        else
            Console.WriteLine($"Кандидат не подходит");
    }
}
```

> * №134. Дано натуральное число N. Проверить, является ли оно четным двузначным числом.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number >= 10 && number <= 99 && number % 2 == 0)
            Console.WriteLine($"Число четное и двузначное");
        else
            Console.WriteLine($"Условие не выполнено");
    }
}
```

> * №135. Дано натуральное число. Проверить, является ли оно нечетным трехзначным числом.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if (number >= 100 && number <= 999 && number % 2 != 0)
            Console.WriteLine($"Число нечетное и трехзначное");
        else
            Console.WriteLine($"Условие не выполнено");
    }
}
```

> * №136. Ввести результаты двух экзаменов (математика и информатика). Абитуриент зачислен, если сумма баллов ≥150 И по каждому предмету не менее 50 баллов.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите баллы по математике: ");
        int math = int.Parse(Console.ReadLine());

        Console.Write("Введите баллы по информатике: ");
        int informatics = int.Parse(Console.ReadLine());

        if (math + informatics >= 150 &&
            math >= 50 && informatics >= 50)
            Console.WriteLine($"Абитуриент зачислен");
        else
            Console.WriteLine($"Абитуриент не зачислен");
    }
}
```

> * №137. Проверить, лежит ли точка с координатами (X,Y) в круговом кольце с внутренним радиусом R1 и внешним R2.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите X: ");
        double x = double.Parse(Console.ReadLine());

        Console.Write("Введите Y: ");
        double y = double.Parse(Console.ReadLine());

        Console.Write("Введите R1: ");
        double r1 = double.Parse(Console.ReadLine());

        Console.Write("Введите R2: ");
        double r2 = double.Parse(Console.ReadLine());

        double distance = x * x + y * y;

        if (distance >= r1 * r1 && distance <= r2 * r2)
            Console.WriteLine($"Точка находится в кольце");
        else
            Console.WriteLine($"Точка не находится в кольце");
    }
}
```

> * №138. Ввести статус билета (true/false) и наличие багажа. Вывести: требуется ли дополнительная оплата багажа.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Билет действителен? ");
        bool ticket = bool.Parse(Console.ReadLine());

        Console.Write("Есть багаж? ");
        bool baggage = bool.Parse(Console.ReadLine());

        if (ticket && baggage)
            Console.WriteLine($"Требуется дополнительная оплата багажа");
        else
            Console.WriteLine($"Дополнительная оплата не требуется");
    }
}
```

> * №139. Дано четырехзначное число. Проверить, читается ли оно одинаково слева направо и справа налево (палиндром).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите четырехзначное число: ");
        int number = int.Parse(Console.ReadLine());

        int a = number / 1000;
        int b = number / 100 % 10;
        int c = number / 10 % 10;
        int d = number % 10;

        if (a == d && b == c)
            Console.WriteLine($"Число является палиндромом");
        else
            Console.WriteLine($"Число не является палиндромом");
    }
}
```

> * №140. Ввести напряжение сети (Вольты) и частоту (Гц). Норма: 220 В±10 И частота 50 Гц±1 Гц. Вывести статус стабильности сети.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите напряжение: ");
        double voltage = double.Parse(Console.ReadLine());

        Console.Write("Введите частоту: ");
        double chast = double.Parse(Console.ReadLine());

        if (voltage >= 210 && voltage <= 230 &&
            chast >= 49 && chast <= 51)
            Console.WriteLine($"Сеть стабильна");
        else
            Console.WriteLine($"Сеть нестабильна");
    }
}
```

> * №141. Ввести признак наличия прав (bool), страховки (bool) и трезвости водителя (bool). Разрешить выезд только при соблюдении всех трех факторов.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Есть права? ");
        bool license = bool.Parse(Console.ReadLine());

        Console.Write("Есть страховка? ");
        bool strahovka = bool.Parse(Console.ReadLine());

        Console.Write("Водитель трезв? ");
        bool trezv = bool.Parse(Console.ReadLine());

        if (license && strahovka && trezv)
            Console.WriteLine($"Выезд разрешен");
        else
            Console.WriteLine($"Выезд запрещен");
    }
}
```

> * №142. Проверить, делится ли введенное число на 4 ИЛИ на 7, но НЕ делится на 28.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите число: ");
        int number = int.Parse(Console.ReadLine());

        if ((number % 4 == 0 || number % 7 == 0) &&
            number % 28 != 0)
            Console.WriteLine($"Условие выполнено");
        else
            Console.WriteLine($"Условие не выполнено");
    }
}
```

> * №143. Ввести текущий месяц и температуру. Вывести аномалию, если месяц летний (6, 7, 8), а температура ниже нуля.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите месяц: ");
        int month = int.Parse(Console.ReadLine());

        Console.Write("Введите температуру: ");
        int temperature = int.Parse(Console.ReadLine());

        if ((month == 6 || month == 7 || month == 8) &&
            temperature < 0)
            Console.WriteLine($"Обнаружена аномалия");
        else
            Console.WriteLine($"Аномалии нет");
    }
}
```

> * №144. Даны три логические переменные A, B, C. Реализовать проверку формулы мажоритарного клапана: «Истинно, если хотя бы две из трех переменных истинны».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите A: ");
        bool A = bool.Parse(Console.ReadLine());

        Console.Write("Введите B: ");
        bool B = bool.Parse(Console.ReadLine());

        Console.Write("Введите C: ");
        bool C = bool.Parse(Console.ReadLine());

        if ((A && B) || (A && C) || (B && C))
            Console.WriteLine($"Истинно");
        else
            Console.WriteLine($"Ложно");
    }
}
```

> * №145. Даны три вещественных числа. Проверить, могут ли они являться длинами сторон тупоугольного треугольника.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите a: ");
        double a = double.Parse(Console.ReadLine());

        Console.Write("Введите b: ");
        double b = double.Parse(Console.ReadLine());

        Console.Write("Введите c: ");
        double c = double.Parse(Console.ReadLine());

        if (a + b > c && a + c > b && b + c > a)
        {
            if (a * a + b * b < c * c ||
                a * a + c * c < b * b ||
                b * b + c * c < a * a)
                Console.WriteLine($"Треугольник тупоугольный");
            else
                Console.WriteLine($"Треугольник не тупоугольный");
        }
        else
            Console.WriteLine($"Это не треугольник");
    }
}
```

> * №146. Даны три вещественных числа. Проверить, могут ли они являться длинами сторон остроугольного треугольника.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите a: ");
        double a = double.Parse(Console.ReadLine());

        Console.Write("Введите b: ");
        double b = double.Parse(Console.ReadLine());

        Console.Write("Введите c: ");
        double c = double.Parse(Console.ReadLine());

        if (a + b > c && a + c > b && b + c > a &&
            a * a + b * b > c * c &&
            a * a + c * c > b * b &&
            b * b + c * c > a * a)
            Console.WriteLine($"Треугольник остроугольный");
        else
            Console.WriteLine($"Треугольник не остроугольный");
    }
}
```

> * №147. Ввести время (часы и минуты). Проверить, попадает ли указанное время в интервал тихого часа (с 13:00 до 15:00).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите часы: ");
        int hours = int.Parse(Console.ReadLine());

        Console.Write("Введите минуты: ");
        int minutes = int.Parse(Console.ReadLine());

        int time = hours * 60 + minutes;

        if (time >= 13 * 60 && time <= 15 * 60)
            Console.WriteLine($"Сейчас тихий час");
        else
            Console.WriteLine($"Сейчас не тихий час");
    }
}
```

> * №148. Проверить, что все цифры введенного трехзначного числа различны между собой.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите трехзначное число: ");
        int number = int.Parse(Console.ReadLine());

        if (number >= 100 && number <= 999)
        {
            int a = number / 100;
            int b = number / 10 % 10;
            int c = number % 10;

            if (a != b && a != c && b != c)
            {
                Console.WriteLine($"Все цифры разные.");
            }
            else
            {
                Console.WriteLine($"Есть одинаковые цифры.");
            }
        }
        else
        {
            Console.WriteLine($"Ошибка: нужно ввести только трехзначное число.");
        }
    }
}
```

> * №149. Ввести логическое значение двух кнопок пульта. Станок запускается только при одновременном зажатии обеих кнопок (защита от случайного пуска).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Первая кнопка нажата? ");
        bool button1 = bool.Parse(Console.ReadLine());

        Console.Write("Вторая кнопка нажата? ");
        bool button2 = bool.Parse(Console.ReadLine());

        if (button1 && button2)
            Console.WriteLine($"Станок запускается");
        else
            Console.WriteLine($"Станок не запускается");
    }
}
```

> * №150. Проверить, лежит ли точка (X,Y) ниже прямой Y=2X+1 и выше параболы Y=X2.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите X: ");
        double x = double.Parse(Console.ReadLine());

        Console.Write("Введите Y: ");
        double y = double.Parse(Console.ReadLine());

        if (y < 2 * x + 1 && y > x * x)
            Console.WriteLine($"Точка находится в нужной области");
        else
            Console.WriteLine($"Точка не находится в нужной области");
    }
}
```
---
### Раздел 4. Оператор выбора switch
---

> * №151. Ввести номер дня недели (1–7). Вывести его словесное название на русском языке.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер дня: ");
        int day = int.Parse(Console.ReadLine());

        switch (day)
        {
            case 1: Console.WriteLine($"Понедельник"); break;
            case 2: Console.WriteLine($"Вторник"); break;
            case 3: Console.WriteLine($"Среда"); break;
            case 4: Console.WriteLine($"Четверг"); break;
            case 5: Console.WriteLine($"Пятница"); break;
            case 6: Console.WriteLine($"Суббота"); break;
            case 7: Console.WriteLine($"Воскресенье"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №152. Ввести номер дня недели (1–7). Вывести, является ли день рабочим («Будни») или нерабочим («Выходной»).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер дня: ");
        int day = int.Parse(Console.ReadLine());

        switch (day)
        {
            case 1:
            case 2:
            case 3:
            case 4:
            case 5:
                Console.WriteLine($"Будни");
                break;

            case 6:
            case 7:
                Console.WriteLine($"Выходной");
                break;

            default:
                Console.WriteLine($"Ошибка");
                break;
        }
    }
}
```

> * №153. Ввести номер месяца (1–12). Вывести название месяца.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер месяца: ");
        int month = int.Parse(Console.ReadLine());

        switch (month)
        {
            case 1: Console.WriteLine($"Январь"); break;
            case 2: Console.WriteLine($"Февраль"); break;
            case 3: Console.WriteLine($"Март"); break;
            case 4: Console.WriteLine($"Апрель"); break;
            case 5: Console.WriteLine($"Май"); break;
            case 6: Console.WriteLine($"Июнь"); break;
            case 7: Console.WriteLine($"Июль"); break;
            case 8: Console.WriteLine($"Август"); break;
            case 9: Console.WriteLine($"Сентябрь"); break;
            case 10: Console.WriteLine($"Октябрь"); break;
            case 11: Console.WriteLine($"Ноябрь"); break;
            case 12: Console.WriteLine($"Декабрь"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №154. Ввести номер месяца (1–12). Вывести количество дней в этом месяце (для невисокосного года).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер месяца: ");
        int month = int.Parse(Console.ReadLine());

        switch (month)
        {
            case 2:
                Console.WriteLine($"28 дней");
                break;

            case 4:
            case 6:
            case 9:
            case 11:
                Console.WriteLine($"30 дней");
                break;

            case 1:
            case 3:
            case 5:
            case 7:
            case 8:
            case 10:
            case 12:
                Console.WriteLine($"31 день");
                break;

            default:
                Console.WriteLine($"Ошибка");
                break;
        }
    }
}
```

> * №155. Ввести номер месяца (1–12). Вывести название поры года («Зима», «Весна», «Лето», «Осень»).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер месяца: ");
        int month = int.Parse(Console.ReadLine());

        switch (month)
        {
            case 12:
            case 1:
            case 2:
                Console.WriteLine($"Зима");
                break;

            case 3:
            case 4:
            case 5:
                Console.WriteLine($"Весна");
                break;

            case 6:
            case 7:
            case 8:
                Console.WriteLine($"Лето");
                break;

            case 9:
            case 10:
            case 11:
                Console.WriteLine($"Осень");
                break;

            default:
                Console.WriteLine($"Ошибка");
                break;
        }
    }
}
```

> * №156. Ввести оценку студента (1–5). Вывести текстовое описание: 1 — «Очень плохо», 2 — «Неудовлетворительно», 3 — «Удовлетворительно», 4 — «Хорошо», 5 — «Отлично».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите оценку: ");
        int grade = int.Parse(Console.ReadLine());

        switch (grade)
        {
            case 1: Console.WriteLine($"Очень плохо"); break;
            case 2: Console.WriteLine($"Неудовлетворительно"); break;
            case 3: Console.WriteLine($"Удовлетворительно"); break;
            case 4: Console.WriteLine($"Хорошо"); break;
            case 5: Console.WriteLine($"Отлично"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №157. Реализовать простой калькулятор: ввести два вещественных числа и символ арифметической операции (+, -, *, /). Через switch выполнить вычисление. Предусмотреть защиту от деления на ноль.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите первое число: ");
        double a = double.Parse(Console.ReadLine());

        Console.Write("Введите второе число: ");
        double b = double.Parse(Console.ReadLine());

        Console.Write("Введите операцию: ");
        char operation = char.Parse(Console.ReadLine());

        switch (operation)
        {
            case '+':
                Console.WriteLine($"{a + b}");
                break;

            case '-':
                Console.WriteLine($"{a - b}");
                break;

            case '*':
                Console.WriteLine($"{a * b}");
                break;

            case '/':
                if (b != 0)
                    Console.WriteLine($"{a / b}");
                else
                    Console.WriteLine($"На ноль делить нельзя");
                break;

            default:
                Console.WriteLine($"Ошибка");
                break;
        }
    }
}
```

> * №158. Ввести букву направления света (N, S, W, E). Вывести название направления («Север», «Юг», «Запад», «Восток»).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите направление: ");
        char napravlenie = char.Parse(Console.ReadLine().ToUpper());

        switch (napravlenie)
        {
            case 'N': Console.WriteLine($"Север"); break;
            case 'S': Console.WriteLine($"Юг"); break;
            case 'W': Console.WriteLine($"Запад"); break;
            case 'E': Console.WriteLine($"Восток"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №159. Ввести номер геометрической фигуры (1 — круг, 2 — прямоугольник, 3 — треугольник). Запросить соответствующие параметры фигуры и вычислить ее площадь.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine($"1. Круг");
        Console.WriteLine($"2. Прямоугольник");
        Console.WriteLine($"3. Треугольник");

        Console.Write("Выберите фигуру: ");
        int choice = int.Parse(Console.ReadLine());

        switch (choice)
        {
            case 1:
                Console.Write("Введите радиус: ");
                double r = double.Parse(Console.ReadLine());
                Console.WriteLine($"{Math.PI * r * r}");
                break;

            case 2:
                Console.Write("Введите длину: ");
                double a = double.Parse(Console.ReadLine());

                Console.Write("Введите ширину: ");
                double b = double.Parse(Console.ReadLine());

                Console.WriteLine($"{a * b}");
                break;

            case 3:
                Console.Write("Введите основание: ");
                double c = double.Parse(Console.ReadLine());

                Console.Write("Введите высоту: ");
                double h = double.Parse(Console.ReadLine());

                Console.WriteLine($"{c * h / 2}");
                break;

            default:
                Console.WriteLine($"Ошибка");
                break;
        }
    }
}
```

> * №160. Ввести номер масти игральной карты (1 — пики, 2 — трефы, 3 — бубны, 4 — червы). Вывести название масти.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер масти: ");
        int mast = int.Parse(Console.ReadLine());

        switch (mast)
        {
            case 1: Console.WriteLine($"Пики"); break;
            case 2: Console.WriteLine($"Трефы"); break;
            case 3: Console.WriteLine($"Бубны"); break;
            case 4: Console.WriteLine($"Червы"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №161. Ввести достоинство карты (числа от 6 до 14). Вывести название: 11 — Валет, 12 — Дама, 13 — Король, 14 — Туз, остальные — по номиналу.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите достоинство карты: ");
        int card = int.Parse(Console.ReadLine());

        switch (card)
        {
            case 11: Console.WriteLine($"Валет"); break;
            case 12: Console.WriteLine($"Дама"); break;
            case 13: Console.WriteLine($"Король"); break;
            case 14: Console.WriteLine($"Туз"); break;
            case 6:
            case 7:
            case 8:
            case 9:
            case 10:
                Console.WriteLine($"{card}");
                break;
            default:
                Console.WriteLine($"Ошибка");
                break;
        }
    }
}
```

> * №162. Ввести буквенное обозначение размера одежды (XS, S, M, L, XL, XXL). Вывести соответствующий российский размер (42, 44, 46, 48, 50, 52).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите буквенное обозначение размера одежды: ");
        string size = Console.ReadLine().ToUpper();

        switch (size)
        {
            case "XS": Console.WriteLine($"42"); break;
            case "S": Console.WriteLine($"44"); break;
            case "M": Console.WriteLine($"46"); break;
            case "L": Console.WriteLine($"48"); break;
            case "XL": Console.WriteLine($"50"); break;
            case "XXL":Console.WriteLine($"52"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №163. Ввести номер единицы длины (1 — дециметр, 2 — километр, 3 — метр, 4 — миллиметр, 5 — сантиметр) и длину отрезка в этих единицах. Перевести и вывести длину в метрах.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine($"1 — дециметр");
        Console.WriteLine($"2 — километр");
        Console.WriteLine($"3 — метр");
        Console.WriteLine($"4 — миллиметр");
        Console.WriteLine($"5 — сантиметр");


        Console.Write("Введите номер единицы длины: ");
        int edinica = int.Parse(Console.ReadLine());

        Console.Write("Введите длину: ");
        double value = double.Parse(Console.ReadLine());

        switch (edinica)
        {
            case 1: Console.WriteLine($"{value / 10}"); break;
            case 2: Console.WriteLine($"{value * 1000}"); break;
            case 3: Console.WriteLine($"{value}"); break;
            case 4: Console.WriteLine($"{value / 1000}"); break;
            case 5: Console.WriteLine($"{value / 100}"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №164. Ввести номер единицы массы (1 — килограмм, 2 — миллиграмм, 3 — грамм, 4 — тонна, 5 — центнер) и массу. Вывести массу в килограммах.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine($"1 — килограмм");
        Console.WriteLine($"2 — миллиграмм");
        Console.WriteLine($"3 — грамм");
        Console.WriteLine($"4 — тонна");
        Console.WriteLine($"5 — центнер");


        Console.Write("Введите номер единицы массы: ");
        int massa = int.Parse(Console.ReadLine());

        Console.Write("Введите массу: ");
        double value = double.Parse(Console.ReadLine());

        switch (massa)
        {
            case 1: Console.WriteLine($"{value}"); break;
            case 2: Console.WriteLine($"{value / 1000000}"); break;
            case 3: Console.WriteLine($"{value / 1000}"); break;
            case 4: Console.WriteLine($"{value * 1000}"); break;
            case 5: Console.WriteLine($"{value * 100}"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №165. Ввести код ошибки HTTP (200, 301, 400, 403, 404, 500, 502). Вывести текстовую расшифровку статуса.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите HTTP-код: ");
        int code = int.Parse(Console.ReadLine());

        switch (code)
        {
            case 200: Console.WriteLine($"Успешный запрос"); break;
            case 301: Console.WriteLine($"Перенаправление"); break;
            case 400: Console.WriteLine($"Неверный запрос"); break;
            case 403: Console.WriteLine($"Доступ запрещен"); break;
            case 404: Console.WriteLine($"Страница не найдена"); break;
            case 500: Console.WriteLine($"Ошибка сервера"); break;
            case 502: Console.WriteLine($"Ошибка шлюза"); break;
            default: Console.WriteLine($"Неизвестный код"); break;
        }
    }
}
```

> * №166. Ввести код валюты (USD, EUR, CNY, RUB). Вывести полное наименование («Доллар США», «Евро», «Китайский юань», «Российский рубль»).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите код валюты: ");
        string name = Console.ReadLine().ToUpper();

        switch (name)
        {
            case "USD": Console.WriteLine($"Доллар США"); break;
            case "EUR": Console.WriteLine($"Евро"); break;
            case "CNY": Console.WriteLine($"Китайский юань"); break;
            case "RUB": Console.WriteLine($"Российский рубль"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №167. Ввести символ клавиши управления движением персонажа (W, A, S, D в любом регистре). Вывести направление движения: вперед, влево, назад, вправо.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите клавишу: ");
        char simv = char.Parse(Console.ReadLine().ToUpper());

        switch (simv)
        {
            case 'W': Console.WriteLine($"Вперед"); break;
            case 'A': Console.WriteLine($"Влево"); break;
            case 'S': Console.WriteLine($"Назад"); break;
            case 'D': Console.WriteLine($"Вправо"); break;
            default: Console.WriteLine($"Неизвестная клавиша"); break;
        }
    }
}
```

> * №168. Ввести номер цвета радуги (1–7). Вывести название цвета.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер цвета радуги: ");
        int color = int.Parse(Console.ReadLine());

        switch (color)
        {
            case 1: Console.WriteLine($"Красный"); break;
            case 2: Console.WriteLine($"Оранжевый"); break;
            case 3: Console.WriteLine($"Желтый"); break;
            case 4: Console.WriteLine($"Зеленый"); break;
            case 5: Console.WriteLine($"Голубой"); break;
            case 6: Console.WriteLine($"Синий"); break;
            case 7: Console.WriteLine($"Фиолетовый"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №169. Ввести признак режима селектора АКПП (P, R, N, D, M). Вывести режим трансмиссии.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите признак режима селектора АКПП: ");
        char mode = char.Parse(Console.ReadLine().ToUpper());

        switch (mode)
        {
            case 'P': Console.WriteLine($"Парковка"); break;
            case 'R': Console.WriteLine($"Задний ход"); break;
            case 'N': Console.WriteLine($"Нейтраль"); break;
            case 'D': Console.WriteLine($"Движение вперед"); break;
            case 'M': Console.WriteLine($"Ручной режим"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №170. Ввести номер пальца руки (1 — большой, 2 — указательный, 3 — средний, 4 — безымянный, 5 — мизинец). Вывести название пальца.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер пальца: ");
        int finger = int.Parse(Console.ReadLine());

        switch (finger)
        {
            case 1: Console.WriteLine($"Большой"); break;
            case 2: Console.WriteLine($"Указательный"); break;
            case 3: Console.WriteLine($"Средний"); break;
            case 4: Console.WriteLine($"Безымянный"); break;
            case 5: Console.WriteLine($"Мизинец"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №171. Ввести номер планеты от Солнца (1–8). Вывести название планеты Солнечной системы.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер планеты от Солнца: ");
        int planet = int.Parse(Console.ReadLine());

        switch (planet)
        {
            case 1: Console.WriteLine($"Меркурий"); break;
            case 2: Console.WriteLine($"Венера"); break;
            case 3: Console.WriteLine($"Земля"); break;
            case 4: Console.WriteLine($"Марс"); break;
            case 5: Console.WriteLine($"Юпитер"); break;
            case 6: Console.WriteLine($"Сатурн"); break;
            case 7: Console.WriteLine($"Уран"); break;
            case 8: Console.WriteLine($"Нептун"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №172. Ввести код тарифа мобильной связи (1 — Базовый, 2 — Студенческий, 3 — Безлимит). Вывести абонентскую плату и включенные гигабайты.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine($"1 — Базовый");
        Console.WriteLine($"2 — Студенческий");
        Console.WriteLine($"3 — Безлимит");

        Console.Write("Введите номер тарифа: ");
        int tariff = int.Parse(Console.ReadLine());

        switch (tariff)
        {
            case 1:
                Console.WriteLine($"Базовый: 300 рублей, 10 ГБ");
                break;

            case 2:
                Console.WriteLine($"Студенческий: 200 рублей, 20 ГБ");
                break;

            case 3:
                Console.WriteLine($"Безлимит: 600 рублей, безлимитный интернет");
                break;

            default:
                Console.WriteLine($"Ошибка");
                break;
        }
    }
}
```

> * №173. Ввести номер квартала года (1–4). Вывести список входящих в него месяцев.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер квартала: ");
        int quarter = int.Parse(Console.ReadLine());

        switch (quarter)
        {
            case 1:
                Console.WriteLine($"Январь, Февраль, Март");
                break;

            case 2:
                Console.WriteLine($"Апрель, Май, Июнь");
                break;

            case 3:
                Console.WriteLine($"Июль, Август, Сентябрь");
                break;

            case 4:
                Console.WriteLine($"Октябрь, Ноябрь, Декабрь");
                break;

            default:
                Console.WriteLine($"Ошибка");
                break;
        }
    }
}
```

> * №174. Ввести букву оценки американской системы (A, B, C, D, F). Вывести эквивалент в пятибалльной системе РФ.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите букву оценки американской системы: ");
        char grade = char.Parse(Console.ReadLine().ToUpper());

        switch (grade)
        {
            case 'A': Console.WriteLine($"5"); break;
            case 'B': Console.WriteLine($"4"); break;
            case 'C': Console.WriteLine($"3"); break;
            case 'D': Console.WriteLine($"2"); break;
            case 'F': Console.WriteLine($"1"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №175. Ввести символ операции над множествами (U — объединение, I — пересечение, D — разность). Вывести расшифровку операции.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите символ операции над множествами: ");
        char operation = char.Parse(Console.ReadLine().ToUpper());

        switch (operation)
        {
            case 'U': Console.WriteLine($"Объединение"); break;
            case 'I': Console.WriteLine($"Пересечение"); break;
            case 'D': Console.WriteLine($"Разность"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №176. Ввести номер режима работы светофора (1 — Красный, 2 — Желтый, 3 — Зеленый, 4 — Мигающий желтый). Вывести предписание для водителя.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер режима: ");
        int mode = int.Parse(Console.ReadLine());

        switch (mode)
        {
            case 1: Console.WriteLine($"Красный — остановиться"); break;
            case 2: Console.WriteLine($"Желтый — приготовиться"); break;
            case 3: Console.WriteLine($"Зеленый — можно ехать"); break;
            case 4: Console.WriteLine($"Мигающий желтый — двигаться осторожно"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №177. Ввести цифру (0–9). Вывести ее словесное написание на русском языке.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите цифру: ");
        int number = int.Parse(Console.ReadLine());

        switch (number)
        {
            case 0: Console.WriteLine($"Ноль"); break;
            case 1: Console.WriteLine($"Один"); break;
            case 2: Console.WriteLine($"Два"); break;
            case 3: Console.WriteLine($"Три"); break;
            case 4: Console.WriteLine($"Четыре"); break;
            case 5: Console.WriteLine($"Пять"); break;
            case 6: Console.WriteLine($"Шесть"); break;
            case 7: Console.WriteLine($"Семь"); break;
            case 8: Console.WriteLine($"Восемь"); break;
            case 9: Console.WriteLine($"Девять"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №178. Ввести римскую цифру (I, V, X, L, C, D, M). Вывести ее арабское значение.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите римскую цифру: ");
        char rim = char.Parse(Console.ReadLine().ToUpper());

        switch (rim)
        {
            case 'I': Console.WriteLine($"1"); break;
            case 'V': Console.WriteLine($"5"); break;
            case 'X': Console.WriteLine($"10"); break;
            case 'L': Console.WriteLine($"50"); break;
            case 'C': Console.WriteLine($"100"); break;
            case 'D': Console.WriteLine($"500"); break;
            case 'M': Console.WriteLine($"1000"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №179. Ввести номер типа транспортного средства (1 — Мотоцикл, 2 — Легковой авто, 3 — Грузовой авто, 4 — Автобус). Вывести категорию водительского удостоверения (A, B, C, D).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine($"1 — Мотоцикл");
        Console.WriteLine($"2 — Легковой авто");
        Console.WriteLine($"3 — Грузовой авто");
        Console.WriteLine($"4 — Автобус");

        Console.Write("Введите номер транспорта: ");
        int transport = int.Parse(Console.ReadLine());

        switch (transport)
        {
            case 1: Console.WriteLine($"Мотоцикл — категория A"); break;
            case 2: Console.WriteLine($"Легковой авто — категория B"); break;
            case 3: Console.WriteLine($"Грузовой авто — категория C"); break;
            case 4: Console.WriteLine($"Автобус — категория D"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №180. Ввести тип двигателя (1 — Бензиновый, 2 — Дизельный, 3 — Гибридный, 4 — Электрический). Вывести вид используемого источника энергии.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine($"1 — Бензиновый");
        Console.WriteLine($"2 — Дизельный");
        Console.WriteLine($"3 — Гибридный");
        Console.WriteLine($"4 — Электрический");

        Console.Write("Введите номер двигателя: ");
        int engine = int.Parse(Console.ReadLine());

        switch (engine)
        {
            case 1: Console.WriteLine($"Бензиновый — бензин"); break;
            case 2: Console.WriteLine($"Дизельный — дизельное топливо"); break;
            case 3: Console.WriteLine($"Гибридный — топливо и электричество"); break;
            case 4: Console.WriteLine($"Электрический — электрическая энергия"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №181. Ввести номер операции в банкомате: 1 — Баланс, 2 — Снятие наличных, 3 — Пополнение, 4 — Перевод. Вывести сообщение о начале выбранной процедуры.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер операции: ");
        int operation = int.Parse(Console.ReadLine());

        switch (operation)
        {
            case 1: Console.WriteLine($"Начинается проверка баланса."); break;
            case 2: Console.WriteLine($"Начинается снятие наличных."); break;
            case 3: Console.WriteLine($"Начинается пополнение счета."); break;
            case 4: Console.WriteLine($"Начинается перевод."); break;
            default: Console.WriteLine($"Ошибка."); break;
        }
    }
}
```

> * №182. Ввести расширение файла (txt, cs, html, png, mp3). Вывести тип содержимого: текстовый документ, исходный код C#, веб-страница, изображение, аудиофайл.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите расширение файла: ");
        string file = Console.ReadLine();

        switch (file)
        {
            case "txt": Console.WriteLine($"Текстовый документ"); break;
            case "cs": Console.WriteLine($"Исходный код C#"); break;
            case "html": Console.WriteLine($"Веб-страница"); break;
            case "png": Console.WriteLine($"Изображение"); break;
            case "mp3": Console.WriteLine($"Аудиофайл"); break;
            default: Console.WriteLine($"Неизвестный тип файла"); break;
        }
    }
}
```

> * №183. Ввести номер химического элемента из первых пяти таблицы Менделеева (1–5). Вывести название элемента и его символ.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер элемента: ");
        int number = int.Parse(Console.ReadLine());

        switch (number)
        {
            case 1: Console.WriteLine($"Водород H"); break;
            case 2: Console.WriteLine($"Гелий He"); break;
            case 3: Console.WriteLine($"Литий Li"); break;
            case 4: Console.WriteLine($"Бериллий Be"); break;
            case 5: Console.WriteLine($"Бор B"); break;
            default: Console.WriteLine($"Ошибка."); break;
        }
    }
}
```

> * №184. Ввести код статуса заказа в интернет-магазине (NEW, PAID, SHIPPED, DELIVERED, CANCELED). Вывести подсказку для клиента.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите статус заказа: ");
        string status = Console.ReadLine().ToUpper();

        switch (status)
        {
            case "NEW": Console.WriteLine($"Заказ принят и ожидает обработки."); break;
            case "PAID": Console.WriteLine($"Заказ оплачен."); break;
            case "SHIPPED": Console.WriteLine($"Заказ отправлен."); break;
            case "DELIVERED": Console.WriteLine($"Заказ доставлен."); break;
            case "CANCELED": Console.WriteLine($"Заказ отменен."); break;
            default: Console.WriteLine($"Неизвестный статус."); break;
        }
    }
}
```

> * №185. Ввести код системы счисления (2, 8, 10, 16) и перевести введенное десятичное число в выбранную систему (через методы класса Convert).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите десятичное число: ");
        int number = int.Parse(Console.ReadLine());

        Console.Write("Введите систему счисления: ");
        int system = int.Parse(Console.ReadLine());

        switch (system)
        {
            case 2: Console.WriteLine($"{Convert.ToString(number, 2)}"); break;
            case 8: Console.WriteLine($"{Convert.ToString(number, 8)}"); break;
            case 10: Console.WriteLine($"{Convert.ToString(number, 10)}"); break;
            case 16: Console.WriteLine($"{Convert.ToString(number, 16)}"); break;
            default: Console.WriteLine($"Ошибка."); break;
        }
    }
}
```

> * №186. Ввести номер курса колледжа (1–4). Вывести: «Первокурсник», «Второй курс», «Предвыпускной курс», «Выпускник».

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер курса: ");
        int course = int.Parse(Console.ReadLine());

        switch (course)
        {
            case 1: Console.WriteLine($"Первокурсник"); break;
            case 2: Console.WriteLine($"Второй курс"); break;
            case 3: Console.WriteLine($"Предвыпускной курс"); break;
            case 4: Console.WriteLine($"Выпускник"); break;
            default: Console.WriteLine($"Ошибка."); break;
        }
    }
}
```

> * №187. Ввести код климатической зоны (1 — Арктическая, 2 — Субарктическая, 3 — Умеренная, 4 — Субтропическая, 5 — Тропическая). Вывести краткую характеристику.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите код зоны: ");
        int zone = int.Parse(Console.ReadLine());

        switch (zone)
        {
            case 1: Console.WriteLine($"Арктическая — очень холодный климат"); break;
            case 2: Console.WriteLine($"Субарктическая — холодная зима и прохладное лето"); break;
            case 3: Console.WriteLine($"Умеренная — смена времен года"); break;
            case 4: Console.WriteLine($"Субтропическая — теплый климат"); break;
            case 5: Console.WriteLine($"Тропическая — жаркий климат"); break;
            default: Console.WriteLine($"Ошибка."); break;
        }
    }
}
```

> * №188. Ввести класс пожарной опасности (1–5). Вывести уровень угрозы и ограничения на посещение лесов.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите класс пожарной опасности: ");
        int danger = int.Parse(Console.ReadLine());

        switch (danger)
        {
            case 1: Console.WriteLine($"Уровень низкий. Ограничений нет"); break;
            case 2: Console.WriteLine($"Уровень умеренный. Соблюдайте осторожность"); break;
            case 3: Console.WriteLine($"Уровень высокий. Посещение лесов ограничено"); break;
            case 4: Console.WriteLine($"Уровень очень высокий. Посещение лесов запрещено"); break;
            case 5: Console.WriteLine($"Уровень чрезвычайный. Посещение лесов запрещено"); break;
            default: Console.WriteLine($"Ошибка."); break;
        }
    }
}
```

> * №189. Ввести номер спортивного разряда (1 — Юношеский, 2 — Взрослый, 3 — КМС, 4 — МС, 5 — МСМК). Вывести расшифровку.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер разряда: ");
        int razryad = int.Parse(Console.ReadLine());

        switch (razryad)
        {
            case 1: Console.WriteLine($"Юношеский разряд"); break;
            case 2: Console.WriteLine($"Взрослый разряд"); break;
            case 3: Console.WriteLine($"КМС - Кандидат в мастера спорта"); break;
            case 4: Console.WriteLine($"МС - Мастер спорта"); break;
            case 5: Console.WriteLine($"МСМК - Мастер спорта международного класса"); break;
            default: Console.WriteLine($"Ошибка."); break;
        }
    }
}
```

> * №190. Ввести код уровня доступа пользователя (G — Guest, U — User, M — Moderator, A — Administrator). Вывести перечень разрешенных действий.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите код доступа: ");
        char dostup = char.Parse(Console.ReadLine().ToUpper());

        switch (dostup)
        {
            case 'G': Console.WriteLine($"Guest — просмотр общедоступной информации."); break;
            case 'U': Console.WriteLine($"User — работа с обычными функциями."); break;
            case 'M': Console.WriteLine($"Moderator — управление контентом."); break;
            case 'A': Console.WriteLine($"Administrator — полный доступ."); break;
            default: Console.WriteLine($"Ошибка."); break;
        }
    }
}
```

> * №191. Ввести букву ноты (C, D, E, F, G, A, B). Вывести русское словесное обозначение (До, Ре, Ми, Фа, Соль, Ля, Си).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите букву ноты: ");
        char note = char.Parse(Console.ReadLine().ToUpper());

        switch (note)
        {
            case 'C': Console.WriteLine($"До"); break;
            case 'D': Console.WriteLine($"Ре"); break;
            case 'E': Console.WriteLine($"Ми"); break;
            case 'F': Console.WriteLine($"Фа"); break;
            case 'G': Console.WriteLine($"Соль"); break;
            case 'A': Console.WriteLine($"Ля"); break;
            case 'B': Console.WriteLine($"Си"); break;
            default: Console.WriteLine($"Ошибка."); break;
        }
    }
}
```

> * №192. Ввести номер типа кузова автомобиля (1 — Седан, 2 — Хэтчбек, 3 — Универсал, 4 — Купе, 5 — Внедорожник). Вывести описание вместимости и компоновки.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер кузова: ");
        int kuzov = int.Parse(Console.ReadLine());

        switch (kuzov)
        {
            case 1: Console.WriteLine($"Седан — отдельный багажник, обычно 4 двери"); break;
            case 2: Console.WriteLine($"Хэтчбек — багажник объединен с салоном"); break;
            case 3: Console.WriteLine($"Универсал — большой багажник и просторный салон"); break;
            case 4: Console.WriteLine($"Купе — обычно две двери и спортивная компоновка"); break;
            case 5: Console.WriteLine($"Внедорожник — высокий кузов и большой салон"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №193. Ввести код типа датчика охранной сигнализации: M (движение), D (открытие двери), S (дым), W (протечка воды). Вывести сообщение о типе угрозы.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите код датчика охранной сигнализации: ");
        char sensor = char.Parse(Console.ReadLine().ToUpper());

        switch (sensor)
        {
            case 'M': Console.WriteLine($"Обнаружено движение"); break;
            case 'D': Console.WriteLine($"Обнаружено открытие двери"); break;
            case 'S': Console.WriteLine($"Обнаружен дым"); break;
            case 'W': Console.WriteLine($"Обнаружена протечка воды"); break;
            default: Console.WriteLine($"Неизвестный датчик"); break;
        }
    }
}
```

> * №194. Ввести номер фазы Луны (1 — Новолуние, 2 — Первая четверть, 3 — Полнолуние, 4 — Последняя четверть). Вывести характеристику фазы.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер фазы Луны: ");
        int phase = int.Parse(Console.ReadLine());

        switch (phase)
        {
            case 1: Console.WriteLine($"Новолуние - Луна почти не видна"); break;
            case 2: Console.WriteLine($"Первая четверть — видна половина Луны"); break;
            case 3: Console.WriteLine($"Полнолуние — виден весь диск Луны"); break;
            case 4: Console.WriteLine($"Последняя четверть - видна половина Луны"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №195. Ввести символ разделителя пути в операционной системе (/ или \). Вывести, к какому семейству ОС относится разделитель (Unix/Linux или Windows).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите разделитель пути: ");
        string razdelitel = Console.ReadLine();

        switch (razdelitel)
        {
            case "/": Console.WriteLine($"Unix/Linux"); break;
            case "\\": Console.WriteLine($"Windows"); break;
            default: Console.WriteLine($"Неизвестный разделитель."); break;
        }
    }
}
```

> * №196. Ввести номер поколения мобильной связи (2, 3, 4, 5). Вывести название стандарта (GPRS/EDGE, UMTS/HSPA, LTE, NR) и типичную скорость.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите поколение связи: ");
        int pokolenie = int.Parse(Console.ReadLine());

        switch (pokolenie)
        {
            case 2: Console.WriteLine($"GPRS/EDGE — низкая скорость"); break;
            case 3: Console.WriteLine($"UMTS/HSPA — средняя скорость"); break;
            case 4: Console.WriteLine($"LTE — высокая скорость"); break;
            case 5: Console.WriteLine($"NR — очень высокая скорость"); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №197. Ввести номер порта протокола (21, 22, 25, 80, 443). Вывести название сетевого протокола (FTP, SSH, SMTP, HTTP, HTTPS).

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите номер порта протокола: ");
        int port = int.Parse(Console.ReadLine());

        switch (port)
        {
            case 21: Console.WriteLine($"FTP"); break;
            case 22: Console.WriteLine($"SSH"); break;
            case 25: Console.WriteLine($"SMTP"); break;
            case 80: Console.WriteLine($"HTTP"); break;
            case 443: Console.WriteLine($"HTTPS"); break;
            default: Console.WriteLine($"Неизвестный порт."); break;
        }
    }
}
```

> * №198. Ввести код режима стиральной машины (1 — Хлопок, 2 — Синтетика, 3 — Шерсть, 4 — Быстрая 15 мин, 5 — Отжим). Вывести температуру стирки и скорость отжима.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите код режима стиральной машины: ");
        int mode = int.Parse(Console.ReadLine());

        switch (mode)
        {
            case 1: Console.WriteLine($"Хлопок — 40°C, 1000 об/мин."); break;
            case 2: Console.WriteLine($"Синтетика — 30°C, 800 об/мин."); break;
            case 3: Console.WriteLine($"Шерсть — 30°C, 600 об/мин."); break;
            case 4: Console.WriteLine($"Быстрая стирка 15 мин — 30°C, 800 об/мин."); break;
            case 5: Console.WriteLine($"Отжим — без стирки, 1000 об/мин."); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №199. Ввести код тарифной зоны электроэнергии (1 — Пик, 2 — Полупик, 3 — Ночь). Вывести стоимость киловатт-часа.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите код тарифной зоны: ");
        int zone = int.Parse(Console.ReadLine());

        switch (zone)
        {
            case 1: Console.WriteLine($"Пик — 7 рублей за кВт-ч."); break;
            case 2: Console.WriteLine($"Полупик — 5 рублей за кВт-ч."); break;
            case 3: Console.WriteLine($"Ночь — 3 рубля за кВт-ч."); break;
            default: Console.WriteLine($"Ошибка"); break;
        }
    }
}
```

> * №200. Ввести код состояния потока выполнения в C# (Running, Suspended, Stopped, Aborted). Вывести пояснение жизненного цикла потока.

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Введите код состояния потока выполнения в C#: ");
        string state = Console.ReadLine();

        switch (state)
        {
            case "Running": Console.WriteLine($"Поток выполняется"); break;
            case "Suspended": Console.WriteLine($"Поток приостановлен"); break;
            case "Stopped": Console.WriteLine($"Поток остановлен"); break;
            case "Aborted": Console.WriteLine($"Выполнение потока прервано"); break;
            default: Console.WriteLine($"Неизвестное состояние"); break;
        }
    }
}
```
