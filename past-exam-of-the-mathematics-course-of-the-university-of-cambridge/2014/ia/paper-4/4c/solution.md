<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

A [four-vector](../../../../../four-vector.md) is a collection of four components $A^\mu=(A^0,\mathbf A)$ that transforms by the same [Lorentz transformation](../../../../../lorentz-transformation.md) as $(ct,\mathbf x)$. Use the [metric signature](../../../../../metric-signature.md) $(-,+,+,+)$. The [Lorentzian inner product](../../../../../lorentzian-inner-product.md) is

$$
A\cdot B=-A^0B^0+A^1B^1+A^2B^2+A^3B^3.
$$

A nonzero [four-vector](../../../../../four-vector.md) is a [timelike vector](../../../../../timelike-vector.md), [null vector](../../../../../null-vector.md) or [spacelike vector](../../../../../spacelike-vector.md) according as $A\cdot A$ is negative, zero or positive. Reversing the [metric signature](../../../../../metric-signature.md) reverses the signs used to name these three classes, without changing their geometric meaning.

For a frame moving at [speed](../../../../../speed.md) $v$ along the positive $x$ axis, write $\beta=v/c$ and use the [Lorentz factor](../../../../../lorentz-factor.md) $\gamma=(1-\beta^2)^{-1/2}$. The component [Lorentz transformation](../../../../../lorentz-transformation.md) is

$$
\boxed{A'^0=\gamma(A^0-\beta A^1),\quad A'^1=\gamma(A^1-\beta A^0),\quad A'^2=A^2,\quad A'^3=A^3.}
$$

Expanding the first two squares gives

$$
-(A'^0)^2+(A'^1)^2=\gamma^2(1-\beta^2)\bigl(-(A^0)^2+(A^1)^2\bigr)=-(A^0)^2+(A^1)^2.
$$

The other two components are unchanged, so $A'\cdot A'=A\cdot A$. Consequently **a [timelike vector](../../../../../timelike-vector.md) remains timelike under a [Lorentz transformation](../../../../../lorentz-transformation.md)**.

For a nonzero [null vector](../../../../../null-vector.md), $|\mathbf A|=|A^0|$ and $A^0\ne0$. Set $a=A^0$ and $\hat{\mathbf n}=\mathbf A/a$. Then $|\hat{\mathbf n}|=1$ and $A=a(1,\hat{\mathbf n})$. If the zero [four-vector](../../../../../four-vector.md) is included among [null vectors](../../../../../null-vector.md), take $a=0$ and any [unit vector](../../../../../unit-vector.md).

For two future-pointing [null vectors](../../../../../null-vector.md), write $A=a(1,\hat{\mathbf n})$ and $B=b(1,\hat{\mathbf m})$ with $a,b>0$. The [sum of future-pointing null vectors](../../../../../sum-of-future-pointing-null-vectors.md) satisfies

$$
(A+B)\cdot(A+B)=-2ab\bigl(1-\hat{\mathbf n}\cdot\hat{\mathbf m}\bigr)\leq0,
$$

because the ordinary [inner product](../../../../../inner-product.md) of two [unit vectors](../../../../../unit-vector.md) is at most one. **The sum is null if their spatial directions coincide, and timelike otherwise.** Its positive time component makes the sum nonzero and future-pointing.

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
