<h1 id="11/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the [imaginary part](../../../../imaginary-part.md) of [De Moivre's theorem](../../../../de-moivre-s-theorem.md) at exponent five. Writing $s=\sin\theta$ and $c=\cos\theta$ gives

$$
\sin5\theta=5c^4s-10c^2s^3+s^5
=5s(1-s^2)^2-10s^3(1-s^2)+s^5
=16s^5-20s^3+5s.
$$

For real $x\in[-1,1]$, put $x=\sin\theta$. The equation becomes $\sin5\theta=1$, so $\theta=\pi/10+2\pi k/5$. The distinct sine values are $1$, $(\sqrt5-1)/4$, and $-(1+\sqrt5)/4$. To establish completeness over the complex numbers as well, factor the polynomial:

$$
16x^5-20x^3+5x-1=(x-1)(4x^2+2x-1)^2.
$$

Thus all [polynomial roots](../../../../root-of-a-polynomial.md), including their [multiplicities](../../../../multiplicity-mathematics.md), are

$$
\boxed{x=1\ \text{(simple)},\qquad
x=\frac{-1+\sqrt5}{4},\ \frac{-1-\sqrt5}{4}\ \text{(each double)}.}
$$

The repeated sine values account for the double roots; there are no additional nonreal roots hidden by the trigonometric parametrization.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [11](../../11.md)
3. [2013 resit](../../../2013-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
