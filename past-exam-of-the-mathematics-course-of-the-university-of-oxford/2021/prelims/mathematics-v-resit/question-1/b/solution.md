<h1 id="question-1/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

Express the [position vector](../../../../../../position-vector.md) in the suggested [orthonormal basis](../../../../../../orthonormal-basis.md) as $\mathbf r=X\mathbf e_1+Y\mathbf e_2+Z\mathbf e_3$. Then

$$
x=\frac{-X+Z}{\sqrt2},\qquad
y=\frac{-X-Z}{\sqrt2},\qquad z=Y.
$$

This [orthogonal transformation](../../../../../../orthogonal-transformation.md) preserves $x^2+y^2+z^2=X^2+Y^2+Z^2$ and has [Jacobian determinant](../../../../../../jacobian-determinant.md) of absolute value one, so $dV=dX\,dY\,dZ$. The basis actually reverses [orientation](../../../../../../orientation-of-a-simplex.md); the absolute value of the [Jacobian determinant](../../../../../../jacobian-determinant.md) is why no minus sign enters the [volume integral](../../../../../../volume-integral.md). Also $x-y=\sqrt2 Z$, so the [half-space](../../../../../../half-space.md) becomes $Z\geq1/2$.

At each fixed $Z\in[1/2,1]$, the section is the [disk](../../../../../../disk-mathematics.md) $X^2+Y^2\leq1-Z^2$, of [area](../../../../../../surface-area.md) $\pi(1-Z^2)$. Its [reflection symmetry](../../../../../../reflection-symmetry.md) in $X$ makes the [integral](../../../../../../integral-split.md) of $X$ vanish. Hence the required [triple integral](../../../../../../triple-integral.md) is

$$
\begin{aligned}
I&=-\frac1{\sqrt2}\int_{1/2}^1
\iint_{X^2+Y^2\leq1-Z^2}(X+Z)\,dX\,dY\,dZ\\
&=-\frac\pi{\sqrt2}\int_{1/2}^1Z(1-Z^2)\,dZ
=-\frac\pi{\sqrt2}\left[\frac{Z^2}2-\frac{Z^4}4\right]_{1/2}^1
=\boxed{-\frac{9\pi}{64\sqrt2}}.
\end{aligned}
$$

The negative sign is also consistent with the cap lying in the direction $(1,-1,0)$, where its average $y$ coordinate is negative.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [Question 1](../../question-1.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
