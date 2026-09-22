<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $u_i=U_i+u_i'$ and $p=P+p'$, with $\overline{u_i'}=\overline{p'}=0$. Assume a statistically stationary mean and sufficient regularity for [Reynolds averaging](../../../../../reynolds-averaging.md) to commute with spatial [derivatives](../../../../../derivative.md). Then

$$
\overline{\partial_tu_i}=\lim_{T\to\infty}\frac{u_i(T)-u_i(0)}T=0
$$

provided the endpoint difference grows sublinearly. Averaging the [continuity equation](../../../../../continuity-equation.md) gives

$$
\boxed{U_{i,i}=0,\qquad u_{i,i}'=0.}
$$

In [Einstein notation](../../../../../einstein-notation.md), the nonlinear term expands as

$$
\begin{aligned}
\overline{u_ju_{i,j}}
&=\overline{(U_j+u_j')(U_{i,j}+u_{i,j}')}\\
&=U_jU_{i,j}+U_j\overline{u_{i,j}'}
+\overline{u_j'}U_{i,j}+\overline{u_j'u_{i,j}'}\\
&=U_jU_{i,j}+\overline{u_j'u_{i,j}'}.
\end{aligned}
$$

Thus the [Reynolds-averaged Navier-Stokes equation](../../../../../reynolds-averaged-momentum-equation.md) is

$$
\boxed{\rho U_jU_{i,j}=-P_{,i}+\mu U_{i,jj}
-\rho\overline{u_j'u_{i,j}'}.}
$$

The extra term survives because the average of a product of zero-mean fluctuations need not vanish; it represents turbulent transport of mean [linear momentum](../../../../../momentum-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../../split.md)
6. [Topics in fluid mechanics course of the University of Oxford](../../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
