<h1 id="13j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $x$ be the parameter-contrast vector for the specified game: it has entries $+1$ for $\beta_i,\beta_j,\beta_{\{i,j\}}$, entries $-1$ for $\beta_k,\beta_\ell,\beta_{\{k,\ell\}}$, and zero elsewhere. Put

$$
\eta=x^T\beta,
\qquad
p=g(\eta)=\frac{e^\eta}{1+e^\eta}.
$$

Under the stated regularity assumptions, [asymptotic normality of a maximum likelihood estimator](../../../../../../asymptotic-normality-of-a-maximum-likelihood-estimator.md) gives

$$
\sqrt N(\widehat\beta-\beta)
\xrightarrow{d}N\!\left(0,I(\beta)^{-1}\right),
$$

where $i_N(\beta)/N\to I(\beta)$. Since $g'(\eta)=p(1-p)$, the [delta method](../../../../../../delta-method.md) gives

$$
\boxed{\sqrt N(\widehat p-p)
\xrightarrow{d}
N\!\left(0,\,[p(1-p)]^2x^TI(\beta)^{-1}x\right).}
$$

Equivalently, for large $N$,

$$
\boxed{\widehat p\ \dot\sim\
N\!\left(p,\,[p(1-p)]^2x^Ti_N(\beta)^{-1}x\right),}
$$

with $p=e^{x^T\beta}/(1+e^{x^T\beta})$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13J](../../13j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
