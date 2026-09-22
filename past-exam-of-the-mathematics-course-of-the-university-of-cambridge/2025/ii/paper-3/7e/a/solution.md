<h1 id="7e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\operatorname{Re}z>0$, absolute convergence permits the double-integral calculation

$$
\Gamma(z)^2
=\int_0^\infty\int_0^\infty
e^{-(s+t)}s^{z-1}t^{z-1}\,ds\,dt.
$$

Put $r=s+t$ and $u=t/(s+t)$, so $s=r(1-u)$, $t=ru$, and the Jacobian has magnitude $r$. The first quadrant becomes $r>0$, $0<u<1$, and therefore

$$
\begin{aligned}
\Gamma(z)^2
&=\int_0^\infty e^{-r}r^{2z-1}\,dr
\int_0^1(1-u)^{z-1}u^{z-1}\,du\\
&=\Gamma(2z)B(z,z).
\end{aligned}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7E](../../7e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
