# Libft

Libft is the first C library I developed as part of the 42 curriculum.
It contains a collection of essential functions for memory handling, string manipulation, and basic I/O.
The goal was to reimplement core libc behavior and build a reusable foundation for future C projects.

## 🧩 Project Goals

* Recreate standard libc functions (`ft_strlen`, `ft_memcpy`, `ft_atoi`, etc.).
* Implement additional utility functions (`ft_split`, `ft_strjoin`, `ft_itoa`, etc.).
* Learn to design, structure, and maintain a C library.
* Follow the strict 42 Norm and ensure proper memory management (no leaks, no unexpected crashes).

> **Note:** Bonus functions were not implemented in this version.

## 📁 Library Contents

### 📝 Part 1 — Reimplemented libc Functions

Recreations of common standard functions, including:

* Character tests: `ft_isalpha`, `ft_isdigit`, `ft_isalnum`, ...
* Memory operations: `ft_memset`, `ft_memcpy`, `ft_memmove`, `ft_bzero`, ...
* String operations: `ft_strlen`, `ft_strlcpy`, `ft_strncmp`, `ft_strchr`, ...
* Conversions: `ft_atoi`
* Allocation: `ft_calloc`, `ft_strdup`

### 🧪 Part 2 — Additional Utility Functions

Higher-level functions built using dynamic allocation:

* Substrings: `ft_substr`
* String joining: `ft_strjoin`
* String trimming: `ft_strtrim`
* String splitting: `ft_split`
* Integer-to-string: `ft_itoa`
* Mapping & iteration: `ft_strmapi`, `ft_striteri`
* File descriptor output: `ft_putchar_fd`, `ft_putstr_fd`, `ft_putnbr_fd`, ...

## 🔧 Compilation

The project comes with a Makefile containing the rules:
`make`, `clean`, `fclean`, `re`.

To build the library:

```bash
make
```

This produces the **libft.a** static library at the project root.

## 🚀 Usage

In another project:

```c
#include "libft.h"
```

Compile with:

```bash
cc my_program.c libft.a -I .
```

## 📚 What I Learned

Through this project, I strengthened my understanding of:

* low-level memory mechanisms in C,
* safe dynamic allocation and error handling,
* writing clean, maintainable, and norm-compliant code,
* building foundational tools for future C projects.

