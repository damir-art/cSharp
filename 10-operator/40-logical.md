# Логические операторы
Логические операторы

    &  (И)
    |  (ИЛИ)
    !  (НЕ)
    ^  (исключающее ИЛИ)
    && (укороченное И)
    || (укороченное ИЛИ)

## && оператор И
Возвращает `true`, если оба операнда `true`:

    true && true  // true
    true && false // false

## II оператор ИЛИ
Возвращает `true`, если хотябы один из операндов `true`:

    true && true   // true
    true && false  // true
    false && false // false

## ! оператор НЕ
Меняет логическое значение на противоположное:

    !true     // false
    !(!true)  // true, двойное отрицание
    !false    // true
    !(!false) // false, двойное отрицание 

## Приоритеты логических операций
При объединении логических операций помните о приоритете их выполнения.

    ! (сначала выплняется отрицание)
    &&
    ||

Далее выполнится && потом ||, две строки ниже одинаковы:

    bool logic = true || false && false;
    bool logic = true || (false && false);

Старайтесь всегда использовать круглые скобки.

# Разница между укороченным и обычным
`||` (укороченный) второй операнд вычисляться не будет, если первый операнд `true`

`|` (обычный) второй операнд будет вычисляться, даже если первый операнд `true`

Обычно используют укороченные операнды.