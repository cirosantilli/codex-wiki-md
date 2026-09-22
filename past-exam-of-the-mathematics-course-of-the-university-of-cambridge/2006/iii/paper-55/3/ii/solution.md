<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use $T=\xi^0$ and $\xi^i=\partial^i\lambda$, and define the physical background [Hubble parameter](../../../../../../hubble-parameter.md) by $H=\dot a/(\bar N a)$. At first order, the spacetime metric components are $\delta g_{00}=-2\bar N^2\Phi$, $\delta g_{0i}=a^2B_{,i}$ and $\delta g_{ij}=-2a^2(\Psi\delta_{ij}+E_{,ij})$. Apply the given passive [cosmological gauge transformation](../../../../../../gauge-transformation-in-cosmological-perturbation-theory.md) component by component. The temporal component changes by $2\bar N\dot{\bar N}T+2\bar N^2\dot T$; the mixed component changes by $\bar N^2T_{,i}-a^2\dot\lambda_{,i}$; and the spatial component changes by $-2a\dot aT\delta_{ij}-2a^2\lambda_{,ij}$. Hence

$$
\boxed{\widetilde\Phi=\Phi-\dot T-\frac{\dot{\bar N}}{\bar N}T,\qquad
\widetilde B=B+\frac{\bar N^2}{a^2}T-\dot\lambda,\qquad
\widetilde\Psi=\Psi+\bar NH T,\qquad
\widetilde E=E+\lambda.}
$$

These are the [scalar gauge transformations with a background lapse](../../../../../../scalar-gauge-transformations-with-a-background-lapse.md) in the paper's sign convention.

Starting in [synchronous gauge](../../../../../../synchronous-gauge-in-cosmology.md), preserving both $\Phi=0$ and $B=0$ requires

$$
\partial_t(\bar N T)=0,\qquad
\dot\lambda=\frac{\bar N^2}{a^2}T.
$$

The first equation integrates to $\bar NT=C(\mathbf x)$; substituting in the second and integrating gives

$$
\boxed{T=\frac{C(\mathbf x)}{\bar N(t)},\qquad
\lambda=C(\mathbf x)\int^t\frac{\bar N(s)}{a(s)^2}\,ds+D(\mathbf x).}
$$

The arbitrary lower integration limit is absorbed into $D$. Thus specifying synchronous lapse and shift does not fix the origins of the freely falling clocks or all spatial coordinate labels. This is the [residual gauge freedom in synchronous gauge](../../../../../../residual-synchronous-gauge-freedom.md).

During [cosmic inflation](../../../../../../cosmic-inflation-split.md), choosing these clocks remains arbitrary. For example, the $C$ mode shifts the spatial potential by $HC$ and the density perturbation by $3HC(\bar\rho+\bar P)$. In the [de Sitter approximation](../../../../../../de-sitter-approximation.md), $H$ varies little, so a nearly constant [metric perturbation](../../../../../../linearized-gravity.md) can contain a pure coordinate contribution. An [inflaton](../../../../../../inflaton.md) fluctuation or [density contrast](../../../../../../density-contrast.md) in [synchronous gauge](../../../../../../synchronous-gauge-in-cosmology.md) therefore cannot be declared physical solely from its time behavior. Use a [uniform-density curvature perturbation](../../../../../../uniform-density-curvature-perturbation.md) or an appropriate field-based gauge-invariant variable, or fix a physical initial slicing. The exact de Sitter case has no evolving homogeneous density clock, which makes density-defined slicing degenerate.

During the standard hot Big Bang, a cold-matter rest frame supplies a convenient additional condition: imposing zero cold-matter velocity removes the nontrivial spatially varying time-shift mode. Before that condition is imposed, the pure-gauge [density contrast](../../../../../../density-contrast.md) for constant $w$ is $3H(1+w)C$, which decays as $t^{-1}$ in either radiation or [matter domination](../../../../../../matter-domination.md). In [conformal time](../../../../../../conformal-time.md) this is proportional to $\tau^{-2}$ during [radiation domination](../../../../../../radiation-domination.md) and $\tau^{-3}$ during [matter domination](../../../../../../matter-domination.md). It can be confused with an independent decaying physical mode unless gauge freedom is fixed. The $D$ mode is a time-independent spatial relabeling and must likewise be fixed by a coordinate or initial-metric convention.

Finally, a scalar density transforms by evaluating the homogeneous scalar at the shifted time:

$$
\delta\widetilde\rho=\delta\rho-\dot{\bar\rho}T.
$$

To reach [Newtonian gauge](../../../../../../newtonian-gauge.md) from synchronous quantities, impose $\widetilde E=\widetilde B=0$. For the nonhomogeneous scalar modes, choose

$$
\lambda=-E_S,\qquad T=-\frac{a^2}{\bar N^2}\dot E_S.
$$

Using background [stress-energy conservation](../../../../../../stress-energy-conservation.md), $\dot{\bar\rho}=-3\bar NH(\bar\rho+\bar P)$, gives the [synchronous-to-Newtonian density transformation with a lapse](../../../../../../synchronous-to-newtonian-density-transformation-with-a-lapse.md):

$$
\boxed{\left(\frac{\delta\rho}{\bar\rho}\right)_N
=\left(\frac{\delta\rho}{\bar\rho}\right)_S
+\frac{a^2\dot E_S}{\bar N^2}\frac{\dot{\bar\rho}}{\bar\rho}
=\left(\frac{\delta\rho}{\bar\rho}\right)_S
-3H\left(1+\frac{\bar P}{\bar\rho}\right)\frac{a^2}{\bar N}\dot E_S.}
$$

The expression includes the lapse factors because dots refer to the arbitrary time coordinate, not automatically to proper time.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
