# Your grammar for the course

This repository holds the grammar you build during the course. The course
site reads `grammar.txt` from it: give the site the address of that file
once, with the **Source** button on the grammar card, and every page then
uses your grammar. A push is picked up shortly after.

## The rule format

One rule per line: a symbol, an arrow `->`, and the symbols it can be
rewritten as. A symbol on the left of some rule is a nonterminal; every
other symbol is a word. A rule may end with a probability in brackets, such
as `[0.5]`. Lines starting with `#` are comments.

## The tests

Each stage has a file of sentence tests in `tests/`, such as
`tests/stage1.txt`. A line starting with `+ ` is a sentence your grammar
must parse; a line starting with `- ` is a sentence it must not parse. The
site runs the current stage's tests on every page and says which sentences
fail and why.

## If you are stuck

Each stage has a reference grammar on the branch named after the stage,
such as `stage1`. Merge that branch, or copy its `grammar.txt`, to continue
from the reference grammar.
