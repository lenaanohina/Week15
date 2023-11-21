# Week15. Ответы на вопросы.

## 1. Из скольких частей состоит основной цикл?

Цикл состоит из 2-ух частей - условия и тела.
Тело цикла — это код, который выполняется, пока выполняется условие цикла.

## 2. Какое количество уровней вложенности могут иметь циклы?

Количество уровней вложенности, как правило, не ограничивается.

## 3. Если switch находится внутри функции, какая инструкция может использоваться для выхода из него?

Инструкция `break` выполняет выход из блока switch .

## 4. Можно ли пропускать части **for**? Что получится, если написать `for(;;)`?

Любое из трёх выражений цикла **for**(инициализация, логическое выражение или шаг) можно пропустить.

Если написать `for(;;)`, то получится бесконечный цикл.

## 5. Самостоятельно разберитесь, как работает цикл while и приведите два примера кода с его использованием.

`while` создаёт цикл, выполняющий заданную инструкцию, пока истинно проверяемое условие. Проверяет условие перед каждой итерацией.

```js
// Пример 1
let num = 0;

while (num < 3) {
  console.log(num);
  num++;
}

// Пример 2
let num = 5;

while (num) {
  console.log(num);
  num--;
}
```

## 6. Как можно принудительно остановить выполнение цикла?

Принудительно остановить выполнение цикла можно с помощью директивы `break`.

Если полностью прекращать цикл не нужно, а только его итерацию, то используют директиву `continue`.

## 7. При помощи цикла for выведите чётные числа от 2 до 10.

```js
for (let i = 2; i <= 10; i += 2) {
  console.log(i);
}
```

## 8. Если тело цикла состоит лишь из одной инструкции, мы можем опустить фигурные скобки `{…}`?

Да, можно опустить фигурные скобки, если тело цикла состоит лишь из одной инструкции.

```js
// Пример
let num = 5;
while (num) console.log(num--);
```

## 9. Что выведет цикл?

```js
for (let i = 0; i < 3; i++) {
  console.log(i);
}
//Выведет:
// 0
// 1
// 2
```

## 10. Оба цикла выводят в консоль одинаковые значения или нет?

```js
let i = 0;
while (++i < 5) console.log(i);
//Выведет:
// 1
// 2
// 3
// 4

let i = 0;
while (i++ < 5) console.log(i);
//Выведет:
// 1
// 2
// 3
// 4
// 5
```

Ответ - нет.
