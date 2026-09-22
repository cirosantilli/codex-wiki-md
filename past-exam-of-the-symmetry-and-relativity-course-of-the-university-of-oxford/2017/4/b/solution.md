<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [electromagnetic four-potential](../../../../electromagnetic-four-potential.md) is $A^\mu=(\Phi/c,\mathbf A)$, and the vacuum [four-wavevector](../../../../four-wavevector.md) is $K^\mu=(\omega/c,0,0,k)$ with $k=\omega/c>0$. Define $\psi=K_\mu X^\mu=\omega t-kz$ and $C=(\omega k)^{-1/2}$. The given transverse potential is $A_y=-C\sin\psi$. Its physical fields are

$$
\boxed{E_y=C\omega\cos\psi,\qquad B_x=-Ck\cos\psi,}
$$

so the [Poynting vector](../../../../poynting-vector.md) points along positive $z$. For our signature, $\partial^\mu=(c^{-1}\partial_t,-\nabla)$, $F^{0i}=-E_i/c$, and $F^{ij}=-\epsilon_{ijk}B_k$. Therefore

$$
\boxed{F^{\mu\nu}=C\cos\psi
\begin{pmatrix}
0&0&-\omega/c&0\\
0&0&0&0\\
\omega/c&0&0&k\\
0&0&-k&0
\end{pmatrix}.}
$$

The square-root prefactor is simply the source's chosen wave normalization; an overall dimensional amplitude could multiply every field.

The [four-current](../../../../four-current.md) is $J^\mu=(c\rho,\mathbf j)$, with $J_\mu=(c\rho,-\mathbf j)$. [Charge conservation](../../../../charge-conservation.md) takes the equivalent forms

$$
\boxed{\partial_t\rho+\nabla\cdot\mathbf j=0,\qquad
\partial_\mu J^\mu=\partial^\mu J_\mu=0.}
$$

Lowering both indices of $F$ changes the sign of its time-space entries: $F_{0i}=E_i/c$, while $F_{ij}=-\epsilon_{ijk}B_k$. The temporal component of $\partial^\mu F_{\mu\nu}$ is $\nabla\cdot\mathbf E/c=\mu_0c\rho$, by [Gauss's law](../../../../gauss-s-law.md). Its spatial components are $c^{-2}\partial_t\mathbf E-\nabla\times\mathbf B=-\mu_0\mathbf j$, by the [Ampère-Maxwell equation](../../../../ampere-s-circuital-law.md). Hence

$$
\boxed{\partial^\mu F_{\mu\nu}=\mu_0J_\nu.}
$$

For the displayed free wave the current vanishes because $k=\omega/c$; the component derivation also proves the sourced identity. The two homogeneous [Maxwell equations](../../../../maxwell-equations-split.md) follow separately from expressing $F$ in terms of a potential.

**Force-sign qualification.** With these definitions the physical [Lorentz force density](../../../../lorentz-force-density.md) is $f_\mu^{\mathrm{phys}}=F_{\mu\nu}J^\nu$, whereas the source prints the reversed contraction $J^\nu F_{\nu\mu}=-f_\mu^{\mathrm{phys}}$. Consequently

$$
\boxed{f_0^{\mathrm{phys}}=\frac{\mathbf j\cdot\mathbf E}{c},\qquad
f_0^{\mathrm{printed}}=-\frac{\mathbf j\cdot\mathbf E}{c}.}
$$

The physical time component is the power transferred to matter per volume divided by $c$, as in [Poynting's theorem](../../../../poynting-theorem.md). For example parallel positive $j_x$ and $E_x$ do positive work, but the literal printed contraction has negative time component. This sign cannot be repaired while simultaneously retaining the source's tensor definition and the Maxwell identity above; reverse the force contraction to describe the physical force.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
