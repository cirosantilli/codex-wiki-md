<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [combinator](../../../../../../combinator.md) is a lambda term without free variables. It is a [fixed-point combinator](../../../../../../fixed-point-combinator.md) when

$$
YF\equiv_\beta F(YF)
$$

for every lambda term $F$.

The [fixed-point theorem for the untyped lambda calculus](../../../../../../fixed-point-theorem-for-the-untyped-lambda-calculus.md) states that every untyped lambda term $F$ has a fixed point up to [beta equivalence](../../../../../../beta-equivalence.md). Put

$$
X=(\lambda x.F(xx))(\lambda x.F(xx)).
$$

One beta reduction gives

$$
X\longrightarrow_\beta F((\lambda x.F(xx))(\lambda x.F(xx)))=F(X),
$$

which proves the theorem. Equivalently,

$$
Y=\lambda f.(\lambda x.f(xx))(\lambda x.f(xx))
$$

is a fixed-point combinator.

Apply the theorem to the lambda term $\operatorname{Succ}$. Its fixed point $Y\operatorname{Succ}$ is a nonnormalizing lambda term satisfying $Y\operatorname{Succ}\equiv_\beta\operatorname{Succ}(Y\operatorname{Succ})$; it is not a [Church numeral](../../../../../../church-numeral.md). The definition of a [lambda-definable function](../../../../../../lambda-definable-function.md) describes the representing term only on Church-numeral inputs, so it does not turn this syntactic fixed point into a natural number $n$ satisfying $n+1=n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
