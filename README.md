# active-calculus-single-mbx
Repository for a conversion of Active Calculus (single variable) to MathBook XML

Active Calculus is available from [scholarworks.gvsu.edu](http://scholarworks.gvsu.edu/books/10/). This project aims to convert Active Calculus 2016 edition to a version in [MathBook XML](mathbook.pugetsound.edu).

# Quickstart Instructions

1. Clone this repository.
2. Clone [MathBook XML](https://github.com/rbeezer/mathbook) and install its dependencies, including [lxml](https://lxml.de/) for Python3 and XeLaTeX.
3. Copy `Makefile.paths.original` to `Makefile.paths`.  Edit `Makefile.paths` as instructed within that file.
4. If you want to use a local WeBWorK server instead of `webwork-ptx.aimath.org`, follow the instructions [here](https://pretextbook.org/doc/publisher-guide/html/webwork-configuration.html) for configuring your WeBWorK server, and set the variable `SERVER` in `Makefile' to its address.
5. Execute `make acs-extraction`.
6. Then execute `make html`, `make pdf`, or other things detailed in `Makefile`. Output will be produced in the `output` folder.
