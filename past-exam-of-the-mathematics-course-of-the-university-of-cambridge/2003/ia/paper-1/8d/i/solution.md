<h1 id="8d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $q=u\cdot v$ and $d=u+v$. The [linear independence](../../../../../../linear-independence.md) assumption implies $d\ne0$. Since $w$ is a [unit vector](../../../../../../unit-vector.md), the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
S=q+w\cdot d\ge q-\|d\|.
$$

Equality holds exactly when $w$ points opposite to $d$. Its required unit length then fixes the scale:

$$
\boxed{w=-\frac{u+v}{\|u+v\|},\qquad\lambda=-\frac1{\|u+v\|}=-\frac1{\sqrt{2+2q}}.}
$$

Here $\|u+v\|^2=2+2q$ because both vectors have unit norm. The minimizing vector is unique, and the [minimum pairwise dot-product sum of three unit vectors](../../../../../../minimum-pairwise-dot-product-sum-of-three-unit-vectors.md) for these fixed $u,v$ is

$$
\boxed{S_{\min}=q-\sqrt{2+2q}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [8D](../../8d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
