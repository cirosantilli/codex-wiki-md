<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $\sigma=\operatorname{sgn}(x_S)$ and $G=A_S^*A_S$. The [injectivity](../../../../../../injective-function.md) of $A_S$ makes this [Gram matrix](../../../../../../gram-matrix.md) a [positive-definite matrix](../../../../../../positive-definite-matrix.md), since $u^*Gu=\|A_Su\|_2^2>0$ for $u\ne0$. Thus its [matrix inverse](../../../../../../matrix-inverse.md) exists. Construct the [least-norm dual certificate](../../../../../../least-norm-dual-certificate.md)

$$
\boxed{h=A_S(A_S^*A_S)^{-1}\sigma.}
$$

On the active coordinates, $A_S^*h=G G^{-1}\sigma=\sigma$. For $l\notin S$, symmetry of the real [Gram matrix](../../../../../../gram-matrix.md) and its [matrix inverse](../../../../../../matrix-inverse.md) gives

$$
(A^*h)_l=a_l^*A_SG^{-1}\sigma=\langle G^{-1}A_S^*a_l,\sigma\rangle.
$$

Condition (iii) makes the [absolute value](../../../../../../absolute-value.md) of this coordinate strictly less than one. Consequently $h$ is a [strict dual certificate for basis pursuit](../../../../../../strict-dual-certificate-for-basis-pursuit.md), and part (c) applies. If $S$ is empty, take $h=0$; the zero [vector](../../../../../../vector.md) uniquely minimizes the [L1 norm](../../../../../../l1-norm.md) on its feasible set. **Condition (iii) supplies an explicit certificate and therefore unique recovery.** There is no claim that this particular [least-norm dual certificate](../../../../../../least-norm-dual-certificate.md) is necessary: other valid certificates may exist when this one fails.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
