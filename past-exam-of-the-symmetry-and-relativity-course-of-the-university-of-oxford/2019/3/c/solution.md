<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $c=1$ and the mostly-plus [Minkowski metric](../../../../minkowski-metric.md) fixed in part [a](../../1/a.md). The [electromagnetic four-potential](../../../../electromagnetic-four-potential.md) and its covariant form are

$$
A^\mu=(\phi,A_x,A_y,A_z),\qquad A_\mu=(-\phi,A_x,A_y,A_z).
$$

Define the [electromagnetic field tensor](../../../../electromagnetic-field-tensor.md) by $F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu$. Since $\mathbf E=-\nabla\phi-\partial_t\mathbf A$ and $\mathbf B=\nabla\times\mathbf A$,

$$
\boxed{F_{\mu\nu}=\begin{pmatrix}
0&-E_x&-E_y&-E_z\\
E_x&0&B_z&-B_y\\
E_y&-B_z&0&B_x\\
E_z&B_y&-B_x&0
\end{pmatrix}.}
$$

Raising both indices changes the signs of its time-space entries. The lower-index signs agree with [Section 2.4.2, equation (2.87), the explicit electromagnetic two-form](../../../../general-relativity-by-david-tong.md); the signature and index placement must be kept consistent.

For a passive boost to a frame moving with $v\widehat{\mathbf x}$, transform the [tensor](../../../../tensor.md) as

$$
F'^{\mu\nu}=\Lambda^\mu{}_{\rho}\Lambda^\nu{}_{\sigma}F^{\rho\sigma},\qquad
\Lambda=\begin{pmatrix}\gamma&-\gamma v&0&0\\-\gamma v&\gamma&0&0\\0&0&1&0\\0&0&0&1\end{pmatrix}.
$$

For example, $F'^{02}=\gamma F^{02}-\gamma vF^{12}=\gamma(E_y-vB_z)$ and $F'^{12}=\gamma(B_z-vE_y)$. Reading off all entries gives

$$
\boxed{\begin{aligned}
E'_x&=E_x,& E'_y&=\gamma(E_y-vB_z),&E'_z&=\gamma(E_z+vB_y),\\
B'_x&=B_x,& B'_y&=\gamma(B_y+vE_z),&B'_z&=\gamma(B_z-vE_y).
\end{aligned}}
$$

For an arbitrary boost [velocity](../../../../velocity.md) $\mathbf v$, rotational covariance gives the [Lorentz transformation of electromagnetic fields](../../../../lorentz-transformation-of-electromagnetic-fields.md)

$$
\boxed{\begin{aligned}
\mathbf E'&=\gamma(\mathbf E+\mathbf v\times\mathbf B)
-\frac{\gamma^2}{\gamma+1}\mathbf v(\mathbf v\cdot\mathbf E),\\
\mathbf B'&=\gamma(\mathbf B-\mathbf v\times\mathbf E)
-\frac{\gamma^2}{\gamma+1}\mathbf v(\mathbf v\cdot\mathbf B).
\end{aligned}}
$$

Here all velocities are in $c=1$ units. Equivalently the parallel components are unchanged and the perpendicular components have the cross-product expressions multiplied by $\gamma$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
