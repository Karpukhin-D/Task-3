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

