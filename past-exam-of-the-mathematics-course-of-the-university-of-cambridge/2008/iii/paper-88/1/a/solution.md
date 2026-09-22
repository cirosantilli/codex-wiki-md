<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $R=|\mathbf x|$, $\mathbf n=\mathbf x/R$ and $t_R=t-R/c_0$. Convolving the source terms in the [Lighthill acoustic analogy](../../../../../../lighthill-acoustic-analogy.md) with the [retarded acoustic Green function](../../../../../../retarded-acoustic-green-function.md), and moving their spatial derivatives outside the integral, gives

$$
\rho'=\partial_{x_i}\partial_{x_j}\int\frac{T_{ij}(\mathbf y,t-|\mathbf x-\mathbf y|/c_0)}{4\pi c_0^2|\mathbf x-\mathbf y|}\,d^3y
-\partial_{x_i}\int\frac{f_i(\mathbf y,t-|\mathbf x-\mathbf y|/c_0)}{4\pi c_0^2|\mathbf x-\mathbf y|}\,d^3y.
$$

The integrals have compact spatial support. For an acoustically compact source, its size $l$ satisfies $\omega l/c_0\ll1$, so the source-dependent retardation is negligible at leading order. Also take $R\gg l$. Define $S_{ij}=\int T_{ij}\,d^3y$ and $F_i=\int f_i\,d^3y$. In the radiation terms the spatial derivatives act on $t_R$, with $\partial_{x_i}t_R=-n_i/c_0$. Derivatives of $1/R$ produce smaller near-field terms. Thus the [far-field acoustic force and stress moments](../../../../../../far-field-acoustic-force-and-stress-moments.md) give

$$
\boxed{\rho'(\mathbf x,t)=\frac{n_in_j\ddot S_{ij}(t_R)}{4\pi c_0^4R}
+\frac{n_i\dot F_i(t_R)}{4\pi c_0^3R}.}
$$

Using $n_i=x_i/R$ gives the equivalent powers of $R$ requested. The force term is an [acoustic dipole](../../../../../../acoustic-dipole.md); the [Lighthill stress tensor](../../../../../../lighthill-stress-tensor.md) produces an [acoustic quadrupole](../../../../../../acoustic-quadrupole.md).

For a small body in low-speed flow, put $M=u/c_0\ll1$. A typical unsteady force has size $F=O(\rho_0u^2l^2)$ and time scale $l/u$, whereas $S=O(\rho_0u^2l^3)$. Therefore

$$
\boxed{\frac{\rho'_D}{\rho_0}=O\!\left(\frac lR M^3\right),
\qquad \frac{\rho'_Q}{\rho_0}=O\!\left(\frac lR M^4\right).}
$$

These are the [acoustic dipole Mach-number scaling](../../../../../../acoustic-dipole-mach-number-scaling.md) and [compact acoustic quadrupole Mach-number scaling](../../../../../../compact-acoustic-quadrupole-mach-number-scaling.md). Since $p'=c_0^2\rho'$ and outgoing acoustic intensity is of order $p'^2/(\rho_0c_0)$, their sound powers scale as

$$
P_D=O(\rho_0u^6l^2/c_0^3),\qquad P_Q=O(\rho_0u^8l^2/c_0^5).
$$

Thus an unsteady force on the body can produce the dominant low-[Mach number](../../../../../../mach-number.md) sound. If the integrated force or its time derivative vanishes, that dipole contribution is absent. Force on the body and force on the fluid have opposite signs.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
