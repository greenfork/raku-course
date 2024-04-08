---
title: Вывод с использованием `say`
---

{% include menu.html %}

Функция `say` (или подпрограмма, или просто программа) печатает значения в
стандартный поток вывода — `STDOUT`. Если вы запускаете программу из терминала,
там же будет и вывод. Если вы используете онлайн сервисы, вывод будет в
обозначенной для этого части страницы.

Вот пример использования `say`:

```raku
say 42;
```

Эта строка может быть как частью большей программы, так и полностью являться
программой. Очевидно, она напечатает `42`.

Теперь давайте попробуем поработать со строками:

```raku
say 'Hello, World!';
```

Voilà, мы получили `Hello, World!` на нашем экране.

Подпрограмма `say` может принимать больше, чем один аргумент, мы можем вывести
больше значений за один раз:

```raku
say 42, 'Hello, World!';
```

Отметьте, что части этого вывода соединены в одну строку: `42Hello, World!`,
поэтому лучше между ними добавить пробелы. И на данный момент вы уже должны быть
способы решить эту проблему, например, таким образом:

```raku
say 42, ' ', 'Hello, World!';
```

После вывода всех аргументов подпрограмма `say` добавит символ новой строки в
конец вывода.

{% include nav.html %}