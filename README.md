# goit-js-hw-03

## Задача 1. Генератор slug `task-1.js`

**Slug** — це завжди рядок у нижньому регістрі, слова якого розділені тире.

🟨 Напиши функцію `slugify(title)`, яка приймає заголовок статті, параметр `title` і повертає
`slug`, створений із цього рядка.

- Значенням параметра `title` будуть рядки, слова яких розділені лише пробілами.
- Усі символи `slug` повинні бути в нижньому регістрі.
- Усі слова `slug` повинні бути розділені тире.

```
console.log(slugify("Arrays for begginers")); // "arrays-for-begginers"
console.log(slugify("English for developer")); // "english-for-developer"
console.log(slugify("Ten secrets of JavaScript")); // "ten-secrets-of-javascript"
console.log(slugify("How to become a JUNIOR developer in TWO WEEKS")); // "how-to-become-a-junior-developer-in-two-weeks"
```

## Задача 2. Композиція масивів `task-2.js`

🟨 Напиши функцію під назвою `makeArray`, яка приймає три параметри: `firstArray` (масив),
`secondArray` (масив) і `maxLength` (число). Функція повинна створювати новий масив, який містить
усі елементи з `firstArray`, а потім усі елементи з `secondArray`.

- Якщо кількість елементів у новому масиві перевищує `maxLength`, функція повинна повернути копію
  масиву з довжиною `maxLength` елементів.
- В іншому випадку функція повинна повернути весь новий масив.

```
console.log(makeArray(["Mango", "Poly"], ["Ajax", "Chelsea"], 3)); // ["Mango", "Poly", "Ajax"]
console.log(makeArray(["Mango", "Poly", "Houston"], ["Ajax", "Chelsea"], 4)); // ["Mango", "Poly", "Houston", "Ajax"]
console.log(makeArray(["Mango"], ["Ajax", "Chelsea", "Poly", "Houston"], 3)); // ["Mango", "Ajax", "Chelsea"]
console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 2)); // ["Earth", "Jupiter"]
console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 4)); // ["Earth", "Jupiter", "Neptune", "Uranus"]
console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus", "Venus"], 0)); // []
```

## Задача 3. Фільтрація масиву чисел `task-3.js`

🟨 Напиши функцію `filterArray(numbers, value)`, яка приймає масив чисел (`numbers`) та значення
(`value`) як параметри. Функція повинна повертати новий масив лише тих чисел із масиву `numbers`,
які більші за значення `value`.

```
console.log(filterArray([1, 2, 3, 4, 5], 3)); // [4, 5]
console.log(filterArray([1, 2, 3, 4, 5], 4)); // [5]
console.log(filterArray([1, 2, 3, 4, 5], 5)); // []
console.log(filterArray([12, 24, 8, 41, 76], 38)); // [41, 76]
console.log(filterArray([12, 24, 8, 41, 76], 20)); // [24, 41, 76]
```
