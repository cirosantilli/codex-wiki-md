<h1 id="23h/solution">Solution</h1>

↑ **Parent:** [23H](../23h.md)

In local coordinates around $p\in R$ and $f(p)\in S$, a nonconstant analytic map has the form

$$
f(z)-f(p)=z^m h(z),\qquad h(0)\ne0.
$$

After shrinking the chart, $h$ has an analytic $m$th root, so a change of coordinate makes the map $z\mapsto z^m$. It maps small discs onto neighborhoods of the origin; hence every nonconstant analytic map of Riemann surfaces is open. If $R$ is compact and $S$ connected, $f(R)$ is compact and therefore closed, and it is also nonempty and open. Thus $f(R)=S$.

For $f:\mathbb D\to\mathbb D$ with $f(0)=0$, the removable-singularity theorem makes $g=f/z$ analytic. On $|z|=r$, $|g(z)|=|f(z)|/r\leq1/r$, and the maximum principle gives the same bound throughout $\mathbb D_r$. Applying the [Schwarz lemma](../../../../../schwarz-lemma.md) to an automorphism $h$ and to $h^{-1}$ shows that every automorphism fixing zero is

$$
h(z)=e^{i\theta}z.
$$

If $F:\mathbb C\to\mathbb C$ is an analytic isomorphism fixing zero, continuity of $F^{-1}$ implies that the preimage of every closed disc is compact. Hence $|F(z)|\to\infty$ as $|z|\to\infty$, and defining $F(\infty)=\infty$ gives an analytic isomorphism of the Riemann sphere.

Consequently an automorphism of $\mathbb D$ fixing zero does extend to $\mathbb C$. A general disc automorphism need not: for $a\ne0$,

$$
\frac{z-a}{1-\bar a z}
$$

has a finite pole and cannot extend to an entire isomorphism.

## ↑ Ancestors (10)

1. [23H](../23h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
