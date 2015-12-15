Wordsearch generator
====================

(o Generador de sopas de letras)

Based on https://github.com/rboulton/wordsearch

Currently, this is a simple command-line script which generates a wordsearch
grid.

Usage:

 python wordsearch.py <difficulty> [word...]

The grid size, and permissible directions for words, is controlled by the
difficulty setting, which is one of `easy`, `normal` and `hard`.

The output grid is displayed on stdout, and written to a pdf file called with the same name of the first word.


Requirements
============

reportlab Python library (https://pypi.python.org/pypi/reportlab)

Improvements from the original version
======================================

* Configurable header and footer
* Allow words with spaces (using quotes). Example: `python wordsearch.py hard word1 "word with spaces" word3
* Allow not only ascii input (for example, words with ñ or á é í ó ú are fine)
