<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

This is an [asymmetrically almost-subadditive sequence](../../../../../../asymmetrically-almost-subadditive-sequence.md). The limit must be allowed to take the value $-\infty$; the stated hypotheses alone do not imply a finite real limit. Define

$$
I=\inf_{k\ge1}\frac{x_k+\alpha_k}{k}\in[-\infty,\infty).
$$

Fix $k$, and write $N=qk+r$ with $1\le r\le k$. Repeatedly apply the given inequality with the first summand equal to $k$. Induction gives

$$
x_N\le q(x_k+\alpha_k)+x_r.
$$

For fixed $k$, there are only finitely many possible residual terms $x_r$, so division by $N$ and passage to the upper limit yield

$$
\limsup_{N\to\infty}\frac{x_N}{N}\le\frac{x_k+\alpha_k}{k}.
$$

This holds for every $k$, and therefore the upper limit is at most $I$. If $I$ is finite, its definition also gives $x_N/N\ge I-\alpha_N/N$, so the lower limit is at least $I$ because $\alpha_N/N\to0$. If $I=-\infty$, the upper bound by every $(x_k+\alpha_k)/k$ makes the upper limit $-\infty$ directly. Thus in both cases

$$
\boxed{\lambda=\lim_{N\to\infty}\frac{x_N}{N}=\inf_{k\ge1}\frac{x_k+\alpha_k}{k}.}
$$

In particular,

$$
\boxed{x_n\ge n\lambda-\alpha_n.}
$$

When $\lambda=-\infty$ this inequality is interpreted in the extended-real sense. For example, $x_n=-n^2$ and $\alpha_n=0$ satisfy the assumptions but have normalized limit $-\infty$. A finite-limit assertion would need an additional lower linear bound.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
