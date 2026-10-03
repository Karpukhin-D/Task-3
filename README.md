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
