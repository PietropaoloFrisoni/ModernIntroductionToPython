# Modern Python: A Practical Introduction from Scratch

Public repository for the *Modern Python: A Practical Introduction from Scratch* course.

**Instructor:** Pietropaolo Frisoni. Computational Scientist, Quantum Software Engineer.

---

## How to use this repository

Thank you for visiting this repository!

Each folder corresponds to one chapter or intermezzo of the course.
Inside each folder you will find the Jupyter notebook for that unit (the same one recorded in the lecture) and a `References.md`
file with links to the official Python documentation and further reading.

You can follow the folders in the order listed below, which is the same order used in the lectures.

I hope you find it useful, and I wish you a lot of fun!

---

## Course order

| # | Folder | Unit |
|---|--------|------|
| 1  | `ch00_brief_overview_of_python`    | Chapter 0: A Brief Overview of Python *(slides only, no notebook)* |
| 2  | `int0_practical_environment`       | Intermezzo 0: The Practical Environment |
| 3  | `ch01_python_as_a_calculator`      | Chapter 1: Python as a Calculator |
| 4  | `ch02_control_flow`                | Chapter 2: Control Flow |
| 5  | `int1_booleans_in_depth`           | Intermezzo 1: Booleans in Depth |
| 6  | `int2_mutability`                  | Intermezzo 2: Mutability |
| 7  | `ch03_data_structures`             | Chapter 3: Built-in Data Structures |
| 8  | `ch04_functions_basics`            | Chapter 4: Functions — Basics |
| 9  | `ch05_functions_advanced`          | Chapter 5: Functions — Advanced |
| 10 | `int3_iterators_generators`        | Intermezzo 3: Iterators and Generators |
| 11 | `ch06_decorators`                  | Chapter 6: Decorators |
| 12 | `ch07_classes_basics`              | Chapter 7: Classes — Basics |
| 13 | `ch08_classes_special_methods`     | Chapter 8: Classes — Special Methods |
| 14 | `ch09_classes_inheritance`         | Chapter 9: Classes — Inheritance |
| 15 | `ch10_exceptions`                  | Chapter 10: Exceptions |
| 16 | `ch11_file_io`                     | Chapter 11: File I/O |
| 17 | `ch12_modules_namespaces_scopes`   | Chapter 12: Modules, Namespaces, and Scopes |

---

## Setup

### Option 1: Local setup (more instructive)

This is the same setup that we used in Intermezzo 0, and the one shown throughout the course videos. I report it here for convenience:

1. Install [Visual Studio Code](https://code.visualstudio.com) and the **Python** and **Jupyter** extensions (both published by Microsoft)
2. Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html) with all default options, then reopen VSCode
3. Create and activate the course environment:
   ```bash
   conda create -n IntroductionToPython python=3.14
   conda activate IntroductionToPython
   ```
4. Install the required packages:
   ```bash
   pip install jupyterlab numpy
   ```
5. In VSCode: `Ctrl+Shift+P` → **Python: Select Interpreter** → choose the one that shows `IntroductionToPython` in the path
6. Clone this repository and open the chapter folders in VSCode

> **Note:** this is just the setup used in the videos, for consistency. Any other combination (PyCharm, `venv`/`virtualenv`, etc.) works just as well. Use whatever tools you're already comfortable with, or whatever you'd like to learn. The Python code itself doesn't change :)

### Option 2: Google Colab (no setup required)

Open any `.ipynb` file directly on [Google Colab](https://colab.research.google.com)
by uploading it or pointing Colab at this repository.

---

## License

The course content (videos, slides, exercises) is available on Udemy.
I share the notebooks here for enrolled students and, more generally, everyone who wants to take a look.
