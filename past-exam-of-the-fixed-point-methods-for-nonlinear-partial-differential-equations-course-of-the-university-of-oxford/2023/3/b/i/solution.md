<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose the real [zero-trace Sobolev space](../../../../../zero-trace-sobolev-space.md)

$$
X=W_0^{1,4}(\Omega),\qquad\|u\|_X=\|\nabla u\|_4,
\qquad Y=L^{8/7}(\Omega).
$$

The [Poincaré inequality](../../../../../poincare-inequality.md) makes this an equivalent [Sobolev norm](../../../../../sobolev-norm.md). Since the dimension is five, the [Sobolev conjugate exponent](../../../../../sobolev-conjugate-exponent.md) is $4^*=5\cdot4/(5-4)=20$. The [Sobolev embedding theorem](../../../../../sobolev-embedding-theorem.md) gives $X\hookrightarrow L^{20}(\Omega)$ continuously. Boundedness of $\Omega$ and [Lp inclusion on a finite measure space](../../../../../lp-inclusion-on-a-finite-measure-space.md) then give $X\hookrightarrow L^8(\Omega)$ continuously, say $\|u\|_8\leq C_8\|u\|_X$.

For $f\in Y$, the [weak formulation](../../../../../weak-formulation.md) is

$$
\boxed{u\in X,\qquad
\int_\Omega |\nabla u|^2\nabla u\cdot\nabla v\,dx
+\int_\Omega u^7v\,dx=\int_\Omega fv\,dx
\quad\forall v\in X.}
$$

The zero [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) is imposed through the [Sobolev trace](../../../../../trace-operator.md). [Hölder's inequality](../../../../../holder-s-inequality.md) verifies every term:

$$
\begin{aligned}
\left|\int_\Omega|\nabla u|^2\nabla u\cdot\nabla v\,dx\right|
&\leq\|\nabla u\|_4^3\|\nabla v\|_4,\\
\left|\int_\Omega u^7v\,dx\right|
&\leq\|u\|_8^7\|v\|_8,\\
\left|\int_\Omega fv\,dx\right|
&\leq\|f\|_{8/7}\|v\|_8.
\end{aligned}
$$

Thus $|\nabla u|^2\nabla u\in L^{4/3}(\Omega;\mathbb R^5)$, while $u^7\in L^{8/7}(\Omega)$, and all three pairings are finite bounded [linear functionals](../../../../../linear-functional.md) in $v$. The choice $Y=L^{8/7}(\Omega)$ is sufficient; it is not intended to be the largest possible space of data.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../split.md)
6. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
