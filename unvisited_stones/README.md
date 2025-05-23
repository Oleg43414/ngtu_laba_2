# Задача: Непосещённые валуны при перелёте птиц

## Условие задачи

Поперёк реки находятся `N` валунов, пронумерованных от 1 до `stones`. Стая птиц хочет перебраться с одного берега на другой.

Каждая i-ая птица может за один перелёт преодолеть расстояние `birds[i]`

**Например:**

- Если птица может перелететь 2 валуна за раз, то её путь будет состоять из валунов 2, 4, 6 и т.д.
- Если птица может перелететь 3 валуна, то она будет посещать валуны 3, 6, 9 и т.д.

**Задача:** Найти количество валунов, на которых **не появится ни одна птица** за всё время пересечения реки.

## Входные данные

- `N` — количество птиц (размер массива `birds`).
- `stones` — общее количество валунов.

`birds` — массив, где `birds[i]` — это расстояние, которое преодолевает i-ая птица за один перелёт.

## Выходные данные

Количество валунов, которые не были посещены ни одной птицей.

## Примеры

### Пример №1

```python
N = 2
stones = 6
birds = [3, 2]
```

### Объяснение

- Птица с `birds[0]` = 3 посещает валуны: 3, 6.
- Птица с `birds[1]` = 2 посещает валуны: 2, 4, 6.
- Непосещённые валуны: 1, 5.
    **Ответ:** `2` (валуны 1 и 5).

---

### Пример №2

```python
N = 2
stones = 6
birds = [5, 1]
```

### Объяснение

- Птица с `birds[0]` = 5 посещает валуны: 5.
- Птица с `birds[1]` = 1 посещает все валуны: 1, 2, 3, 4, 5, 6.
- Непосещённых валунов нет.
    **Ответ:** `0`

## Реализация

**Задача решается с помощью отметки посещённых валунов:**

1. Создаётся массив `visited` размером `stones + 1` (индексация от 1 до `stones`).
2. Для каждой птицы отмечаются все валуны, которые она посещает (с шагом `birds[i]`).
3. Подсчитывается количество `visited[i] = false` (непосещённые валуны).

### Доступные реализации

**Задача решена на 13 языках программирования:**

1. **C++** (`unvisited_stones.cpp`)
2. **Kotlin** (`UnvisitedStones.kt`)
3. **C#** (`UnvisitedStones.cs`)
4. **PHP** (`unvisited_stones.php`)
5. **Rust** (`unvisited_stones.rs`)
6. **Go** (`unvisited_stones.go`)
7. **TypeScript** (`unvisitedStones.ts`)
8. **Swift** (`UnvisitedStones.swift`)
9. **JavaScript** (`unvisitedStones.js`)
10. **Python** (`unvisited_stones.py`)
11. **Java** (`UnvisitedStones.java`)
12. **Ruby** (`unvisited_stones.rb`)
13. **Assembler** (`x86 NASM`) (`unvisited_stones.asm`)

Каждый файл содержит `DocString` с описанием функции и примером использования.

---

**Дата:** 14.04.2025
