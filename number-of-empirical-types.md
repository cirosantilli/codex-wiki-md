# Number of empirical types

↑ **Parent:** [Method of types](method-of-types.md)

A possible [empirical distribution](type-information-theory.md) corresponds to nonnegative [integer](integer.md) counts $(n_1,\ldots,n_m)$ with sum $n$. [Stars and bars](stars-and-bars-combinatorics.md) therefore gives

$$
\#\{\text{length-}n\text{ types}\}=\binom{n+m-1}{m-1}\leq(n+1)^m.
$$

The bound also follows by letting each count independently range from zero to $n$, which overcounts tuples whose sum is wrong. With the [alphabet](alphabet.md) fixed, the count grows polynomially in $n$, whereas there are $m^n$ strings when $m\geq2$. For binary symbols there are exactly $n+1$ profiles: the number of ones can be any [integer](integer.md) from zero through $n$.

This reduces a rare-event calculation to a sum over profiles when the event depends only on counts. An event that depends on order may instead require counting the relevant subset inside each [type class](type-class.md). A source with [statistical dependence](statistical-dependence.md) need not make strings of the same [empirical distribution](type-information-theory.md) equiprobable; the memoryless assumption cannot simply be dropped.

## ↑ Ancestors (7)

1. [Method of types](method-of-types.md)
2. [Type (information theory)](type-information-theory.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
