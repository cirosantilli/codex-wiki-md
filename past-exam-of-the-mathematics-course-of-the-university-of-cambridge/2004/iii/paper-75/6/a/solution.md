<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Batchelor entrainment hypothesis](../../../../../../batchelor-entrainment-hypothesis.md) assumes that the mean ambient inflow normal to the edge of a turbulent [turbulent plume](../../../../../../turbulent-plume-split.md) is proportional to its representative axial [velocity](../../../../../../velocity.md), $v_e=\alpha w$. With [top-hat plume model](../../../../../../top-hat-plume-model.md) fields and circumference $2\pi b$, the added volume per height is $2\pi b\alpha w=2\pi\alpha\sqrt M$. It is an integral turbulent mixing closure; it does not assert that every instantaneous eddy has the same inward speed. Use constant positive $\alpha$, uniform resting ambient, [Boussinesq approximation](../../../../../../boussinesq-approximation.md), negligible drag and no buoyancy loss.

Since $B'=0$, $B=B_0$. Eliminate $z$ between the volume and momentum balances:

$$
\frac{dM}{dQ}=\frac{B_0Q}{2\alpha M^{3/2}},\qquad \frac{d(M^{5/2})}{dQ}=\frac{5B_0Q}{4\alpha}.
$$

The zero-source-flux condition gives $M^{5/2}=5B_0Q^2/(8\alpha)$, the [pure plume balance](../../../../../../pure-plume-balance.md). Substitution in $Q'=2\alpha\sqrt M$ and integration gives

$$
\boxed{M=\left(\frac{9\alpha B_0}{10}\right)^{2/3}z^{4/3},\qquad Q=\frac{6\alpha}{5}\left(\frac{9\alpha B_0}{10}\right)^{1/3}z^{5/3},\qquad B=B_0}.
$$

Recovering the top-hat fields from $b=Q/\sqrt M$, $w=M/Q$ and $g'=B/Q$ yields

$$
\boxed{b=\frac{6\alpha}{5}z,\quad w=\frac{5}{6\alpha}\left(\frac{9\alpha B_0}{10}\right)^{1/3}z^{-1/3},\quad g'=\frac{5B_0}{6\alpha}\left(\frac{9\alpha B_0}{10}\right)^{-1/3}z^{-5/3}}.
$$

The paper's ratio is therefore

$$
\boxed{\Gamma=\frac{M^{5/2}}{B_0Q^2}=\frac{5}{8\alpha}}.
$$

This is the constant inverse-normalized ratio used here, not the catalog's normalized [plume balance parameter](../../../../../../plume-balance-parameter.md), which is one for a [pure plume](../../../../../../pure-plume.md). The zero-flux point source is a limiting similarity origin: the speed and density anomaly diverge there, so a physically finite source must regularize the near field. The expressions are valid in the region where the [Boussinesq approximation](../../../../../../boussinesq-approximation.md) and turbulent closure apply.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
