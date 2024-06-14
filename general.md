# General consensus

1. Functions and class methods must be written under the constraint of 20 lines.
2. Given the functionalities, they must follow the standardized methods explained in this repository.
3. Developers must use >3.10 python version for typing purposes(Usage of | operator instead of Union):

```python 
from typing import Union
## Use this
numero: int | float = 3
## Instead of
numero: Union[int, float] = 3
```

4. Each recursive function must be supported by a decent amount of error handling routines that avoid issues.
5. The usage of annotations are mandatory for local and global variables, functions, methods, etc.
6. Comments must be written with the number sign syntax (#) for one-line comments under 10 words, for many-line comments, the triple quotation mark syntax must be used (remember that each line must have at most 10 words) both immitating the behaviour of markdown files:

```python 
# Tyni comment $M_i$ 

"""
# Title
## Subtitle
### Subsubtitle
- point 1
- point 2
- point 3
1. enum 1
2. enum 2
3. enum 3

latex syntax
$\sum_{i = 1}^n i$

$
\begin{equation}

\end{equation}
$
"""
```
The only exception to this rule is complex latex expressions.

7. The usage of standarized Black formatter is mandatory in the continuous integration step.
8. Each repository must be maintained under a CI/CD workflow with the following components:
    ## CI:
    - Test automation for indepedent functionalities and integrated ones.
    - Black formatter.
    - Auto commit to branch.
    ## CD
    - push version to pypi.

9. 






