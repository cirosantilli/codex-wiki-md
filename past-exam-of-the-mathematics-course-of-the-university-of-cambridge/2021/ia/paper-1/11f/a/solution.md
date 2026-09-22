<h1 id="11f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Taylor theorem with Lagrange remainder](../../../../../../taylor-theorem-with-lagrange-remainder.md) states that if $f$ is $n$ times differentiable between $a$ and $x$, then some $\xi$ between $a$ and $x$ satisfies

$$
f(x)=\sum_{j=0}^{n-1}
\frac{f^{(j)}(a)}{j!}(x-a)^j
+\frac{f^{(n)}(\xi)}{n!}(x-a)^n.
$$

Let $T_{n-1}$ denote the displayed polynomial and choose $K$ so that

$$
F(t)=f(t)-T_{n-1}(t)-K(t-a)^n
$$

satisfies $F(x)=0$. By construction,

$$
F(a)=F'(a)=\cdots=F^{(n-1)}(a)=0.
$$

Starting with the two zeros $a,x$ and applying [Rolle theorem](../../../../../../rolle-theorem.md) repeatedly, there is a $\xi$ between them with $F^{(n)}(\xi)=0$. Since

$$
F^{(n)}(\xi)=f^{(n)}(\xi)-n!K,
$$

we have $K=f^{(n)}(\xi)/n!$, proving the theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11F](../../11f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
