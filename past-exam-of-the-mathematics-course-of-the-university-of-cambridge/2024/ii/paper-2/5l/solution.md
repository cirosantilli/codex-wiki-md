<h1 id="5l/solution">Solution</h1>

↑ **Parent:** [5L](../5l.md)

Put $K=nY$. Apart from a factor independent of $p$, the likelihood is

$$
L(p)=p^{nY}(1-p)^{n(1-Y)}.
$$

Thus the [score function](../../../../../informant-function.md) and [Fisher information matrix](../../../../../fisher-information-matrix.md) are

$$
S(p)=\ell'(p)=n\left(\frac Yp-\frac{1-Y}{1-p}\right)
=\frac{n(Y-p)}{p(1-p)},
\qquad
I(p)=\frac n{p(1-p)}.
$$

The [Newton method](../../../../../newton-s-method-in-optimization.md) and [Fisher scoring](../../../../../scoring-algorithm.md) updates are respectively

$$
p^{(r+1)}=p^{(r)}-\frac{\ell'(p^{(r)})}{\ell''(p^{(r)})},
\qquad
p^{(r+1)}=p^{(r)}+I(p^{(r)})^{-1}S(p^{(r)}).
$$

Since $\widehat p=Y$, initialization at $p^{(0)}=Y$ requires zero steps for either algorithm. Moreover,

$$
p+I(p)^{-1}S(p)=p+\frac{p(1-p)}n\frac{n(Y-p)}{p(1-p)}=Y,
$$

so [binomial-proportion Fisher scoring](../../../../../binomial-proportion-fisher-scoring.md) reaches the MLE in one step from every interior $p^{(0)}\ne Y$.

## ↑ Ancestors (10)

1. [5L](../5l.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
