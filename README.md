<img src="readme/libft.png" alt="libft" width="900"/>

<div align="center">

# Libft
### A Comprehensive C Standard Library Implementation

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![License][license-shield]][license-url]

</div>

---

## 🇬🇧 English

<details>
<summary><b>📖 Click to expand/collapse English version</b></summary>

### About

**Libft** is a compulsory foundational project for 42 School students. It consists of creating a static library of utility functions in C, reimplementing essential standard C library functions alongside custom utility functions.

This project teaches:
- Memory management and allocation
- String manipulation techniques
- Data structures (linked lists)
- Makefile optimization
- Code documentation and norming standards

### 📋 Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Makefile Targets](#makefile-targets)
- [Function Reference](#function-reference)
- [Credits](#credits)

<a name="features"></a>

### ✨ Features

- **50+ utility functions** across multiple categories
- **Bonus linked list functions** for advanced data structure manipulation
- **Strict C89/C99 compliance** with 42 School norming standards
- **Fully documented** with clear purpose statements
- **Production-ready** static library compilation

<a name="installation"></a>

### 🚀 Installation

```bash
# Clone the repository
git clone https://github.com/HaruSnak/42-libft
cd 42-libft

# Compile the library
make

# Compile with bonus functions
make bonus
```

<a name="usage"></a>

### 💻 Usage

Include the library in your C projects:

```c
#include "libft.h"
```

Compile your program linking against the library:

```bash
gcc your_program.c libft.a -o your_program
./your_program
```

<a name="project-structure"></a>

### 📂 Project Structure

```
libft/
├── Makefile                 # Build configuration
├── includes/
│   └── libft.h             # Main header file
├── char/                   # Character type functions
│   ├── ft_isalnum.c
│   ├── ft_isalpha.c
│   ├── ft_isascii.c
│   ├── ft_isdigit.c
│   ├── ft_isprint.c
│   ├── ft_tolower.c
│   └── ft_toupper.c
├── conv/                   # Conversion functions
│   ├── ft_atoi.c
│   └── ft_itoa.c
├── mem/                    # Memory manipulation
│   ├── ft_bzero.c
│   ├── ft_calloc.c
│   ├── ft_memchr.c
│   ├── ft_memcmp.c
│   ├── ft_memcpy.c
│   ├── ft_memmove.c
│   └── ft_memset.c
├── str/                    # String manipulation
│   ├── ft_split.c
│   ├── ft_strchr.c
│   ├── ft_strdup.c
│   ├── ft_striteri.c
│   ├── ft_strjoin.c
│   ├── ft_strlcat.c
│   ├── ft_strlcpy.c
│   ├── ft_strlen.c
│   ├── ft_strmapi.c
│   ├── ft_strncmp.c
│   ├── ft_strnstr.c
│   ├── ft_strrchr.c
│   ├── ft_strtrim.c
│   └── ft_substr.c
├── put/                    # Output functions
│   ├── ft_putchar_fd.c
│   ├── ft_putendl_fd.c
│   ├── ft_putnbr_fd.c
│   └── ft_putstr_fd.c
└── lst/                    # Linked list (bonus)
    ├── ft_lstadd_back_bonus.c
    ├── ft_lstadd_front_bonus.c
    ├── ft_lstclear_bonus.c
    ├── ft_lstdelone_bonus.c
    ├── ft_lstiter_bonus.c
    ├── ft_lstlast_bonus.c
    ├── ft_lstmap_bonus.c
    ├── ft_lstnew_bonus.c
    └── ft_lstsize_bonus.c
```

<a name="makefile-targets"></a>

### 🛠️ Makefile Targets

| Target | Description |
|--------|-------------|
| `make` or `make all` | Compile library and create `libft.a` |
| `make bonus` | Add bonus linked list functions |
| `make clean` | Remove object files |
| `make fclean` | Remove object files and library |
| `make re` | Full recompilation |
| `make normi` | Check norminette compliance (main) |
| `make normib` | Check norminette compliance (bonus) |

<a name="function-reference"></a>

### 📚 Function Reference

#### Character Functions (`<ctype.h>`)
- [`ft_isalnum`](char/ft_isalnum.c) - Check for alphanumeric character
- [`ft_isalpha`](char/ft_isalpha.c) - Check for alphabetic character
- [`ft_isascii`](char/ft_isascii.c) - Check if character is ASCII
- [`ft_isdigit`](char/ft_isdigit.c) - Check for digit (0-9)
- [`ft_isprint`](char/ft_isprint.c) - Check for printable character
- [`ft_tolower`](char/ft_tolower.c) - Convert character to lowercase
- [`ft_toupper`](char/ft_toupper.c) - Convert character to uppercase

#### String Functions (`<string.h>`)
- [`ft_strchr`](str/ft_strchr.c) - Locate character in string
- [`ft_strlen`](str/ft_strlen.c) - Get string length
- [`ft_strdup`](str/ft_strdup.c) - Duplicate string
- [`ft_strlcpy`](str/ft_strlcpy.c) - Copy string with size limit
- [`ft_strlcat`](str/ft_strlcat.c) - Concatenate strings with size limit
- [`ft_strncmp`](str/ft_strncmp.c) - Compare strings (limited)
- [`ft_strnstr`](str/ft_strnstr.c) - Locate substring
- [`ft_strrchr`](str/ft_strrchr.c) - Find last character occurrence
- [`ft_split`](str/ft_split.c) - Split string by delimiter
- [`ft_strjoin`](str/ft_strjoin.c) - Concatenate two strings
- [`ft_strtrim`](str/ft_strtrim.c) - Trim characters from ends
- [`ft_substr`](str/ft_substr.c) - Extract substring
- [`ft_strmapi`](str/ft_strmapi.c) - Apply function to each character
- [`ft_striteri`](str/ft_striteri.c) - Apply function with index

#### Memory Functions (`<string.h>`)
- [`ft_memset`](mem/ft_memset.c) - Fill memory with constant byte
- [`ft_memcpy`](mem/ft_memcpy.c) - Copy memory area
- [`ft_memmove`](mem/ft_memmove.c) - Copy memory (overlapping safe)
- [`ft_memchr`](mem/ft_memchr.c) - Find byte in memory
- [`ft_memcmp`](mem/ft_memcmp.c) - Compare memory areas
- [`ft_bzero`](mem/ft_bzero.c) - Clear memory
- [`ft_calloc`](mem/ft_calloc.c) - Allocate and zero memory

#### Conversion Functions (`<stdlib.h>`)
- [`ft_atoi`](conv/ft_atoi.c) - Convert string to integer
- [`ft_itoa`](conv/ft_itoa.c) - Convert integer to string

#### Output Functions (Non-standard)
- [`ft_putchar_fd`](put/ft_putchar_fd.c) - Write character to file descriptor
- [`ft_putstr_fd`](put/ft_putstr_fd.c) - Write string to file descriptor
- [`ft_putendl_fd`](put/ft_putendl_fd.c) - Write string + newline to file descriptor
- [`ft_putnbr_fd`](put/ft_putnbr_fd.c) - Write number to file descriptor

#### Linked List Functions (Bonus)
- [`ft_lstnew`](lst/ft_lstnew_bonus.c) - Create new list element
- [`ft_lstadd_front`](lst/ft_lstadd_front_bonus.c) - Add element to list front
- [`ft_lstadd_back`](lst/ft_lstadd_back_bonus.c) - Add element to list back
- [`ft_lstlast`](lst/ft_lstlast_bonus.c) - Get last list element
- [`ft_lstsize`](lst/ft_lstsize_bonus.c) - Count list elements
- [`ft_lstdelone`](lst/ft_lstdelone_bonus.c) - Delete single element
- [`ft_lstclear`](lst/ft_lstclear_bonus.c) - Delete entire list
- [`ft_lstiter`](lst/ft_lstiter_bonus.c) - Apply function to each element
- [`ft_lstmap`](lst/ft_lstmap_bonus.c) - Apply function and create new list

### 👨‍🎓 Note
<p align="left">
    <img src="https://image.noelshack.com/fichiers/2024/11/2/1710270009-125.png"
         alt="Note" width="180" height="164">
</p>

<a name="credits"></a>

### 📖 Credits

- **42 School Norm**: [Official C Coding Standard](https://cdn.intra.42.fr/pdf/pdf/960/norme.en.pdf)

### 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

</details>

---

## 🇫🇷 Français

<details>
<summary><b>📖 Cliquez pour développer/réduire la version française</b></summary>

### À propos

**Libft** est un projet fondamental obligatoire pour les étudiants de l'école 42. Il s'agit de créer une bibliothèque statique de fonctions utilitaires en C, réimplémentant les fonctions essentielles de la librairie standard C avec des fonctions utilitaires personnalisées.

Ce projet enseigne :
- La gestion de la mémoire et l'allocation dynamique
- Les techniques de manipulation de chaînes
- Les structures de données (listes chaînées)
- L'optimisation des Makefiles
- La documentation du code et les normes de programmation

### 📋 Table des matières

- [Caractéristiques](#caractéristiques)
- [Installation](#installation-1)
- [Utilisation](#utilisation)
- [Structure du projet](#structure-du-projet)
- [Cibles du Makefile](#cibles-du-makefile)
- [Référence des fonctions](#référence-des-fonctions)
- [Crédits](#crédits-1)

<a name="caractéristiques"></a>

### ✨ Caractéristiques

- **Plus de 50 fonctions utilitaires** réparties dans plusieurs catégories
- **Fonctions de listes chaînées bonus** pour la manipulation avancée de structures de données
- **Conformité stricte C89/C99** avec les normes de l'école 42
- **Entièrement documentées** avec des descriptions claires
- **Prêtes pour la production** avec compilation en bibliothèque statique

<a name="installation-1"></a>

### 🚀 Installation

```bash
# Cloner le dépôt
git clone https://github.com/HaruSnak/Libft.git
cd Libft

# Compiler la bibliothèque
make

# Compiler avec les fonctions bonus
make bonus
```

<a name="utilisation"></a>

### 💻 Utilisation

Incluez la bibliothèque dans vos projets C :

```c
#include "libft.h"
```

Compilez votre programme en le liant à la bibliothèque :

```bash
gcc your_program.c libft.a -o your_program
./your_program
```

<a name="structure-du-projet"></a>

### 📂 Structure du projet

```
libft/
├── Makefile                 # Configuration de compilation
├── includes/
│   └── libft.h             # Fichier d'en-tête principal
├── char/                   # Fonctions de type caractère
│   ├── ft_isalnum.c
│   ├── ft_isalpha.c
│   ├── ft_isascii.c
│   ├── ft_isdigit.c
│   ├── ft_isprint.c
│   ├── ft_tolower.c
│   └── ft_toupper.c
├── conv/                   # Fonctions de conversion
│   ├── ft_atoi.c
│   └── ft_itoa.c
├── mem/                    # Manipulation de mémoire
│   ├── ft_bzero.c
│   ├── ft_calloc.c
│   ├── ft_memchr.c
│   ├── ft_memcmp.c
│   ├── ft_memcpy.c
│   ├── ft_memmove.c
│   └── ft_memset.c
├── str/                    # Manipulation de chaînes
│   ├── ft_split.c
│   ├── ft_strchr.c
│   ├── ft_strdup.c
│   ├── ft_striteri.c
│   ├── ft_strjoin.c
│   ├── ft_strlcat.c
│   ├── ft_strlcpy.c
│   ├── ft_strlen.c
│   ├── ft_strmapi.c
│   ├── ft_strncmp.c
│   ├── ft_strnstr.c
│   ├── ft_strrchr.c
│   ├── ft_strtrim.c
│   └── ft_substr.c
├── put/                    # Fonctions de sortie
│   ├── ft_putchar_fd.c
│   ├── ft_putendl_fd.c
│   ├── ft_putnbr_fd.c
│   └── ft_putstr_fd.c
└── lst/                    # Listes chaînées (bonus)
    ├── ft_lstadd_back_bonus.c
    ├── ft_lstadd_front_bonus.c
    ├── ft_lstclear_bonus.c
    ├── ft_lstdelone_bonus.c
    ├── ft_lstiter_bonus.c
    ├── ft_lstlast_bonus.c
    ├── ft_lstmap_bonus.c
    ├── ft_lstnew_bonus.c
    └── ft_lstsize_bonus.c
```
<a name="cibles-du-makefile"></a>

### 🛠️ Cibles du Makefile

| Cible | Description |
|-------|-------------|
| `make` ou `make all` | Compiler la bibliothèque et créer `libft.a` |
| `make bonus` | Ajouter les fonctions bonus de listes chaînées |
| `make clean` | Supprimer les fichiers objets |
| `make fclean` | Supprimer les fichiers objets et la bibliothèque |
| `make re` | Recompilation complète |
| `make normi` | Vérifier la conformité norminette (principal) |
| `make normib` | Vérifier la conformité norminette (bonus) |

<a name="référence-des-fonctions"></a>

### 📚 Référence des fonctions

#### Fonctions de caractère (`<ctype.h>`)
- [`ft_isalnum`](char/ft_isalnum.c) - Vérifier si alphanumétique
- [`ft_isalpha`](char/ft_isalpha.c) - Vérifier si alphabétique
- [`ft_isascii`](char/ft_isascii.c) - Vérifier si ASCII
- [`ft_isdigit`](char/ft_isdigit.c) - Vérifier si chiffre (0-9)
- [`ft_isprint`](char/ft_isprint.c) - Vérifier si imprimable
- [`ft_tolower`](char/ft_tolower.c) - Convertir en minuscule
- [`ft_toupper`](char/ft_toupper.c) - Convertir en majuscule

#### Fonctions de chaîne (`<string.h>`)
- [`ft_strchr`](str/ft_strchr.c) - Localiser caractère dans chaîne
- [`ft_strlen`](str/ft_strlen.c) - Obtenir longueur de chaîne
- [`ft_strdup`](str/ft_strdup.c) - Dupliquer chaîne
- [`ft_strlcpy`](str/ft_strlcpy.c) - Copier chaîne avec limite de taille
- [`ft_strlcat`](str/ft_strlcat.c) - Concaténer chaînes avec limite de taille
- [`ft_strncmp`](str/ft_strncmp.c) - Comparer chaînes (limitées)
- [`ft_strnstr`](str/ft_strnstr.c) - Localiser sous-chaîne
- [`ft_strrchr`](str/ft_strrchr.c) - Trouver dernière occurrence de caractère
- [`ft_split`](str/ft_split.c) - Diviser chaîne par délimiteur
- [`ft_strjoin`](str/ft_strjoin.c) - Concaténer deux chaînes
- [`ft_strtrim`](str/ft_strtrim.c) - Supprimer caractères des extrémités
- [`ft_substr`](str/ft_substr.c) - Extraire sous-chaîne
- [`ft_strmapi`](str/ft_strmapi.c) - Appliquer fonction à chaque caractère
- [`ft_striteri`](str/ft_striteri.c) - Appliquer fonction avec index

#### Fonctions de mémoire (`<string.h>`)
- [`ft_memset`](mem/ft_memset.c) - Remplir mémoire avec octet constant
- [`ft_memcpy`](mem/ft_memcpy.c) - Copier zone mémoire
- [`ft_memmove`](mem/ft_memmove.c) - Copier mémoire (chevauchement sûr)
- [`ft_memchr`](mem/ft_memchr.c) - Trouver octet en mémoire
- [`ft_memcmp`](mem/ft_memcmp.c) - Comparer zones mémoire
- [`ft_bzero`](mem/ft_bzero.c) - Effacer mémoire
- [`ft_calloc`](mem/ft_calloc.c) - Allouer et initialiser à zéro mémoire

#### Fonctions de conversion (`<stdlib.h>`)
- [`ft_atoi`](conv/ft_atoi.c) - Convertir chaîne en entier
- [`ft_itoa`](conv/ft_itoa.c) - Convertir entier en chaîne

#### Fonctions de sortie (Non-standard)
- [`ft_putchar_fd`](put/ft_putchar_fd.c) - Écrire caractère sur descripteur fichier
- [`ft_putstr_fd`](put/ft_putstr_fd.c) - Écrire chaîne sur descripteur fichier
- [`ft_putendl_fd`](put/ft_putendl_fd.c) - Écrire chaîne + nouvelle ligne
- [`ft_putnbr_fd`](put/ft_putnbr_fd.c) - Écrire nombre sur descripteur fichier

#### Fonctions de listes chaînées (Bonus)
- [`ft_lstnew`](lst/ft_lstnew_bonus.c) - Créer nouvel élément de liste
- [`ft_lstadd_front`](lst/ft_lstadd_front_bonus.c) - Ajouter élément en tête
- [`ft_lstadd_back`](lst/ft_lstadd_back_bonus.c) - Ajouter élément en queue
- [`ft_lstlast`](lst/ft_lstlast_bonus.c) - Obtenir dernier élément
- [`ft_lstsize`](lst/ft_lstsize_bonus.c) - Compter éléments de liste
- [`ft_lstdelone`](lst/ft_lstdelone_bonus.c) - Supprimer un élément
- [`ft_lstclear`](lst/ft_lstclear_bonus.c) - Supprimer toute la liste
- [`ft_lstiter`](lst/ft_lstiter_bonus.c) - Appliquer fonction à chaque élément
- [`ft_lstmap`](lst/ft_lstmap_bonus.c) - Appliquer fonction et créer nouvelle liste

### 👨‍🎓 Note
<p align="left">
    <img src="https://image.noelshack.com/fichiers/2024/11/2/1710270009-125.png"
         alt="Note" width="180" height="164">
</p>

<a name="crédits-1"></a>

### 📖 Crédits

- **Norme 42**: [Standard C officiel](https://cdn.intra.42.fr/pdf/pdf/960/norme.en.pdf)

### 📄 Licence

Ce projet est sous licence **MIT** - voir le fichier [LICENSE](LICENSE) pour plus de détails.

</details>

---

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
[license-shield]: https://img.shields.io/github/license/HaruSnak/Libft.svg?style=for-the-badge
[license-url]: https://github.com/HaruSnak/Libft/blob/master/LICENSE
