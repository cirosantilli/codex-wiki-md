# Karatsuba operand splitting

↑ **Parent:** [Karatsuba multiplication](karatsuba-multiplication.md)

Fix an [integer](integer.md) base $B\geq2$. Let $x,y\geq0$ have at most $n$ digits in [positional notation](positional-notation.md), treating zero as one digit. For $n>1$, set $m=\lceil n/2\rceil$ using the [ceiling function](ceiling-function.md), and $q=B^m$. [Euclidean division](euclidean-division.md) gives

$$
a=\lfloor x/q\rfloor,\quad b=x-aq,\qquad c=\lfloor y/q\rfloor,\quad d=y-cq,
$$

where $0\leq b,d<q$ and $0\leq a,c<B^{n-m}$. The [floor function](floor-function.md) selects the high block; the remainder selects the low block. Both operands must use the same $q$, including when their actual digit lengths differ.

For odd $n$, the low block has $m$ digit positions and the high block has $n-m=m-1$. Leading zero padding aligns a shorter operand without changing its [integer](integer.md) value. Padding to a power-of-two length is optional: the split itself works for every $n$. If power-of-two padding is used, the padded length is less than twice the original length, so it changes only a constant factor in the [asymptotic analysis](asymptotic-analysis.md).

## ↑ Ancestors (4)

1. [Karatsuba multiplication](karatsuba-multiplication.md)
2. [Algorithm](algorithm.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Karatsuba worked multiplication](karatsuba-worked-multiplication.md)
