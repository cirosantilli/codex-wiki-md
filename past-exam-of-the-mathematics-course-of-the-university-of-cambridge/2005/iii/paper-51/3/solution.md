<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [connected correlation function](../../../../../connected-correlation-function.md)

$$
G(r)=\langle\sigma_0\sigma_r\rangle-\langle\sigma_0\rangle\langle\sigma_r\rangle.
$$

Away from criticality its large-distance decay is exponential, $G(r)\sim r^{-p}e^{-r/\xi}$ with a model-dependent algebraic prefactor; the exponential rate defines the [correlation length](../../../../../correlation-length.md) $\xi$. At criticality $\xi$ diverges and the decay becomes a power law. Subtracting the disconnected product is essential in the ordered phase: the unconnected [correlation function](../../../../../correlation-function.md) tends to the square of the spontaneous [magnetization](../../../../../magnetization.md) rather than to zero.

For total [free energy](../../../../../thermodynamic-free-energy.md) $F=-\beta^{-1}\ln Z$, at fixed temperature and a field-independent additive constant,

$$
M=-\frac1N\frac{\partial F}{\partial h},\qquad\chi=-\frac1N\frac{\partial^2F}{\partial h^2}.
$$

Writing $S=\sum_r\sigma_r$, differentiation of the [Boltzmann weight](../../../../../boltzmann-factor.md) gives $\partial_h\langle S\rangle=\beta(\langle S^2\rangle-\langle S\rangle^2)$. Consequently

$$
\chi=\frac\beta N\sum_{r,s}\left(\langle\sigma_r\sigma_s\rangle-\langle\sigma_r\rangle\langle\sigma_s\rangle\right).
$$

For a translation-invariant state, each separation occurs $N$ times, so **$\chi=\beta\sum_rG(r)$**. Without translation invariance, the double-sum formula remains the correct relation.

**Gaussian calculation and thinning.** Interpret the displayed local expression as a [Hamiltonian](../../../../../hamiltonian.md) density, to be integrated over space. For $\kappa>0$ and $m^2>0$, completing the square in Fourier modes gives the [connected correlation function](../../../../../connected-correlation-function.md)

$$
\widetilde G(k)=\frac1{\beta(\kappa^{-1}k^2+m^2)}=\frac\kappa{\beta(k^2+\kappa m^2)}.
$$

The uniform field changes the mean to $-h/m^2$ because of the source's $+h\phi$ convention, but does not change this covariance. The nearest pole has inverse length $\sqrt{\kappa m^2}$, equivalently the Green function solves $(-\nabla^2+\kappa m^2)G=\kappa\delta/\beta$. Thus

$$
\boxed{\xi=\frac1{\sqrt{\kappa m^2}}.}
$$

Here $m^2$ is the positive mass coefficient; if $m$ denotes its positive square root, $\xi=1/(\sqrt\kappa\,m)$.

For a [Gaussian thinning transformation](../../../../../gaussian-momentum-shell-scaling.md), split modes into $|k|<\Lambda/b$ and $\Lambda/b<|k|<\Lambda$. The modes are independent, so integrating out the shell produces only an additive [free-energy density](../../../../../free-energy-density.md) and leaves the low-mode quadratic action unchanged. Restore the cutoff by $x=b x'$ and $\phi(x)=b^{-(D-2)/2}\phi'(x')$. Substituting into the kinetic, mass and source terms gives

$$
\kappa'=\kappa,\qquad (m^2)'=b^2m^2,\qquad h'=b^{(D+2)/2}h.
$$

Hence the thermal and field scaling eigenvalues are $y_t=2$ and $y_h=(D+2)/2$. Applying the exponent relations derived in part (f) gives the requested formal [Gaussian critical exponents](../../../../../gaussian-critical-exponent.md)

$$
\boxed{\alpha=2-\frac D2=\frac{4-D}{2},\qquad\beta_m=\frac{D-y_h}{y_t}=\frac{D-2}{4}.}
$$

The heat-capacity result can also be checked directly: the quadratic determinant contributes $f_s\sim(m^2)^{D/2}$, after removing analytic ultraviolet terms, and two derivatives with respect to $m^2\propto t$ give $|t|^{D/2-2}$. At $D=2$, the free-energy power is accompanied by a logarithm, $f_s\sim m^2\ln m^2$, whose second derivative still has index $\alpha=1$. At $D=4$ this becomes a logarithmic [heat capacity](../../../../../heat-capacity.md) singularity, with index $\alpha=0$, rather than a strictly constant singular term.

There is an important [ordered-phase obstruction in a Gaussian scalar model](../../../../../ordered-phase-obstruction-in-a-gaussian-scalar-model.md). A purely quadratic potential is unbounded below for $m^2<0$, so the Hamiltonian as printed has no stable ordered phase and no literal spontaneous-magnetization exponent. The displayed $\beta_m$ is its Gaussian scaling index, obtained by assigning the field its Gaussian scaling dimension; it is not a construction of a stable ordered equilibrium. For $D<4$, a stabilizing quartic interaction is relevant and generally changes the actual critical fixed point. For $D\leq2$, massless Gaussian infrared fluctuations also obstruct interpreting the formal zero or negative index as an ordinary bounded-spin ordering law. These qualifications do not alter the requested thinning calculation, but are necessary for its physical interpretation.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
