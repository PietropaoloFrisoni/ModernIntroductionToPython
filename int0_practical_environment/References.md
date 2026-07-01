# Intermezzo 0 — References
### Modern Introduction to Python from scratch

---

## Reference 1: [Installing Visual Studio Code](https://code.visualstudio.com/docs/setup/setup-overview)
**Official setup guide for Visual Studio Code across Windows, macOS, and Linux. Covers download, installation, and first launch.**

The installation steps change occasionally between OS versions, so I'd always check this page rather than following an older tutorial that might be outdated.

---

## Reference 2: [Python in Visual Studio Code](https://code.visualstudio.com/docs/languages/python)
**Official VS Code documentation for Python support, including how to install the Python extension, select an interpreter, and use features such as syntax highlighting, autocompletion, and the integrated debugger.**

The interpreter selection step in particular is something that trips up many people the first time (this page explains it clearly).

---

## Reference 3: [Installing Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)
**Official Conda installation guide. Covers the differences between Anaconda and Miniconda and provides instructions for all major operating systems.**

As mentioned in the video, you can use Miniconda, not necessarily Anaconda (Reference 5 explains why).

---

## Reference 4: [Conda User Guide](https://docs.conda.io/projects/conda/en/latest/user-guide/index.html)
**The official Conda user guide. Covers creating and managing environments, installing packages, switching between environments, and managing Python versions.**

The section on environments is the most important one for day-to-day use.

---

## Reference 5: [Miniconda](https://docs.anaconda.com/miniconda/)
**Official page for Miniconda, the lightweight alternative to the full Anaconda distribution. Recommended if you want a minimal Conda installation without pre-installed packages.**

This is what we installed in the course. The main reason to prefer Miniconda over Anaconda is that it doesn't bundle hundreds of packages you won't use (you install only what you need).

---

## Reference 6: [pip Documentation](https://pip.pypa.io/en/stable/)
**Official documentation for pip, the standard Python package installer. Covers installation, basic usage, managing requirements files, and configuration.**

You will use `pip install` so often it will become muscle memory. The rest of the documentation is worth knowing too.

---

## Reference 7: [PyPI — Python Package Index](https://pypi.org/)
**The official repository of Python packages. Every package installed via `pip install` is fetched from here by default. You can search for packages and browse their documentation pages.**

Worth searching here before writing any new functionality. Chances are someone has already written and packaged it.

---

## Reference 8: [venv — Creation of Virtual Environments](https://docs.python.org/3/library/venv.html)
**Official Python documentation for `venv`, the built-in module for creating lightweight virtual environments. Useful if you prefer a standard-library solution without installing Conda.**

An alternative to Conda if you want a lighter-weight solution. For this course we used Conda, but `venv` is good to know about. It is honestly easier if you only care about Python.

---

## Reference 9: [JupyterLab Documentation](https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html)
**Official installation and getting started guide for JupyterLab, the interactive development environment used in this course.**

If something goes wrong with the Jupyter setup inside VSCode, this is a good place to look for troubleshooting.

---

## Reference 10: [The Python Interpreter](https://docs.python.org/3/tutorial/interpreter.html)
**Official Python tutorial section on using the interpreter directly. Covers how to launch the REPL, pass scripts and arguments, and understand interactive mode.**

Worth reading if you want to use Python directly from the terminal, which I genuinely recommend for quick tests and experiments.
