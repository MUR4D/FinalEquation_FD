# Метод Дормана-Принса для обыкновенных дифференциальных уравнений

Этот репозиторий содержит код на C++, реализующий метод Дормана-Принса (метод Рунге-Кутты 4-5) для решения обыкновенных дифференциальных уравнений (ОДУ) вида:

\[
\begin{cases}
    \dfrac{d^{2}y}{dx^{2}} + \text{sh}(x) \dfrac{dy}{dx} + xy + x = 0 \\
    0 \leq x \leq 1 \\
    -\dfrac{dy}{dx}(0) = 1 \\
    \dfrac{dy}{dx}(1) = 1 \\
\end{cases}
\]

## Структура кода

- `main.cpp`: Содержит основную реализацию метода Дормана-Принса для решения данного ОДУ.
- `fcn()`: Функция, определяющая систему уравнений для решения.
- `dopri5()`: Функция, реализующая метод Дормана-Принса.
- Константы и вспомогательные функции, необходимые для метода, определены внутри кода.
- Выводит результат на каждом шаге интеграции.

## Использование

Скомпилируйте код с помощью компилятора C++. Основная функция `main()` инициализирует параметры ОДУ и выполняет метод Дормана-Принса.

Для изменения системы ОДУ измените функцию `fcn()` в соответствии с вашим дифференциальным уравнением.

## Требования

- Компилятор C++
- Стандартная математическая библиотека

## Запуск

Скомпилируйте код с помощью компилятора C++ и запустите созданный исполняемый файл. Измените параметры и начальные условия в функции `main()` по необходимости.

## Лицензия

Этот код предоставляется по [лицензии MIT](LICENSE).