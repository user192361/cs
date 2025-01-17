# Переменные и Типы данных в C++

## Переменные

- **Переменные** - это именованные области памяти, используемые для хранения данных в программе.

- В C++, перед использованием переменной её нужно **объявить** с указанием типа данных.

  Пример объявления переменной:

  ```cpp
  int age = 25;  // Объявление целочисленной переменной с именем "age" и значением 25
  ```

## Типы данных

C++ предоставляет различные **типы данных** для хранения разных видов данных. Ниже представлены основные типы данных:

- **Целочисленные типы данных**:

  - `int`: Целые числа.
  - `short`: Короткие целые числа.
  - `char`: Символы.

- **Вещественные типы данных**:

  - `float`: Одинарная точность с плавающей запятой.
  - `double`: Двойная точность с плавающей запятой.

- **Логический тип данных**:

  - `bool`: Булево значение `true` или `false`.

- **Тип данных для символьных строк**:
  - `std::string`: Строки текста.

## Именование переменных

- Нельзя начинать с цифры
- Нельзя включать спец. символы кроме "`_`"
- Нельзя использовать ключевые слова вроде `int`
- Старайтесь делать понятные названия (`studentsCount` лучше, чем `c`)

## Арифметические операции

- **Сложение (+)**: `int sum = a + b;`
- **Вычитание (-)**: `int difference = a - b;`
- **Умножение (\*)**: `int product = a * b;`
- **Деление (/)**: `float quotient = a / b;`
- **Остаток от деления (%)**: `int remainder = a % b;`

## Дополнительные операции:

- **Инкремент (++)**: `a++;` - увеличит `a` на единицу.
- **Декремент (--)**: `a--;` - точно не угадаете.

> Таким образом, можно увеличить значение `a` на единицу двумя способами: `a = a + 1` или `a++`.

## Работа со строками

- Для работы со строками используется тип данных `string`.

- Пример объявления и инициализации строки:

  ```cpp
  string name = "John";
  ```

- Строки можно конкатенировать:

  ```cpp
  string greeting = "Hello, " + name;
  ```

## Ввод и вывод значений

> Лайфхак: Если не хотите писать префикс `std::`, то можно написать перед `int main()` фразу `using namespace std;`.

- **Вывод на консоль**:

  ```cpp
  #include <iostream>

  using namespace std;

  int main() {
      int age = 30;
      cout << "Мой возраст: " << age << endl;
      return 0;
  }
  ```

- **Ввод с консоли**:

  ```cpp
  #include <iostream>

  using namespace std;

  int main() {
      int age;
      cout << "Введите ваш возраст: ";
      cin >> age;
      cout << "Ваш возраст: " << age << endl;
      return 0;
  }
  ```

## Таблица с типами данных

| Тип данных    | Размер в байтах | Предельные значения                              |
| ------------- | --------------- | ------------------------------------------------ |
| `int`         | 4               | От -2 x 10⁹ до 2 x 10⁹                           |
| `short`       | 2               | От -32,768 до 32,767                             |
| `long long`   | 8               | От -9 x 10¹⁸ до 9 x 10¹⁸                         |
| `char`        | 1               | От -128 до 127                                   |
| `float`       | 4               | Приблизительно от ±3.4 x 10³⁸ до ±1.18 x 10⁻³⁸   |
| `double`      | 8               | Приблизительно от ±1.8 x 10³⁰⁸ до ±2.22 x 10⁻³⁰⁸ |
| `bool`        | 1               | `true` или `false`                               |
| `std::string` | Переменный      | Не применимо                                     |

## Задачи!!

1. **Задача на целочисленные типы данных**:

   Вы разрабатываете программу для учета количества проданных билетов в кинотеатре. Каждый билет стоит 1500 рублей. Напишите программу, которая будет принимать количество проданных билетов и выводить общую сумму выручки.

2. **Задача на вещественные типы данных**:

   Вы разрабатываете программу для вычисления ежедневных расходов на бензин во время поездки на автомобиле. Пользователь вводит количество пройденных километров и средний расход топлива (в литрах на 100 километров). Напишите программу, которая вычислит и выведет общее количество потраченных литров топлива и стоимость на заправку.

3. **Комбинированная задача**:

   Вы разрабатываете программу для вычисления итоговой оценки по предметам в школе. Пользователь вводит оценки по 5 предметам (целые числа). Напишите программу, которая вычислит среднюю оценку и выведет её.
