<h1 id="differential-equations/9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Integrating the complex exponential and taking its even and odd combinations gives the standard [Laplace transforms](../../../../../laplace-transform.md)

$$
\boxed{\mathcal L[a_1](p)=\frac p{p^2+\omega^2},\qquad
\mathcal L[a_2](p)=\frac\omega{p^2+\omega^2}.}
$$

For example, $\mathcal L[e^{i\omega t}]=(p-i\omega)^{-1}$ for $\operatorname{Re}p>0$, and the real sine and cosine identities follow by combining the two signs of $i\omega$.

Apply part (a) once to the cosine transform and twice to the sine transform:

$$
\begin{aligned}
\mathcal L[a_3](p)&=-\frac d{dp}\frac p{p^2+\omega^2}
=\boxed{\frac{p^2-\omega^2}{(p^2+\omega^2)^2}},\\
\mathcal L[a_4](p)&=\frac{d^2}{dp^2}\frac\omega{p^2+\omega^2}
=\boxed{\frac{2\omega(3p^2-\omega^2)}{(p^2+\omega^2)^3}}.
\end{aligned}
$$

All four transforms are valid on the stated right half-plane.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [9](../../9.md)
3. [Differential Equations](../../../differential-equations.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
