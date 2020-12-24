---
title: Hello, World! in Raku
---

{% include menu.html %}

Great, we have learnt the most essential things that are required to talk to Raku and to see the response, so let’s go straight to the first real program, ‘Hello, World!’.

    say 'Hello, World!';

Just before we learn the basics of functions in the second part of this couse, let us see a few different options that you can use in this program.

First of all, you can put parentheses around the function argument:

    say('Hello, World!');

Second, you can use other functions, namely, `put`, and `print`. Again, with or without parentheses:

    put 'Hello, World!';

    print("Hello, World!\n");

Notice that in the case of `print`, you need to manyally add the newline character at the end of the message. But don’t worry, we’ll cover all these details later.

But before we move on, let me show one more exciting option. You can call a function as a method directly on the string:

    'Hello, World!'.say;

{% include nav.html %}