<h1 id="22h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $e_m$ denote the sequence with a one in coordinate $m$ and zeros elsewhere.

For $T_1$, one has $\lVert e_m\rVert_p=1$ but $\lVert T_1e_m\rVert_p=m$ for every $p$, including $p=\infty$. Thus $T_1$ is unbounded for every $p$.

For $T_2$, the sequence $T_2e_m$ has entries $-(m-1)$ and $m$ in coordinates $m-1$ and $m$, respectively. Hence $\lVert T_2e_m\rVert_p\geq m$, so $T_2$ is also unbounded for every $p$.

For $T_3$, coordinatewise division gives

$$
\lVert T_3x\rVert_p\leq\lVert x\rVert_p
$$

for every $1\leq p\leq\infty$. Thus $T_3$ is a bounded [diagonal operator on sequence space](../../../../../../diagonal-operator-on-sequence-space.md) for every $p$.

For $T_4$, write $a=(n^{-1/2})_{n\geq1}$. Then $T_4x=x_1a$, and coordinate evaluation satisfies $|x_1|\leq\lVert x\rVert_p$. By the [p-series](../../../../../../p-series.md) criterion, $a\in\ell^p$ exactly when $p>2$, while $a\in\ell^\infty$. Therefore $T_4$ is bounded precisely for

$$
2<p\leq\infty.
$$

For $p\leq2$, even $T_4e_1$ does not belong to $\ell^p$.

For $T_5$, let $q$ be the [Holder conjugate exponent](../../../../../../conjugate-exponents.md) of $p$. [Holder inequality](../../../../../../holder-inequality.md) gives, for finite $p$,

$$
\left|\sum_{j=1}^nx_j\right|
\leq n^{1/q}\lVert x\rVert_p,
$$

and consequently

$$
\lVert T_5x\rVert_p^p
\leq\lVert x\rVert_p^p
\sum_{n=1}^{\infty}\frac{n^{p/q}}{2^{np}}<\infty.
$$

For $p=\infty$,

$$
|(T_5x)_n|\leq\frac n{2^n}\lVert x\rVert_\infty
\leq\lVert x\rVert_\infty.
$$

Thus $T_5$ is bounded for every $1\leq p\leq\infty$. Altogether,

$$
\boxed{
\begin{array}{c|ccccc}
&T_1&T_2&T_3&T_4&T_5\\ \hline
\text{bounded on }\ell^p
&\text{never}&\text{never}&\text{all }p&2<p\leq\infty&\text{all }p
\end{array}}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22H](../../22h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
