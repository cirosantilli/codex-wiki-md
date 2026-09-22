<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write the [longitudinal velocity correlation](../../../../../../longitudinal-velocity-correlation.md) as $Q_{LL}=u^2f(r)$, where $u^2$ is one-component [variance](../../../../../../variance-split.md). For [isotropic turbulence](../../../../../../isotropic-turbulence.md), [incompressibility](../../../../../../incompressible-flow.md) gives the transverse correlation $g=f+rf'/2$ and hence

$$
C(r)=u^2(3f+rf'),\qquad
L=4\pi u^2\int_0^\infty r^2(3f+rf')dr
=4\pi u^2[r^3f]_0^\infty.
$$

Exponential decay of the full second-order [velocity correlation tensor](../../../../../../velocity-correlation-tensor.md) makes the last boundary value zero, so $L=0$. For invariance of $I$ we additionally need $r^4K\to0$, as part (ii) shows. This follows if the premise of rapid decay of all two-point correlations includes the two-position triple correlation and persists during evolution; exponential second-order decay at one initial time alone does not establish it. Under this far-field assumption,

$$
\boxed{L=0,\qquad I=\mathrm{constant}.}
$$

Integration by parts also gives $I=8\pi u^2\int_0^\infty r^4f(r)dr$. Assume a nonzero invariant, a self-preserving large-scale correlation shape $f(r,t)=\mathcal F(r/\ell(t))$, high [Reynolds number](../../../../../../reynolds-number.md), freely decaying turbulence and a constant dimensionless dissipation coefficient. Then $I=C_Iu^2\ell^5$ and the energy budget gives $d(u^2)/dt=-C_\epsilon u^3/\ell$, with fixed positive shape constants. Eliminating $\ell$ gives, for $q=u^2$,

$$
\frac{dq}{dt}=-A I^{-1/5}q^{17/10},\qquad
q^{-7/10}(t)=q^{-7/10}(t_0)+\frac{7A}{10}I^{-1/5}(t-t_0).
$$

Thus the [Kolmogorov decay law](../../../../../../kolmogorov-decay-law.md), with a virtual origin $t_*$, is

$$
\boxed{u^2\propto(t-t_*)^{-10/7},\quad
\ell\propto(t-t_*)^{2/7},\quad
\epsilon\propto(t-t_*)^{-17/7}.}
$$

Neither the invariant alone nor [dimensional analysis](../../../../../../dimensional-analysis.md) without the stated large-scale and energy-budget assumptions fixes this decay law.

Now let $\boldsymbol J=\int_V\boldsymbol x\times\boldsymbol u\,dV$. Integrate the supplied identity over both position variables. For a genuinely confined [incompressible flow](../../../../../../incompressible-flow.md) with $\boldsymbol u\cdot\boldsymbol n=0$ on the boundary, each divergence produces a zero surface term, because its flux contains the normal [velocity](../../../../../../velocity.md) at the corresponding point. Averaging the remaining identity gives

$$
\boxed{\langle|\boldsymbol J|^2\rangle
=-\int_V\int_V|\boldsymbol x'-\boldsymbol x|^2
\langle\boldsymbol u(\boldsymbol x)\cdot\boldsymbol u(\boldsymbol x')\rangle dVdV'.}
$$

In a large approximately homogeneous region with short-range correlations, replacing the pair-overlap volume by $V$ suggests $\langle|\boldsymbol J|^2\rangle\simeq VI$. The [Landau angular-momentum argument for turbulent decay](../../../../../../landau-angular-momentum-argument-for-turbulent-decay.md) interprets $I$ as angular-momentum-fluctuation density. For an isolated torque-free turbulent cloud, [conservation of angular momentum](../../../../../../conservation-of-angular-momentum.md) then motivates constant $I$.

The weaknesses concern precisely the passage to an infinite homogeneous field. A fixed large subvolume is not an isolated cloud: it exchanges [momentum](../../../../../../momentum.md) and [angular momentum](../../../../../../angular-momentum.md) by advection and [fluid pressure](../../../../../../fluid-pressure.md) forces. Impermeable walls eliminate the stated velocity-flux terms but need not eliminate viscous or [fluid pressure](../../../../../../fluid-pressure.md) torques. Moreover nonlocal [fluid pressure](../../../../../../fluid-pressure.md) can generate long-range correlations, invalidating the assumed decay, and boundary terms with large lever arms require control before taking a volume limit. Thus the exact integrated identity is sound under its boundary conditions, but the inferred conservation law requires additional hypotheses.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 87](../../../paper-87-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
