# Арифметические операторы

    byte a = 3;
    byte b = 5;
    int c = a + b; // результат арифметической операции должен быть int
    Console.WriteLine(c);
    
    c = a + b; // сложение
    c = a - b; // вычитание
    -с;        // унарный минус
    c = a * b; // умножение
    c = a / b; // деление, byte убирает всё что после точки
    c = a % b; // деление по модулю
    
    c++; // инкремент (постфикс)
    c--; // декремент (постфикс)

## Пример
Создаём калькулятор, который суммирует числа:

    Console.WriteLine("Введите первое число: ");
    byte a = Convert.ToByte(Console.ReadLine());

    Console.WriteLine("Введите второе число: ");
    byte b = Convert.ToByte(Console.ReadLine());

    int c = a + b;

    Console.WriteLine("Результат: " + c);
    // вместо `с` можно использовать (a + b) скобки обязательны

    Console.ReadKey();

## Инкремент, декремент
Различие между префиксом и постфиксом.

    x++; // аналог x = x + 1;

    int i = 1;
    print(i);   // 1
    print(i++); // 1
    print(i);   // 2
    print(++i); // 3

## `%` оператор деления по модулю
Остаток от деления двух чисел: 12 % 10 == 2
Можно применять как целым числам так и дробным.

## `/` оператор деления
Если деление применяется к целому числу, остаток от деления отбрасывается.