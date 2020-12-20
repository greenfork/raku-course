---
title: Solution of ‘Class desks’
---

[Start](/raku-course/) / [Part 1](/raku-course/part1) / [Numbers](/raku-course/numbers) / [Exercises](/raku-course/numbers/exercises) / [Class desks](..)

# The solution of ‘Class desks’

The solution of the problem is shown below.

## Code

    my $students = 23;

    my $desks = $students div 2 + $students % 2;

    say "$desks desks must be bought.";


🦋 You can find the full code in the file [class-desks.raku](https://github.com/ash/raku-course/blob/master/exercises/numbers/class-desks.raku).

## Output

Run the program at least twice trying odd and even number of students. For example, for the input numbers `23` and `24`, the program prints the same result:

    $ raku class-desks.raku
    12 desks must be bought.

## Comments

It is not enough just to divide the number of students by two. It is important to handle both odd and even numbers, and in this solution, one of the possible solutions to round the number up is encoded: `$students div 2 + $students % 2`. When the number of students is even, the second component is zero, and the result is equal to the number of students divided by two. But when the number of students is odd, the first component is still an integer number due to the use of `div` instead of `/`, and the second term of the expression adds an extra desk.

## Next exercise

| [Number of tens](/raku-course/numbers/exercises/tens) →

## Course navigation

← [Numbers](/raku-course/numbers) / [Operations with numbers](/raku-course/numbers/operations) | [Code blocks](/raku-course/code-blocks) →