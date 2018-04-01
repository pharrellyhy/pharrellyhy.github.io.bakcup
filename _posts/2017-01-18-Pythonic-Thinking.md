---
layout: post
title: Pythonic Thinking
tags: python
---
Programmers from other languages may not familiar with the word _pythonic_ and its meaning. Basically, each programming language follows a particular coding style. Over the years, the Python community has come to use the adjective _pythonic_ to describe the code that follows its own style.

The first thing that will make your code _pythonic_ is to follow [PEP 8](https://www.python.org/dev/peps/pep-0008/) Style Guide. I will list some rules that I think are most important:

**Whitespace**:
+ Use spaces instead of tabs for indentation.
+ Use four spaces for each level of syntactically significant indenting.
+ Lines should be 79 characters in length or less (There have some discussions that for modern computers which have wider screen would definitely fit more characters in one line. So around 100 should be a reasonable choice).
+ Functions and classes that in a file should be separated by two blank lines
+ Methods in a class should be separated by one blank line.
+ **_No space_** aorund list indices, function calls or keyword argument assignments 
+ Put **_only one_** space before and after variable assignments.

**Naming**:
+ Functions, variables and attributes should be in *lowercase_underscore* format.
+ Protected functions and instance attributes should be in *_leading_underscore* format.
+ Private instance attributes should be in *__double_leading_underscore* format.
+ Classes and exceptions should be in *CapitalizedWord* format.
+ Module level constants should be in ALL_CAPS format.
+ Class methods should use *cls* as the name of the first parameter (which refers to the class)
+ Instance methods in classes should use *self* as the name of the first parameter (which refers to the class)

**Expressions and Statements**:
+ Use inline negation (`if x is not y`) instead of negation of positive expressions (`if not x is y`).
+ Don't check for empty values (`[] or ''`) by checking their lengh (`if len(x) == 0`). Use `if not x` and empty values are implicitly evaluated to `False`.
+ Always put `import` at the top of a file.
+ Always use absolute import instead relative import. For example, `from bar import foo`, not just `import foo`.

If you use **Sublime** as your coding editor, I would recommand using **Anaconda** to check your coding style. Just open *Anaconda User-Settings* and set `anaconda_linting` to `true`. You can also ignore some *PEP8* rules by setting a `pep8_ignore` list. 
