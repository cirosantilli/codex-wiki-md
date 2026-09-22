<h1 id="a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The solution is the continuous [Doléans-Dade exponential](../../../../../doleans-dade-exponential.md):

$$
\boxed{S_t=\exp\{X_t-X_0-\tfrac12[X]_t\}.}
$$

Here $[X]$ is the continuous [quadratic variation](../../../../../quadratic-variation.md) starting from zero, denoted by the angle-bracket notation in the source. If $X=M+A$ with $A$ continuous of finite variation, then $[X]=[M]$.

Set $U=X-X_0-\frac12[X]$. Its quadratic variation is still $[X]$. Applying [Itô's formula](../../../../../ito-s-lemma.md) to $e^U$ gives

$$
dS=S\,dU+\tfrac12S\,d[U]
=S\,dX-\tfrac12S\,d[X]+\tfrac12S\,d[X]=S\,dX.
$$

The initial value is $S_0=1$. This verification applies to the full semimartingale, including its finite-variation part.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
