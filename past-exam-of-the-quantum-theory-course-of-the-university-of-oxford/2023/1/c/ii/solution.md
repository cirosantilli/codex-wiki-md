<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For an arc represented by $0\leq x\leq a$, take $0\leq a\leq2\pi R$. The [Born rule](../../../../../born-rule.md) uses

$$
|\Psi(t,x)|^2=\frac1{\pi R}\cos^2\!\left(\frac{2(x+s\tau)}R\right),\qquad \tau=t-T.
$$

Integrate using $\cos^2u=(1+\cos2u)/2$:

$$
\boxed{\begin{aligned}
\Pr(0\leq x\leq a)&=\frac1{\pi R}\int_0^a\cos^2\!\left(\frac{2(x+s\tau)}R\right)dx\\
&=\frac{a}{2\pi R}+\frac1{8\pi}
\left[\sin\!\left(\frac{4(a+s\tau)}R\right)-\sin\!\left(\frac{4s\tau}R\right)\right].
\end{aligned}}
$$

The result is zero at $a=0$ and one at $a=2\pi R$, checking the [wavefunction normalization](../../../../../wavefunction-normalization.md). At $s=0$ it reduces to $a/(2\pi R)+\sin(4a/R)/(8\pi)$, the stationary position [probability](../../../../../probability.md). Longer intervals on the periodically identified coordinate require specifying the corresponding subset of the circle; integrating multiple turns would count the same positions repeatedly.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the quantum theory course of the University of Oxford](../../../../split.md)
6. [Quantum theory course of the University of Oxford](../../../../../quantum-theory-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
