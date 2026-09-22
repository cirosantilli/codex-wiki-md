<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix $k\geq1$ and write $n=qk+r$ with $1\leq r\leq k$ and $q\geq0$. Repeatedly use the given inequality with its second index equal to $k$. This yields

$$
x_{qk+r}\leq x_r+q(x_k+\alpha_k).
$$

There are only finitely many possible remainders for fixed $k$, so

$$
\limsup_{n\to\infty}\frac{x_n}{n}\leq\frac{x_k+\alpha_k}{k}.
$$

Taking $k=1$ rules out positive infinity for this upper limit. Let $L=\liminf x_n/n$, which may be negative infinity, and choose $k_j\to\infty$ with $x_{k_j}/k_j\to L$. The assumption $\alpha_{k_j}/k_j\to0$ then gives $\limsup x_n/n\leq L$. This also works when $L=-\infty$, by taking an arbitrarily negative upper bound. Therefore the [asymmetrically almost-subadditive sequence](../../../../../../asymmetrically-almost-subadditive-sequence.md) has

$$
\boxed{\lim_{n\to\infty}\frac{x_n}{n}=\gamma\in[-\infty,\infty),\qquad\gamma=\inf_{k\geq1}\frac{x_k+\alpha_k}{k}}.
$$

The last infimum identity follows from the fixed-$k$ bound and from the convergence of the corrected ratios to $\gamma$. No positivity assumption on $\alpha_n$ is required.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
