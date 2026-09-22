<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Applying the stage equations to $y'=\lambda y$ gives the [stability function](../../../../../../stability-function.md)

$$
R(z)=1+zb^T(I-zA)^{-1}\mathbf1
=\frac{1+z/2+z^2/12}{1-z/2+z^2/12},\qquad z=h\lambda.
$$

The poles are $3\pm i\sqrt3$, both in the right half-plane. To determine the whole domain rather than only its boundary, multiply numerator and denominator by 12 and put $z=x+iy$. Direct expansion gives

$$
|z^2-6z+12|^2-|z^2+6z+12|^2=-24x(|z|^2+12).
$$

Thus $|R(z)|\leq1$ exactly when $x\leq0$, with no pole in that set. Consequently

$$
\boxed{\mathcal D=\{z:\operatorname{Re}z\leq0\},\qquad\text{the method is A-stable}.}
$$

On the imaginary axis $|R|=1$, and in the open left half-plane it is less than one. Its limit along the negative real axis is one, so [A-stability](../../../../../../a-stability.md) here does not imply stiff decay or [L-stability](../../../../../../l-stability.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
