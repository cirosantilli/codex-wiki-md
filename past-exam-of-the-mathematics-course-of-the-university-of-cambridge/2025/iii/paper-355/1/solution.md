<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write the reaction terms as

$$
f(u,v)=u(1+u-\gamma v),\qquad
g(u,v)=v(\beta u-v).
$$

A nonzero homogeneous equilibrium satisfies $v_*=\beta u_*$ and $1+u_*-\gamma v_*=0$, hence

$$
\boxed{u_*=\frac1{\beta\gamma-1},\qquad
v_*=\frac{\beta}{\beta\gamma-1}}.
$$

For physically positive populations it exists exactly when

$$
\boxed{\beta\gamma>1}.
$$

The reaction [Jacobian matrix](../../../../../jacobian-matrix.md) at this equilibrium is

$$
J=u_*
\begin{pmatrix}
1&-\gamma\\
\beta^2&-\beta
\end{pmatrix}.
$$

Its trace and determinant are

$$
\operatorname{tr}J=u_*(1-\beta),\qquad
\det J=u_*^2\beta(\beta\gamma-1)>0.
$$

The equilibrium is therefore stable to spatially uniform perturbations when

$$
\boxed{\beta>1,\qquad\beta\gamma>1}.
$$

For a spatial [Fourier mode](../../../../../fourier-mode.md) of wavenumber $k$, put $q=k^2$. The linearized [reaction–diffusion system](../../../../../reaction-diffusion-system.md) has matrix

$$
J_q=J-q\begin{pmatrix}1&0\\0&d\end{pmatrix}.
$$

Its trace is smaller than $\operatorname{tr}J$, while

$$
\det J_q
=dq^2-u_*(d-\beta)q
+u_*^2\beta(\beta\gamma-1).
$$

The [two-species diffusion-driven instability criterion](../../../../../two-species-diffusion-driven-instability-criterion.md) says that this upward-opening quadratic becomes negative for some $q>0$ precisely when

$$
d>\beta,\qquad
(d-\beta)^2>4d\beta(\beta\gamma-1).
$$

Combining all conditions, a [Turing instability](../../../../../turing-instability.md) may occur in the region

$$
\boxed{
\beta>1,\qquad d>\beta,\qquad
\frac1\beta<\gamma<
\frac1\beta+\frac{(d-\beta)^2}{4d\beta^2}}.
$$

At onset the discriminant vanishes, and the double root is

$$
q_c=\frac{u_*(d-\beta)}{2d}.
$$

The threshold relation gives

$$
\beta\gamma-1=\frac{(d-\beta)^2}{4d\beta},
\qquad
u_*=\frac{4d\beta}{(d-\beta)^2},
$$

so the critical wavenumber is

$$
\boxed{k_c=\left(\frac{2\beta}{d-\beta}\right)^{1/2}}.
$$

If $d=1$, uniform stability requires $\beta>1$ whereas diffusion-driven instability requires $d>\beta$. These inequalities are incompatible, so the Turing region vanishes.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 355](../../paper-355-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
