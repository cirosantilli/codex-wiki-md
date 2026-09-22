<h1 id="11e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Rotate the disc so that $P=r\in(0,1)$ lies on the positive real axis. From part (b), the perpendicular hyperbolic line $\ell$ is a Euclidean circle orthogonal to the unit circle, with centre $c>1$ on the real axis and radius $R=c-r$. Orthogonality of the two circles gives

$$
c^2=1+R^2.
$$

Combining the two equations yields

$$
c=\frac{1+r^2}{2r},
\qquad
R=\frac{1-r^2}{2r}.
$$

The radial distance formula from part (b) says

$$
\rho=2\operatorname{artanh}r,
\qquad r=\tanh(\rho/2).
$$

The hyperbolic double-angle identities now give

$$
\sinh\rho=\frac{2r}{1-r^2},
\qquad
\tanh\rho=\frac{2r}{1+r^2}.
$$

Therefore

$$
\boxed{R=\frac1{\sinh\rho},
\qquad c=\frac1{\tanh\rho}}.
$$

This is the [Euclidean circle representing a perpendicular hyperbolic line](../../../../../../euclidean-circle-representing-a-perpendicular-hyperbolic-line.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11E](../../11e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
