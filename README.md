# A Lean 4 Metaprogramming Book

Authors: Arthur Paulino, Damiano Testa, Edward Ayers, Evgenia Karunus, Henrik Böving, Jannis Limperg, Siddhartha Gadgil, Siddharth Bhat

A PDF is [available here for download](../../releases/download/latest/Metaprogramming.in.Lean.4.pdf) (and is rebuilt on each change).

* Main
    1. [Introduction](md/main/intro.md)
    2. [Overview](md/main/overview.md)
    3. [Expressions](md/main/expressions.md)
    4. [`MetaM`](md/main/metam.md)
    5. [`Syntax`](md/main/syntax.md)
    6. [Macros](md/main/macros.md)
    7. [Elaboration](md/main/elaboration.md)
    8. [DSLs](md/main/dsls.md)
    9. [Tactics](md/main/tactics.md)
    10. [Cheat sheet](md/main/cheat-sheet.md)
* Extra
    1. [Options](md/extra/options.md)
    2. [Attributes](md/extra/attributes.md)
    1. [Pretty Printing](md/extra/pretty-printing.md)
* Solutions to exercises
    1. ...
    2. [Expressions](md/solutions/expressions.md)
    3. [`MetaM`](md/solutions/metam.md)
    4. [`Syntax`](md/solutions/syntax.md)
    5. ...
    6. [Elaboration](md/solutions/elaboration.md)

Sources to extract material from:
* [Material written by Ed](https://github.com/leanprover-community/mathlib4/blob/tutorial/docs/metaprogramming/02_metavariables.md)

## Contributing

The markdown files are generated automatically via [lean2md](https://github.com/arthurpaulino/lean2md).
Thus, if you're going to write or fix content for the book, please do so in the original Lean files inside the [lean](lean) directory.

**Important**: since `lean2md` is so simple, please avoid using comment sections
in Lean code blocks with `/- ... -/`. If you want to insert commentaries, do so
with double dashes `--`.

### Building the markdown files

This is not required, but if you want to build the markdown files, you can do so by running `lake run build`.
It requires having Python installed, as well as the `lean2md` package.

Or, if you have [viper](https://github.com/arthurpaulino/viper) installed and a linked environment that has `lean2md`, you can call `lake run viper_build`.
