<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $z(x,y)=Z(r,s)$ in the new [coordinates](../../../../../coordinate-linear-algebra.md). Since

$$
\partial_x=\partial_r-\partial_s,\qquad \partial_y=\partial_r+\partial_s,
$$

the [partial differential equation](../../../../../partial-differential-equation-split.md) becomes

$$
z_{xx}-z_{yy}=-4Z_{rs}=0.
$$

For a twice continuously differentiable [solution of a differential equation](../../../../../solution-of-a-differential-equation.md), $Z_r$ is independent of $s$, so [integration](../../../../../integral-split.md) first in $r$ and then in $s$ gives

$$
\boxed{z(x,y)=\phi(y+x)+\psi(y-x).}
$$

This is the decomposition of the [one-dimensional wave equation](../../../../../one-dimensional-wave-equation.md) into waves traveling in opposite directions.

The first [initial condition](../../../../../initial-condition.md) gives $\phi(y)+\psi(y)=\cos y$. The second [initial condition](../../../../../initial-condition.md) gives $\phi'(y)-\psi'(y)=0$. Differentiating the first relation and combining the two relations yields $\phi'=psi'=-\tfrac12\sin y$. Thus $\phi(y)=\tfrac12\cos y+C$ and $\psi(y)=\tfrac12\cos y-C$. The constants cancel, and the [cosine addition formula](../../../../../cosine-addition-formula.md) gives

$$
\boxed{z(x,y)=\frac{\cos(y+x)+\cos(y-x)}2=\cos x\cos y.}
$$

Both [initial conditions](../../../../../initial-condition.md) and the [partial differential equation](../../../../../partial-differential-equation-split.md) follow directly by differentiation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
