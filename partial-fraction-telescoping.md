# Partial fraction telescoping

↑ **Parent:** [Telescoping sum](telescoping-sum.md)

Sometimes a [sum](sum.md) does not initially look like a difference of neighboring entries. A [partial fraction decomposition](partial-fraction-decomposition.md) can reveal the cancellation. For the original example

$$
S_N=\sum_{k=1}^N\frac1{(3k-2)(3k+1)},
$$

subtract the two [reciprocals](multiplicative-inverse.md):

$$
\frac1{3k-2}-\frac1{3k+1}
=\frac{(3k+1)-(3k-2)}{(3k-2)(3k+1)}
=\frac3{(3k-2)(3k+1)}.
$$

Thus

$$
S_N=\frac13\left(1-\frac14+\frac14-\frac17+\cdots+\frac1{3N-2}-\frac1{3N+1}\right)
=\frac13\left(1-\frac1{3N+1}\right)
=\frac{N}{3N+1}.
$$

For $N=3$, direct [addition](addition.md) gives $1/4+1/28+1/70=3/10$. For $N=6$, the six positive entries add to $6/19\approx0.315789$. The [partial sums](partial-sum.md) approach $1/3$, and the exact [series remainder](series-remainder.md) is

$$
\boxed{\frac13-S_N=\frac1{3(3N+1)}.}
$$

This formula answers an accuracy question as well as a summation question. To make the remaining positive [series remainder](series-remainder.md) smaller than $0.001$, solve $1/[3(3N+1)]<1/1000$. The result is $9N+3>1000$, so **the smallest permitted [integer](integer-split.md) is $N=111$**. At $N=110$, the error is $1/993>0.001$; at $N=111$, it is $1/1002<0.001$.

## ↑ Ancestors (7)

1. [Telescoping sum](telescoping-sum.md)
2. [Summation](summation.md)
3. [Addition](addition.md)
4. [Arithmetic](arithmetic-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Boundary limits of telescoping series](boundary-limits-of-telescoping-series.md)
