<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In each factor of the [BCS ground state](../../../../../../bcs-ground-state.md), the [BCS anomalous average](../../../../../../bcs-anomalous-average.md) is $\langle b_k\rangle=u_kv_k=\Delta_k/(2E_k)$. Self-consistency therefore gives the zero-temperature [BCS gap equation](../../../../../../bcs-gap-equation.md)

$$
\boxed{\Delta_k=-\sum_{k'}V_{k,k'}\frac{\Delta_{k'}}{2\sqrt{\xi_{k'}^2+|\Delta_{k'}|^2}}}.
$$

Put $\Omega_D=\hbar\omega_D$. The specified constant attractive interaction makes $\Delta_k$ independent of $k$ inside the energy shell and zero outside it:

$$
\boxed{\Delta_k=\Delta\,\mathbf1_{\{|\xi_k|<\Omega_D\}}}.
$$

The printed $\delta_{k,0}$ is incompatible with this interaction: $k$ labels relative pair momentum, not the total momentum of a [Cooper pair](../../../../../../cooper-pair.md). Every pair here has zero total momentum, while many relative momenta contribute.

For the nonzero solution, the [constant-shell BCS gap equation](../../../../../../constant-shell-bcs-gap-equation.md) becomes $1=(V/L^3)\sum_{|\xi_k|<\Omega_D}(2\sqrt{\xi_k^2+\Delta^2})^{-1}$. Let $\nu_s$ denote the approximately constant [single-spin density of states](../../../../../../single-spin-density-of-states.md) per unit volume at the [Fermi level](../../../../../../fermi-level.md). Then

$$
1=\nu_sV\int_0^{\Omega_D}\frac{d\xi}{\sqrt{\xi^2+\Delta^2}}=\nu_sV\operatorname{arsinh}\frac{\Omega_D}{\Delta},\qquad \boxed{\Delta=\frac{\hbar\omega_D}{\sinh(1/(\nu_sV))}}.
$$

In [weak coupling](../../../../../../weak-coupling.md), $\Delta\simeq2\hbar\omega_De^{-1/(\nu_sV)}$. The displayed answer in the question uses $\nu=\nu_s$. If “total electronic density of states” includes both spin species, $\nu_{\mathrm{tot}}=2\nu_s$, the argument instead reads $2/(\nu_{\mathrm{tot}}V)$. If the density counts the whole box rather than unit volume, divide it by $L^3$ before using this formula.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
