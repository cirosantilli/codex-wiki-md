<h1 id="32e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For

$$
V=4t^2\partial_t+4tx\partial_x-(x^2+2t)\partial_u,
$$

the flow equations are

$$
\frac{dT}{d\epsilon}=4T^2,
\qquad
\frac{dX}{d\epsilon}=4TX,
\qquad
\frac{dU}{d\epsilon}=-(X^2+2T),
$$

with $(T,X,U)=(t,x,u)$ at $\epsilon=0$. Solving the first two gives, with $d=1-4\epsilon t$,

$$
T=\frac td,
\qquad X=\frac xd.
$$

Integrating the last equation then gives the one-parameter group

$$
\boxed{
T=\frac{t}{1-4\epsilon t},
\qquad
X=\frac{x}{1-4\epsilon t},
\qquad
U=u-\frac{\epsilon x^2}{1-4\epsilon t}
+\frac12\log(1-4\epsilon t),}
$$

defined locally where $1-4\epsilon t>0$.

To verify the symmetry infinitesimally, use

$$
\xi^t=4t^2,
\qquad \xi^x=4tx,
\qquad \eta=-(x^2+2t).
$$

The needed coefficients of the [second prolongation of a Lie point symmetry](../../../../../../second-prolongation-of-a-lie-point-symmetry.md) are

$$
\eta^t=-2-8tu_t-4xu_x,
\qquad
\eta^x=-2x-4tu_x,
$$

and

$$
\eta^{xx}=-2-8tu_{xx}.
$$

For the [potential Burgers equation](../../../../../../potential-burgers-equation.md) written as

$$
F=u_t-u_{xx}-u_x^2=0,
$$

we obtain

$$
\begin{aligned}
\operatorname{pr}^{(2)}V(F)
&=\eta^t-\eta^{xx}-2u_x\eta^x\\
&=-8t(u_t-u_{xx}-u_x^2)\\
&=-8tF.
\end{aligned}
$$

**Thus the prolonged generator is tangent to the solution manifold $F=0$, and the finite transformations above form the [projective Lie symmetry of the potential Burgers equation](../../../../../../projective-lie-symmetry-of-the-potential-burgers-equation.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [32E](../../32e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
