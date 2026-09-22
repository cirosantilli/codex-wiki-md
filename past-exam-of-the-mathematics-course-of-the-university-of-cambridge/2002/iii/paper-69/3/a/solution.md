<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [scaling hypothesis for critical phenomena](../../../../../../scaling-hypothesis-for-critical-phenomena.md) describes the singular part of the equilibrium [free-energy density](../../../../../../free-energy-density.md), rather than its analytic background. For an isotropic system in spatial dimension $D$, with thermal scaling field $t$ and [conjugate field](../../../../../../field-conjugate-to-an-order-parameter.md) $h$, write

$$
f_s(t,h)=b^{-D}f_s(b^{y_t}t,b^{y_h}h).
$$

This follows from coarse graining near a [renormalization-group fixed point](../../../../../../renormalization-group-fixed-point.md): a [correlation volume](../../../../../../correlation-volume.md) is enlarged by $b^D$, while the relevant thermal and field perturbations grow with their [eigenvalues](../../../../../../eigenvalue.md). Choosing $b=|t|^{-1/y_t}$ gives

$$
f_s(t,h)=|t|^{2-\alpha}\Phi_\pm(h/|t|^\Delta),\qquad
2-\alpha=D/y_t,\quad \Delta=y_h/y_t.
$$

The two functions describe the two sides of the transition. Nonuniversal metric factors multiplying $t,h,f_s$ must be allowed when comparing microscopic models. Exponents and suitably normalized scaling functions or amplitude ratios characterize a [universality class](../../../../../../universality-class.md).

Differentiating the [free-energy density](../../../../../../free-energy-density.md) gives the [order parameter](../../../../../../order-parameter.md) $M=-\partial_hf_s$, [magnetic susceptibility](../../../../../../magnetic-susceptibility.md) $\chi=\partial_hM$ and singular [heat capacity](../../../../../../heat-capacity.md) proportional to $-\partial_t^2f_s$. Thus

$$
\beta_{\rm mag}=\frac{D-y_h}{y_t},\qquad
\gamma=\frac{2y_h-D}{y_t},\qquad
\alpha=2-\frac D{y_t}.
$$

The subscript distinguishes the order-parameter exponent from inverse temperature. At $t=0$, choose $b=|h|^{-1/y_h}$ to obtain $M\sim\operatorname{sgn}(h)|h|^{1/\delta}$, with $\delta=y_h/(D-y_h)$. These derivatives imply the [Rushbrooke scaling relation](../../../../../../rushbrooke-scaling-relation.md) $\alpha+2\beta_{\rm mag}+\gamma=2$ and the [Widom scaling relation](../../../../../../widom-scaling-relation.md) $\gamma=\beta_{\rm mag}(\delta-1)$. Equivalently, the equation of state has $h=|t|^\Delta\mathcal H_\pm(M/|t|^{\beta_{\rm mag}})$, with $\Delta=\beta_{\rm mag}\delta=\beta_{\rm mag}+\gamma$.

The [correlation length](../../../../../../correlation-length.md) scales as $\xi\sim|t|^{-\nu}$, $\nu=1/y_t$. At criticality the connected [correlation function](../../../../../../correlation-function.md) behaves as $G(r)\sim r^{-(D-2+\eta)}$, giving $y_h=(D+2-\eta)/2$. Integrating $G$ over a [correlation volume](../../../../../../correlation-volume.md) gives $\chi\sim\xi^{2-\eta}$ and hence the [Fisher scaling relation](../../../../../../fisher-scaling-relation.md) $\gamma=(2-\eta)\nu$. The [hyperscaling relation](../../../../../../hyperscaling-relation.md) $2-\alpha=D\nu$ expresses one singular free-energy contribution per [correlation volume](../../../../../../correlation-volume.md).

These laws organize measurements: plotting $M/|t|^{\beta_{\rm mag}}$ against $h/|t|^\Delta$ collapses near-critical curves onto the appropriate scaling function. A finite system replaces the divergent length by its size $L$; the corresponding prediction is $f_s=L^{-D}\mathcal F(tL^{y_t},hL^{y_h})$ under the same scaling assumptions. Finite size rounds a sharp thermodynamic singularity.

The hypothesis has a domain of validity. At a [renormalization-group fixed point](../../../../../../renormalization-group-fixed-point.md) one generally needs $f_s=b^{-D}f_s(b^{y_t}t,b^{y_h}h,b^{y_u}u,\ldots)$, including other scaling fields. Ordinary irrelevant couplings can be set to zero in a nonsingular limiting scaling function. A [dangerously irrelevant coupling](../../../../../../dangerously-irrelevant-coupling.md) cannot: above the [upper critical dimension](../../../../../../upper-critical-dimension.md) of scalar quartic theory, the quartic term is irrelevant at the Gaussian point but still stabilizes the ordered phase. Consequently naive hyperscaling fails there even though other exponent relations can remain valid. Marginal variables can produce logarithms, anisotropic systems require the appropriate volume exponent, and the [Berezinskii–Kosterlitz–Thouless transition](../../../../../../berezinskii-kosterlitz-thouless-transition.md) has an essential correlation-length singularity instead of a finite power-law $\nu$. **Scaling theory relates observables through a small number of fixed-point dimensions; it does not make analytic backgrounds, marginal logarithms or dangerously irrelevant variables disappear.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
