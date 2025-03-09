# ft_PushSwap

This project asks us to sort data in a stack, using a limited set of instructions,
and with as few operations as possible.To succeed, we'll have to manipulate
different sorting algorithms and choose the most appropriate for optimized data sorting.

# Introduction

The Push swap project is a simple and effective algorithmic exercise: you have to sort some data.
We have at our disposal a set of integers, two stacks and a set of instructions for manipulating them.
Our goal? To write a C program called push_swap that calculates and displays on the standard output
the smallest program, made up of instructions from the Push swap language, for sorting the integers
passed as parameters.

The possible instructions are:

    pa (push A): Take the first element at the top of B and put it at the top of A. Do nothing if B is empty.
    pb (push B): Take the first element at the top of A and put it at the top of B. Do nothing if A is empty.
    sa (swap A): Swap the first 2 elements at the top of stack A. Do nothing if there is only one or no elements.
    sb (swap B): Swap the first 2 elements at the top of stack B. Do nothing if there is only one or no elements.
    ss: sa and sb at the same time.
    ra (rotate A): Shift all elements of stack A up by 1. The first element becomes the last one.
    rb (rotate B): Shift all elements of stack B up by 1. The first element becomes the last one.
    rr: ra and rb at the same time.
    rra (reverse rotate A): Shift all elements of stack A down by 1. The last element becomes the first one.
    rrb (reverse rotate B): Shift all elements of stack b down by 1. The last element becomes the first one.
    rrr : rra and rrb at the same time.


## Installing and Compiling ft_PushSwap

Clone the repository

```shell
https://github.com/guillaumeschwartz76/ft_PushSwap.git
```

You can go to the directory for compilation and can do ```make```.

## Executing ft_PushSwap

This program takes as its parameter a list of INTEGERS.

```shell
./push_swap 2 1 3 6 5 8
```

and display
```shell
pb
pb
sb
pb
ra
sa
rra
rra
pa
pa
pa
```

```shell
./push_swap 2 1 3 6 5 8 | wc -l
11
```

## Performance

To validate this project, we need to perform certain sorts with a minimum number of operations:

    - For a minimalist validation (and a score of 80/100), we need to be able to sort
    100 random numbers in less than 700 operations. Please note that we're talking
    about an average, but as a general rule, we should always have less than
    700 operations to complete the sort.

    - For optimum and maximum validation of the project,
    we need to fulfill the above condition, but also sort 500 random numbers
    all in a maximum of 5500 operations.

