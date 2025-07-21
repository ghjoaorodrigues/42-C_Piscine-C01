# C Piscine - C 01

![42 Badge](https://img.shields.io/badge/42-C_Piscine-brightgreen)
![C Badge](https://img.shields.io/badge/Language-C-blue)
![Status Badge](https://img.shields.io/badge/Status-Completed-success)

## What I Learned

Through this C 01 module of the C Piscine at 42 School, I developed fundamental programming skills and knowledge:

- **Pointer fundamentals** - Gained deep understanding of memory addresses and pointer operations
- **Memory manipulation** - Learned direct memory access through pointer dereferencing
- **Multi-level pointers** - Mastered complex pointer chains and indirection levels
- **Parameter passing by reference** - Understanding the difference between pass-by-value and pass-by-reference
- **Array manipulation** - Working with arrays through pointers and understanding array-pointer relationship
- **String handling** - Basic string operations using character pointers
- **Algorithm implementation** - Built sorting and reversing algorithms from scratch
- **Debugging skills** - Developed ability to trace through pointer operations and memory states
- **Code efficiency** - Learned to write compact, efficient functions with minimal overhead
- **42 Norm compliance** - Strict adherence to coding standards and best practices

This module established my foundation in pointer arithmetic and memory management, essential skills for all subsequent C programming at 42.

## About the Project

C 01 is the first module in the C Piscine curriculum focusing on pointers and basic memory manipulation. It introduces essential concepts through 9 progressively challenging exercises that build understanding of:

- Pointer dereferencing and assignment
- Multi-level pointer indirection
- Variable swapping through pointers
- Mathematical operations with pointer parameters
- String manipulation using character arrays
- Array processing and algorithms

## Implementation Details

The module consists of 9 exercises, each building upon previous concepts:

### Basic Pointer Operations

Foundation exercises introducing pointer concepts:

| Exercise | Function | Description | Key Concept |
|----------|----------|-------------|-------------|
| ex00 | ft_ft | Set value through single pointer | Basic dereferencing |
| ex01 | ft_ultimate_ft | Set value through 9-level pointer | Multi-level indirection |
| ex02 | ft_swap | Swap two integer values | Parameter modification |

### Mathematical Operations with Pointers

Functions that perform calculations and store results through pointer parameters:

| Exercise | Function | Description | Parameters |
|----------|----------|-------------|------------|
| ex03 | ft_div_mod | Division with separate result storage | a, b, *div, *mod |
| ex04 | ft_ultimate_div_mod | In-place division and modulo | *a, *b |

### String and Array Manipulation

Working with character and integer arrays through pointers:

| Exercise | Function | Description | Return Type |
|----------|----------|-------------|-------------|
| ex05 | ft_putstr | Display string to standard output | void |
| ex06 | ft_strlen | Count characters in string | int |
| ex07 | ft_rev_int_tab | Reverse integer array in place | void |
| ex08 | ft_sort_int_tab | Sort integer array ascending | void |

## Usage

```bash
# Compile individual exercises
cc -Wall -Wextra -Werror ft_ft.c -o ft_ft

# Test with main function (example for ft_ft)
cc -Wall -Wextra -Werror ft_ft.c main.c -o test
```

## Implementation Examples

### Basic Pointer Usage
```c
// ex00: ft_ft
void ft_ft(int *nbr)
{
    *nbr = 42;
}
```

### Multi-level Pointers
```c
// ex01: ft_ultimate_ft  
void ft_ultimate_ft(int *********nbr)
{
    *********nbr = 42;
}
```

### Array Manipulation
```c
// ex07: ft_rev_int_tab
void ft_rev_int_tab(int *tab, int size)
{
    int i = 0;
    int temp;
    
    while (i < size / 2)
    {
        temp = tab[i];
        tab[i] = tab[size - 1 - i];
        tab[size - 1 - i] = temp;
        i++;
    }
}
```

## Technical Challenges Overcome

- **Understanding pointer syntax** - Mastering the difference between `*ptr` and `ptr`
- **Multi-level indirection** - Navigating complex pointer chains without losing track
- **Array-pointer relationship** - Understanding how arrays decay to pointers in function parameters
- **In-place algorithms** - Modifying data structures without additional memory allocation
- **Boundary conditions** - Handling edge cases in array manipulation (empty arrays, single elements)
- **Memory safety** - Ensuring all pointer dereferences are valid to prevent segmentation faults

## Key Learning Outcomes

This module provided essential understanding of:
- How variables are stored in memory and accessed through addresses
- The relationship between arrays and pointers in C
- Parameter passing mechanisms and when to use each approach
- Basic algorithm implementation using only pointer arithmetic
- The importance of careful memory access and bounds checking

---

*This project was completed as part of the 42 School C Piscine, demonstrating my foundational understanding of C programming, pointer manipulation, and algorithm implementation.*

---

## License

This project is licensed under the [MIT License](./LICENSE).
