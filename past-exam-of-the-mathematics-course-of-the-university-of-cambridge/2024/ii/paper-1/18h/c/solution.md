<h1 id="18h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\beta$ satisfy $\beta^p=\alpha$. Since $K=\mathbb Q(\alpha)\subseteq\mathbb Q(\beta)$,

$$
[\mathbb Q(\beta):\mathbb Q]=[K(\beta):K][K:\mathbb Q].
$$

The [polynomial](../../../../../../polynomial-split.md) $f(X^p)$ has degree $p[K:\mathbb Q]$ and has root $\beta$. It is irreducible exactly when $[K(\beta):K]=p$.

If $\alpha=\gamma^p$ for some $\gamma\in K$, then $\gamma$ is a root of $f(X^p)$ of degree at most $[K:\mathbb Q]$, so $f(X^p)$ is reducible. Conversely, if it is reducible, then

$$
d=[K(\beta):K]<p.
$$

Since $p$ is prime, $1\leq d<p$ implies $\gcd(d,p)=1$. Applying [coprime-degree descent for powers](../../../../../../coprime-degree-descent-for-powers.md) to $K(\beta)/K$ and $\beta^p=\alpha$ shows that $\alpha$ is a $p$th power in $K$. Hence

$$
\boxed{f(X^p)\text{ is irreducible}\quad\Longleftrightarrow\quad
\alpha\notin K^p.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18H](../../18h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
