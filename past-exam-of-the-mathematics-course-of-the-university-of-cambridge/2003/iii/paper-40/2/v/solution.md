<h1 id="2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

At the last observed failure time $a_*$, any individual still in the [risk set](../../../../../../risk-set.md) must either fail there or be censored there or later. If there are no such censored observations, every remaining individual fails, so $d_*=r_*$. Thus the final [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md) factor is zero, while the final [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md) jump is one:

$$
\boxed{\widehat H_{\rm KM}(a_*)=+\infty,\qquad \widehat H_{\rm NA}(a_*)=\sum_{a_m\le a_*}\frac{d_m}{r_m}<\infty.}
$$

There is no small-jump approximation at this endpoint. Without ties the final [risk set](../../../../../../risk-set.md) has size one, so the same discrepancy follows from its last single failure.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [2](../../2.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
