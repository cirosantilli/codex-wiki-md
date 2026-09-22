<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Brouwer fixed-point theorem](../../../../brouwer-fixed-point-theorem.md) says that every [continuous map](../../../../continuous-map.md) $T:\overline B_R(0)\to\overline B_R(0)$ has a [fixed point](../../../../fixed-point.md). To use the supplied [outward vector field zero theorem](../../../../outward-vector-field-zero-theorem.md), first extend the construction to all of $\mathbb R^n$. Let

$$
P_R(x)=\begin{cases}x,&|x|\leq R,\\Rx/|x|,&|x|>R,\end{cases}\qquad g(x)=x-T(P_R(x)).
$$

The [radial retraction onto a closed ball](../../../../radial-retraction-onto-a-closed-ball.md) $P_R$ is continuous, so $g$ is a continuous vector field on the required whole space. On $|x|=R$, the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) gives

$$
g(x)\cdot x=R^2-T(x)\cdot x\geq R^2-|T(x)|R\geq0.
$$

The supplied theorem gives $g(x_0)=0$ with $|x_0|\leq R$. There $P_R(x_0)=x_0$, hence $\boxed{T(x_0)=x_0}$. This explicit extension avoids presuming that the original map $T$ was defined outside the ball.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../split.md)
5. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
