<h1 id="10f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One precise version of the [Taylor theorem with Lagrange remainder](../../../../../../taylor-theorem-with-lagrange-remainder.md) is as follows. Let $n\geq0$, let $f$ and its [derivatives](../../../../../../derivative.md) through order $n$ be continuous on the closed interval between distinct points $a$ and $x$, and suppose $f^{(n+1)}$ exists throughout its interior. Then some $\xi$ strictly between $a$ and $x$ satisfies

$$
\boxed{f(x)=\sum_{k=0}^n\frac{f^{(k)}(a)}{k!}(x-a)^k
+\frac{f^{(n+1)}(\xi)}{(n+1)!}(x-a)^{n+1}.}
$$

Here the endpoint [derivatives](../../../../../../derivative.md) are understood as restrictions of derivatives defined near the interval, or as their continuous one-sided extensions. No continuity of $f^{(n+1)}$ is required. For $x=a$ the equality is immediate with zero remainder.

To prove the formula, write the [Taylor polynomial](../../../../../../taylor-polynomial.md) as $P_n(t)=\sum_{k=0}^n f^{(k)}(a)(t-a)^k/k!$ and define

$$
K=\frac{f(x)-P_n(x)}{(x-a)^{n+1}},\qquad
h(t)=f(t)-P_n(t)-K(t-a)^{n+1}.
$$

Then $h(a)=h(x)=0$, and $h^{(j)}(a)=0$ for $j=1,\ldots,n$. The [Rolle theorem](../../../../../../rolle-theorem.md) gives a zero $\xi_1$ of $h'$ strictly between $a$ and $x$. If $n\geq1$, apply the [Rolle theorem](../../../../../../rolle-theorem.md) to $h'$ between $a$ and $\xi_1$, using $h'(a)=0$, to get a zero $\xi_2$ of $h''$. Repeating produces a point $\xi_{n+1}$ strictly between $a$ and $x$ with $h^{(n+1)}(\xi_{n+1})=0$. Each application is justified by continuity on the relevant closed interval and differentiability in its interior; the same construction works when $x<a$.

Since $P_n$ has degree at most $n$,

$$
0=h^{(n+1)}(\xi_{n+1})
=f^{(n+1)}(\xi_{n+1})-(n+1)!K.
$$

Substituting this value of $K$ into its definition proves the displayed [Taylor theorem with Lagrange remainder](../../../../../../taylor-theorem-with-lagrange-remainder.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10F](../../10f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
