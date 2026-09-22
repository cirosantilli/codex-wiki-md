<h1 id="a/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $f(z)=\sin z$, $f'(z)=\cos z$ and $f''(z)=-\sin z$. [Itô's formula](../../../../../ito-s-lemma.md) gives

$$
d\sin(B_t)=\cos(B_t)\,dB_t-\tfrac12\sin(B_t)\,dt.
$$

Since $B_0=0$, this is exactly

$$
\boxed{dX_t=\cos B_t\,dB_t-\tfrac12X_t\,dt,\qquad X_0=0.}
$$

The integrand retains $\cos B_t$; replacing it by a fixed sign of $\sqrt{1-X_t^2}$ would lose information about the phase of $B_t$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
