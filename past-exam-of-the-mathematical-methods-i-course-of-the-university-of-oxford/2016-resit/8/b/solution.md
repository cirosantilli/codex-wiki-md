<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The given particular solution $y_p=x^2$ suggests the standard reduction of a [Riccati equation](../../../../riccati-equation.md). Substitution of $y=x^2+1/v$ gives

$$
-2x^3v'=5x^2v+2,
\qquad v'+\frac{5}{2x}v=-\frac1{x^3}.
$$

On either side of $x=0$, an [integrating factor](../../../../integrating-factor.md) is $|x|^{5/2}$, so $v=(C-2\sqrt{|x|})/|x|^{5/2}$. Hence

$$
\boxed{y=x^2\frac{C-\sqrt{|x|}}{C-2\sqrt{|x|}},}
$$

along with the separately recovered particular solution $y=x^2$. The denominator must remain nonzero on the solution interval; $x=0$ is a singular point of the divided differential equation.

For the positive-$x$ branch, $y(1)=(C-1)/(C-2)$ and $y(4)=16(C-2)/(C-4)$. Nonsingular endpoint values exclude $C=2,4$, so

$$
\boxed{y(4)\bigl(3-2y(1)\bigr)=16.}
$$

The particular solution $y=x^2$ gives the same value directly. These evaluations concern one solution branch, with a common integration constant, rather than independently chosen solutions at the two points.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [2016 resit](../../../2016-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
