<h1 id="11h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [arithmetic function](../../../../../../arithmetic-function.md) $f$ is [multiplicative](../../../../../../multiplicative-function.md) when $f(1)=1$ and $f(mn)=f(m)f(n)$ whenever $m$ and $n$ are [coprime](../../../../../../coprime-integers.md). If $m$ and $n$ are coprime, every divisor $d$ of $mn$ has a unique factorization $d=d_1d_2$ with $d_1\mid m$ and $d_2\mid n$. Hence the [Dirichlet convolution](../../../../../../dirichlet-convolution.md) of multiplicative functions satisfies

$$
\begin{aligned}
(f\star g)(mn)
&=\sum_{d_1\mid m}\sum_{d_2\mid n}
f(d_1d_2)g\!\left(\frac m{d_1}\frac n{d_2}\right)\\
&=(f\star g)(m)(f\star g)(n),
\end{aligned}
$$

and $(f\star g)(1)=1$, so it is multiplicative.

Let $\varepsilon$ be the [identity for Dirichlet convolution](../../../../../../identity-for-dirichlet-convolution.md), with $\varepsilon(1)=1$ and $\varepsilon(n)=0$ for $n>1$. The [Möbius function](../../../../../../mobius-function.md) satisfies $\mu\star1=\varepsilon$. Therefore, using commutativity and associativity,

$$
f=\mu\star g
\quad\Longrightarrow\quad
f\star1=g\star(\mu\star1)=g\star\varepsilon=g.
$$

This is the [Möbius inversion formula](../../../../../../mobius-inversion-formula.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11H](../../11h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
