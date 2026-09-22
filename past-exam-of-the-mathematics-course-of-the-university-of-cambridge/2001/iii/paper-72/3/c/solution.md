<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [renormalization group](../../../../../../renormalization-group.md) organizes how a statistical system changes when observed at progressively larger length scales. Start with its [partition function](../../../../../../canonical-partition-function.md) and a microscopic cutoff $\Lambda$. Split the [Fourier transform](../../../../../../fourier-transform.md) field into modes below $\Lambda/b$ and modes in the shell $\Lambda/b<|q|<\Lambda$. Integrate the shell modes, rescale coordinates $x'=x/b$ to restore the cutoff, and rescale the field to keep a chosen gradient normalization. This is a [renormalization-group transformation](../../../../../../renormalization-group-transformation.md). It preserves the [partition function](../../../../../../canonical-partition-function.md) when the generated interactions and additive [free energy](../../../../../../thermodynamic-free-energy.md) terms are retained; truncating the resulting operator expansion is an approximation.

A [renormalization-group fixed point](../../../../../../renormalization-group-fixed-point.md) has an invariant dimensionless interaction structure. The continuous flow of a nearby scaling field $v_i$ takes the linearized form

$$
\frac{dv_i}{d\ell}=y_iv_i+O(v^2),\qquad \ell=\log b.
$$

A positive $y_i$ defines a [relevant operator](../../../../../../relevant-operator.md), a negative $y_i$ an [irrelevant operator](../../../../../../irrelevant-operator.md), and a zero $y_i$ a [marginal operator](../../../../../../marginal-operator.md) requiring nonlinear analysis. The continuous-flow eigenvalues $y_i$ should not be confused with the discrete multipliers $b^{y_i}$. To reach a critical point, tune the relevant thermal variable and set the relevant symmetry-breaking source to zero. The resulting flow stays on the [critical surface](../../../../../../critical-surface.md).

Microscopically different systems whose remaining couplings approach the same fixed point share a [universality class](../../../../../../universality-class.md). Irrelevant perturbations lose their influence on long-distance exponents. Relevant directions explain why varying the temperature or field moves the system away from criticality. The thermal scaling field obeys $t'=b^{y_t}t$, while the rescaled [correlation length](../../../../../../correlation-length.md) is $\xi'=\xi/b$. Taking $b=|t|^{-1/y_t}$ therefore gives $\nu=1/y_t$.

If the field has scaling dimension $x_\phi=(d-2+\eta)/2$, the source term $\int h\phi$ has eigenvalue $y_h=d-x_\phi=(d+2-\eta)/2$. The singular [free-energy density](../../../../../../free-energy-density.md) then obeys

$$
f_s(t,h)=b^{-d}f_s(b^{y_t}t,b^{y_h}h),\qquad
2-\alpha=d/y_t,\qquad\Delta=y_h/y_t,
$$

when the [hyperscaling relation](../../../../../../hyperscaling-relation.md) is valid. This derives the [scaling hypothesis for critical phenomena](../../../../../../scaling-hypothesis-for-critical-phenomena.md) and the exponent relations of Question 2 from the fixed-point picture.

At the [Gaussian fixed point](../../../../../../gaussian-fixed-point.md), keeping $\int(\nabla\phi)^2$ invariant gives $x_\phi=(d-2)/2$. The quadratic coupling has $y_r=2$ and the quartic coupling has $y_u=4-d$. Thus quartic interactions are relevant below four dimensions, marginal at four, and irrelevant above four. Below four, in dimensions where an ordinary continuous short-range scalar transition exists, an interacting [Wilson-Fisher fixed point](../../../../../../wilson-fisher-fixed-point.md) governs that transition. Above four, the Gaussian fixed point gives mean-field powers, but the quartic term remains necessary to stabilize the ordered state: it is a [dangerously irrelevant coupling](../../../../../../dangerously-irrelevant-coupling.md), explaining the failure of naive [hyperscaling](../../../../../../hyperscaling-relation.md). **The renormalization group connects scale invariance, universality, relevant tuning parameters and fluctuation corrections in one framework.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
