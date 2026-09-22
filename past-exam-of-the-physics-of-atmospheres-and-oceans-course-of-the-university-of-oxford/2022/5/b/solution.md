<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [linear three-reservoir carbon model](../../../../linear-three-reservoir-carbon-model.md), with concentrations as a column [vector](../../../../vector.md), the linear [ordinary differential equation](../../../../ordinary-differential-equation.md) is

$$
\boxed{\dot{\mathbf x}=J\mathbf x+\mathbf f,\qquad
J=\begin{pmatrix}
-r/R_a&r/R_a&0\\
r/R_b&-(r+s)/R_b&s/R_b\\
0&s/R_d&-s/R_d
\end{pmatrix},\qquad
\mathbf f=\begin{pmatrix}E/R_a\\0\\0\end{pmatrix}.}
$$

A homogeneous [normal mode](../../../../normal-mode.md) has $\mathbf x=\mathbf v e^{\lambda t}$, where $J\mathbf v=\lambda\mathbf v$. For negative real [eigenvalues](../../../../eigenvalue.md) the e-folding relaxation time is $\tau=-1/\lambda$. The row sums vanish, so $\mathbf v_3=(1,1,1)^T$ has $\lambda_3=0$ and

$$
\boxed{\tau_3=\infty.}
$$

Equal effective concentrations generate no exchange. Summing the reservoir budgets gives

$$
\frac{d}{dt}(R_aC_a+R_bC_b+R_dC_d)=E.
$$

Thus injected [carbon dioxide](../../../../carbon-dioxide.md) is conserved after emissions cease: the model redistributes it but contains no permanent removal. The zero [normal mode](../../../../normal-mode.md) records this conserved excess [mass](../../../../mass.md), rather than a long but finite decay.

To check the other [normal modes](../../../../normal-mode.md) are damped, set $D=\operatorname{diag}(R_a,R_b,R_d)$ and $L=-DJ$. Then

$$
\mathbf z^TL\mathbf z=r(z_a-z_b)^2+s(z_b-z_d)^2\geq0.
$$

The [similarity transformation](../../../../similarity-transformation.md) $D^{1/2}JD^{-1/2}=-D^{-1/2}LD^{-1/2}$ is a symmetric negative-semidefinite [matrix](../../../../matrix.md) with a one-dimensional [kernel](../../../../kernel-of-a-linear-map-split.md), so the remaining two [eigenvalues](../../../../eigenvalue.md) are strictly negative.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
