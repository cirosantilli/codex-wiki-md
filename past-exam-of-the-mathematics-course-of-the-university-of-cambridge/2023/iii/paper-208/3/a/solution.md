<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $X_1,\ldots,X_n$ be [independent random variables](../../../../../../independent-random-variables.md), let $f=f(X_1,\ldots,X_n)$, and let each $f_i$ depend on every coordinate except $X_i$. The [modified logarithmic Sobolev inequality](../../../../../../modified-logarithmic-sobolev-inequality.md) states that, for every real $\lambda$ for which the expectations exist,

$$
\operatorname{Ent}(e^{\lambda f})
\leq\mathbb E\left[e^{\lambda f}\sum_{i=1}^n
\phi\bigl(-\lambda(f-f_i)\bigr)\right],
\qquad
\phi(u)=e^u-u-1.
$$

To prove it, first apply [tensorization of entropy](../../../../../../tensorization-of-entropy.md):

$$
\operatorname{Ent}(e^{\lambda f})
\leq\sum_{i=1}^n\mathbb E\!\left[
\operatorname{Ent}_{X_i}(e^{\lambda f})
\right].
$$

Condition on all coordinates except $X_i$ and use the stated variational formula with the admissible constant $u=e^{\lambda f_i}$. The $i$th conditional entropy is at most

$$
\begin{aligned}
\mathbb E_{X_i}\!\left[
e^{\lambda f}(\lambda f-\lambda f_i)
-(e^{\lambda f}-e^{\lambda f_i})
\right]
&=\mathbb E_{X_i}\!\left[
e^{\lambda f}\phi\bigl(-\lambda(f-f_i)\bigr)
\right].
\end{aligned}
$$

Summing and taking the remaining expectations proves the inequality.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
