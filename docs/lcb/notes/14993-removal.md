# Extension Builder Language
## Core types

* The use of the keyword `undefined`, which was deprecated in LiveCode
  8.0.0, has been removed.  Use `nothing` instead.
  * Use `returns nothing` when defining a handler which returns no
    value.
  * Use `nothing` to indicate no value when manipulating optionally
    type variables

* The `is defined`, `is undefined`, `is not defined`, and `is not
  undefined` syntax, which was deprecated in LiveCode 8.0.0, has been
  removed.  Use `is` and `is not` with `nothing` instead.
  * Use `<expr> is nothing` and `<expr> is not nothing` to test
    whether an expression has a value or not
  * The expression `<left> is <right>` will now evaluate to `true` if
    `<left>` and `<right>` are both nothing
  * The expression `<left> is not <right>` will now evaluate to `true`
    if one of `<left>` or `<right>` are nothing (but not both).
