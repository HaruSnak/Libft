<img src="readme/libft.png" alt="libft" width="900"/>

# Libft
The libft project is a compulsory project for students of school 42. It consists of creating a static library of utility functions in C language. This library must reimplement certain functions of the standard C library, as well as other functions deemed useful by the students.

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

## 📒 Index

- [About](#about)
- [Installation](#installation)
- [Development](#development)
  - [File Structure](#file-structure) 
- [Notes](#notes)
- [Credits](#credits)

## About
**Functions contained in this library:**<br>
<br>


### Functions from `<ctype.h>`

- [`ft_isalnum`](char/ft_isalnum.c) - checks for an alphanumeric character.
- [`ft_isalpha`](char/ft_isalpha.c) - checks for an alphabetic character.
- [`ft_isascii`](char/ft_isascii.c) - checks whether c fits into the ASCII character set.
- [`ft_isdigit`](char/ft_isdigit.c) - checks for a digit (0 through 9).
- [`ft_isprint`](char/ft_isprint.c) - checks for any printable character.
- [`ft_tolower`](char/ft_tolower.c) - convert char to lowercase.
- [`ft_toupper`](char/ft_toupper.c) - convert char to uppercase.


### Functions from `<string.h>`

- [`ft_bzero`](mem/ft_bzero.c) - zero a byte string.
- [`ft_memchr`](mem/ft_memchr.c) - scan memory for a character.
- [`ft_memcmp`](mem/ft_memcmp.c) - compare memory areas.
- [`ft_memcpy`](mem/ft_memcpy.c) - copy memory area.
- [`ft_memmove`](mem/ft_memmove.c) - copy memory area.
- [`ft_memset`](mem/ft_memset.c) - fill memory with a constant byte.
- [`ft_strchr`](str/ft_strchr.c) - locate character in string.
- [`ft_strdup`](str/ft_strdup.c) - creates a duplicate for the string passed as parameter.
- [`ft_strlcat`](str/ft_strlcat.c) - concatenate string to a specific size.
- [`ft_strlcpy`](str/ft_strlcpy.c) - copy string to a specific size.
- [`ft_strlen`](str/ft_strlen.c) - calculate the length of a string.
- [`ft_strncmp`](str/ft_strncmp.c) - compare two strings.
- [`ft_strnstr`](str/ft_strnstr.c) - locate a substring in a string.
- [`ft_strrchr`](str/ft_strrchr.c) - locate character in string.

### Functions from `<stdlib.h>`
- [`ft_atoi`](conv/ft_atoi.c)	- convert a string to an integer.
- [`ft_calloc`](mem/ft_calloc.c)	- allocates memory and sets its bytes' values to 0.

### Non-standard functions
- [`ft_itoa`](conv/ft_itoa.c) - converts a number into a string.
- [`ft_putchar_fd`](put/ft_putchar_fd.c) - output a char to a file descriptor.
- [`ft_putendl_fd`](put/ft_putendl_fd.c) - output a string to a file descriptor, followed by a new line.
- [`ft_putnbr_fd`](put/ft_putnbr_fd.c) - output a number to a file descriptor.
- [`ft_putstr_fd`](put/ft_putstr_fd.c) - output a string to a file descriptor.
- [`ft_split`](str/ft_split.c) - splits a string using a char as parameter.
- [`ft_striteri`](str/ft_striteri.c) - applies a function to each character of a string.
- [`ft_strjoin`](str/ft_strjoin.c) - concatenates two strings.
- [`ft_strmapi`](str/ft_strmapi.c) - applies a function to each character of a string.
- [`ft_strtrim`](str/ft_strtrim.c) - trims the beginning and end of string with specific set of chars.
- [`ft_substr`](str/ft_substr.c) - returns a substring from a string.


### Linked list functions

- [`ft_lstadd_back`](lst/ft_lstadd_back_bonus.c) - adds an element at the end of a list.
- [`ft_lstadd_front`](lst/ft_lstadd_front_bonus.c) - adds an element at the beginning of a list.
- [`ft_lstclear`](lst/ft_lstclear_bonus.c) - deletes and free list.
- [`ft_lstdelone`](lst/ft_lstdelone_bonus.c) - deletes one element from the list.
- [`ft_lstiter`](lst/ft_lstiter_bonus.c) - applies a function to each element of a list.
- [`ft_lstlast`](lst/ft_lstlast_bonus.c) - returns the last element of the list.
- [`ft_lstmap`](lst/ft_lstmap_bonus.c) - applies a function to each element of a list.
- [`ft_lstnew`](lst/ft_lstnew_bonus.c) - creates a new list element.
- [`ft_lstsize`](lst/ft_lstsize_bonus.c) - counts the number of elements in a list.


## Installation
```bash
# Clone this repository
$ git clone https://github.com/HaruSnak/Libft.git

# Go into the repository
$ cd Libft

# To compile the program
$ make

# Allows you to do a complete cleaning of your construction environment
$ make fclean # Or make clean
```

## Usage
To use the Libft library in your C projects:

1. Include the header file in your source code:
   ```c
   #include "libft.h"
   ```

2. Compile your program linking with the library:
   ```bash
   gcc your_program.c libft.a -o your_program
   ```

3. Run your program:
   ```bash
   ./your_program
   ```

## Makefile Targets
- `make` or `make all`: Compile the main library functions and create `libft.a`.
- `make bonus`: Compile the bonus linked list functions and add them to `libft.a`.
- `make clean`: Remove object files.
- `make fclean`: Remove object files and the library file.
- `make re`: Recompile everything from scratch.
- `make normi`: Check norminette for main files.
- `make normib`: Check norminette for bonus files.

## Development
### File Structure

```
.
└── 📁libft
    └── Makefile
    └── 📁char
        └── ft_isalnum.c
        └── ft_isalpha.c
        └── ft_isascii.c
        └── ft_isdigit.c
        └── ft_isprint.c
        └── ft_tolower.c
        └── ft_toupper.c
    └── 📁conv
        └── ft_atoi.c
        └── ft_itoa.c
    └── 📁includes
        └── libft.h
    └── 📁lst
        └── ft_lstadd_back_bonus.c
        └── ft_lstadd_front_bonus.c
        └── ft_lstclear_bonus.c
        └── ft_lstdelone_bonus.c
        └── ft_lstiter_bonus.c
        └── ft_lstlast_bonus.c
        └── ft_lstmap_bonus.c
        └── ft_lstnew_bonus.c
        └── ft_lstsize_bonus.c
    └── 📁mem
        └── ft_bzero.c
        └── ft_calloc.c
        └── ft_memchr.c
        └── ft_memcmp.c
        └── ft_memcpy.c
        └── ft_memmove.c
        └── ft_memset.c
    └── 📁put
        └── ft_putchar_fd.c
        └── ft_putendl_fd.c
        └── ft_putnbr_fd.c
        └── ft_putstr_fd.c
    └── 📁str
        └── ft_split.c
        └── ft_strchr.c
        └── ft_strdup.c
        └── ft_striteri.c
        └── ft_strjoin.c
        └── ft_strlcat.c
        └── ft_strlcpy.c
        └── ft_strlen.c
        └── ft_strmapi.c
        └── ft_strncmp.c
        └── ft_strnstr.c
        └── ft_strrchr.c
        └── ft_strtrim.c
        └── ft_substr.c
```

## Notes
<p align="left">
    <img src="https://image.noelshack.com/fichiers/2024/11/2/1710270009-125.png"
         alt="Sponsored by Evil Martians" width="180" height="164">
</p>

## Credits

Below you will find the links used for this project:

- [Norm 42](https://cdn.intra.42.fr/pdf/pdf/960/norme.en.pdf)

[contributors-shield]: https://img.shields.io/github/contributors/HaruSnak/Libft.svg?style=for-the-badge
[contributors-url]: https://github.com/HaruSnak/Libft/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/HaruSnak/Libft.svg?style=for-the-badge
[forks-url]: https://github.com/HaruSnak/Libft/network/members
[stars-shield]: https://img.shields.io/github/stars/HaruSnak/Libft.svg?style=for-the-badge
[stars-url]: https://github.com/HaruSnak/Libft/stargazers
[issues-shield]: https://img.shields.io/github/issues/HaruSnak/Libft.svg?style=for-the-badge
[issues-url]: https://github.com/HaruSnak/Libft/issues
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/shany-moreno-5a863b2aa

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
