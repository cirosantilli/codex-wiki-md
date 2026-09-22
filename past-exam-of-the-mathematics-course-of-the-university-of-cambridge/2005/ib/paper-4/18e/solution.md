<h1 id="18e/solution">Solution</h1>

↑ **Parent:** [18E](../18e.md)

Use the standard ideal-fluid assumptions underlying the stated relation: both fluids are incompressible, inviscid and unbounded away from the interface, with no surface tension. An [irrotational flow](../../../../../irrotational-flow.md) has $u_j=\nabla\phi_j$, and [incompressibility](../../../../../incompressible-flow.md) gives $\Delta\phi_j=0$ in each fluid. The unsteady [Bernoulli equation](../../../../../bernoulli-equation.md) is

$$
\phi_{j,t}+\tfrac12|\nabla\phi_j|^2+\frac{p_j}{\rho_j}+gz=C_j(t),
$$

where the arbitrary time functions can be absorbed into the potentials. On $z=\zeta(x,t)$ the material-interface and normal-stress conditions are

$$
\zeta_t+\phi_{j,x}\zeta_x=\phi_{j,z}\quad(j=1,2),\qquad p_1=p_2.
$$

Disturbance velocities decay as $z\to\pm\infty$. The equilibrium pressures are $p_*-\rho_jgz$.

Linearize at the resting flat interface. The equations become $\Delta\phi_j=0$, $\zeta_t=\phi_{j,z}$ on $z=0$, and

$$
\rho_1(\phi_{1,t}+g\zeta)=\rho_2(\phi_{2,t}+g\zeta).
$$

For $k>0$, write $\zeta=\eta e^{i(kx-\omega t)}$. Decay selects $\phi_1=A_1e^{-kz}e^{i(kx-\omega t)}$ above and $\phi_2=A_2e^{kz}e^{i(kx-\omega t)}$ below. The kinematic conditions give $A_1=i\omega\eta/k$ and $A_2=-i\omega\eta/k$. Substituting into the dynamic condition gives

$$
\rho_1(\omega^2/k+g)\eta=\rho_2(-\omega^2/k+g)\eta,
\qquad \boxed{\omega^2=\frac{\rho_2-\rho_1}{\rho_2+\rho_1}gk.}
$$

For a signed wave number replace $k$ by $|k|$. A heavier lower fluid gives stable [interfacial gravity waves](../../../../../interfacial-gravity-wave.md); a heavier upper fluid gives $\omega^2<0$ and [Rayleigh-Taylor instability](../../../../../rayleigh-taylor-instability.md). The density ordering is not silently assumed positive in the derivation.

## ↑ Ancestors (10)

1. [18E](../18e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
