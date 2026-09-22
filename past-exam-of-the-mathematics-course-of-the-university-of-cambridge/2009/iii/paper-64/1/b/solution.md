<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $D_t=\partial_t+\mathbf u\cdot\nabla$. The [continuity equation](../../../../../../continuity-equation.md) and the expanded [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) are

$$
D_t\rho=-\rho\nabla\cdot\mathbf u,\qquad D_t\mathbf B=(\mathbf B\cdot\nabla)\mathbf u-\mathbf B\nabla\cdot\mathbf u,
$$

so $D_t(B_i/\rho)=(B_j/\rho)\partial_ju_i$. Because $\mathbf B=\nabla\times\mathbf A$, the induction equation permits the [magnetic vector potential](../../../../../../magnetic-vector-potential.md) equation $\partial_t\mathbf A=\mathbf u\times\mathbf B-\nabla\varphi$, with an arbitrary scalar electric potential $\varphi$ carrying the gauge choice. Using $(\mathbf u\times\nabla\times\mathbf A)_i=u_j\partial_iA_j-u_j\partial_jA_i$ yields

$$
D_tA_i=\partial_i(\mathbf u\cdot\mathbf A-\varphi)-A_j\partial_i u_j.
$$

Contracting with $B_i/\rho$ and differentiating that factor gives

$$
\begin{aligned}
D_t\left(\frac{A_iB_i}{\rho}\right)
&=\frac{B_i}{\rho}\partial_i(\mathbf u\cdot\mathbf A-\varphi)-\frac{B_iA_j}{\rho}\partial_i u_j+\frac{A_iB_j}{\rho}\partial_j u_i\\
&=\frac{\mathbf B}{\rho}\cdot\nabla(\mathbf u\cdot\mathbf A-\varphi).
\end{aligned}
$$

The last two terms cancel by exchanging their dummy indices. Thus the requested [material derivative](../../../../../../material-derivative.md) is

$$
\boxed{D_t(\mathbf A\cdot\mathbf B/\rho)=\frac{\mathbf B}{\rho}\cdot\nabla(\mathbf u\cdot\mathbf A-\varphi).}
$$

This is [material transport of magnetic helicity density](../../../../../../material-transport-of-magnetic-helicity-density.md).

For a material volume, [mass conservation](../../../../../../mass-conservation.md) gives $d\int_{V(t)}\rho h\,dV/dt=\int_{V(t)}\rho D_th\,dV$. Apply this with $h=\mathbf A\cdot\mathbf B/\rho$, and use $\nabla\cdot\mathbf B=0$ and the [divergence theorem](../../../../../../divergence-theorem.md):

$$
\frac{dH_m}{dt}=\int_{V(t)}\mathbf B\cdot\nabla(\mathbf u\cdot\mathbf A-\varphi)\,dV=\int_{\partial V(t)}(\mathbf u\cdot\mathbf A-\varphi)\mathbf B\cdot\mathbf n\,dS.
$$

If the [magnetic field lines](../../../../../../magnetic-field-line.md) do not penetrate the boundary, $\mathbf B\cdot\mathbf n=0$, so $\boxed{dH_m/dt=0}$.

For uniqueness under a regular, single-valued [gauge transformation](../../../../../../gauge-transformation.md) $\mathbf A\mapsto\mathbf A+\nabla\Lambda$,

$$
\Delta H_m=\int_V\nabla\Lambda\cdot\mathbf B\,dV=\int_{\partial V}\Lambda\mathbf B\cdot\mathbf n\,dS=0.
$$

Consequently this [magnetic helicity](../../../../../../magnetic-helicity.md) is both conserved and gauge independent. As usual, vector potentials are understood to be globally regular potentials for the same field, rather than unrelated harmonic-circulation choices on a multiply connected restricted domain.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
