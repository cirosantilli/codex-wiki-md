<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $D_t=\partial_t+\mathbf u\cdot\nabla$ for the [material derivative](../../../../../../material-derivative.md). For any specific quantity $f$, [conservation of mass](../../../../../../mass-conservation.md) gives

$$
\partial_t(\Sigma f)+\nabla\cdot(\Sigma f\mathbf u)=\Sigma D_tf.
$$

Dotting the momentum equation with $\Sigma\mathbf u$ produces the [kinetic energy](../../../../../../kinetic-energy.md) balance

$$
\partial_t\left(\frac12\Sigma u^2\right)+\nabla\cdot\left(\frac12\Sigma u^2\mathbf u\right)=-\mathbf u\cdot\nabla P-\Sigma\mathbf u\cdot\nabla\Phi_t.
$$

The [Coriolis acceleration](../../../../../../coriolis-acceleration.md) does no work because $\mathbf u\cdot(\mathbf e_z\times\mathbf u)=0$. Since the [shearing-sheet tidal potential](../../../../../../shearing-sheet-tidal-potential.md) is time-independent, its advected potential-energy density obeys

$$
\partial_t(\Sigma\Phi_t)+\nabla\cdot(\Sigma\Phi_t\mathbf u)=\Sigma\mathbf u\cdot\nabla\Phi_t.
$$

For the [isothermal equation of state](../../../../../../globally-isothermal-equation-of-state.md), define the [barotropic energy density](../../../../../../barotropic-energy-density.md) $U=c_s^2\Sigma\ln(\Sigma/\Sigma_{\rm ref})$, with fixed positive reference [surface density](../../../../../../surface-density-of-a-disk.md) $\Sigma_{\rm ref}$. The [continuity equation](../../../../../../continuity-equation.md) implies

$$
\partial_tU+\nabla\cdot(U\mathbf u)=-c_s^2\Sigma\nabla\cdot\mathbf u=-P\nabla\cdot\mathbf u.
$$

Adding these balances combines the two [pressure](../../../../../../pressure.md) terms into $-\nabla\cdot(P\mathbf u)$. This establishes [isothermal shearing-sheet energy conservation](../../../../../../isothermal-shearing-sheet-energy-conservation.md). Thus **the conserved energy density and its flux** are

$$
\boxed{\partial_tE+\nabla\cdot\mathbf F=0,\quad E=\frac12\Sigma u^2+c_s^2\Sigma\ln\frac{\Sigma}{\Sigma_{\rm ref}}+\Sigma\Phi_t,\quad \mathbf F=(E+P)\mathbf u.}
$$

Choosing the density unit so that $\Sigma_{\rm ref}=1$ reproduces the printed logarithm. Changing the reference adds a multiple of the conserved mass to $E$ and its advective [energy flux](../../../../../../energy-flux.md). The [barotropic energy density](../../../../../../barotropic-energy-density.md) is the mathematical energy of this fixed-[isothermal sound speed](../../../../../../isothermal-sound-speed.md) closure; it is not the microscopic thermal energy of a thermally isolated gas. Maintaining an [isothermal process](../../../../../../isothermal-process.md) can require heat exchange.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
