<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $x_1=t$, $x_2=t^2$. The two inactive constraints are strict exactly for $-2<t<2$. [Complementary slackness](../../../../complementary-slackness.md) gives $\lambda_1=\lambda_2=0$. The [KKT conditions](../../../../karush-kuhn-tucker-conditions.md) reduce to

$$
4t^2-2t\lambda_3=0,\qquad t+2t^2+\lambda_3=0,\qquad\lambda_3\geq0.
$$

If $t=0$ these give $\lambda_3=0$. Otherwise $\lambda_3=2t$ and $t=-3/2$, which gives a negative multiplier and is inadmissible. Therefore

$$
\boxed{x=(0,0),\qquad\lambda=(0,0,0)}
$$

is the only [KKT point](../../../../kkt-point.md) with this active set. Its active [gradient](../../../../gradient.md) $(0,1)$ is nonzero, so the [linear independence constraint qualification](../../../../linear-independence-constraint-qualification.md), and hence the [Mangasarian–Fromovitz constraint qualification](../../../../mangasarian-fromovitz-constraint-qualification.md), holds.

It is **not a local maximizer**: $(0,\varepsilon)$ is feasible for small $\varepsilon>0$ and has objective $\varepsilon^2>0=F(0,0)$. The feasible boundary path $(t,t^2)$ for small negative $t$ has objective $2t^3+t^4<0$, so it is not a local minimizer either.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
