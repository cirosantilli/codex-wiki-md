<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Let $t,h$ be the thermal and magnetic scaling fields, with eigenvalues $b^{y_t}$ and $b^{y_h}$. After discarding irrelevant variables whose vanishing is nonsingular, the homogeneous singular [free-energy density](../../../../../../free-energy-density.md) satisfies

$$
f_s(t,h)=b^{-D}f_s(b^{y_t}t,b^{y_h}h).
$$

Choose $b=|t|^{-1/y_t}$. Then

$$
f_s(t,h)=|t|^{D/y_t}\mathcal F_\pm(h|t|^{-y_h/y_t}),\qquad\xi(t,h)=|t|^{-1/y_t}\mathcal X_\pm(h|t|^{-y_h/y_t}).
$$

Two thermal derivatives give the [heat-capacity critical exponent](../../../../../../heat-capacity-critical-exponent.md); one and two field derivatives give the [order-parameter critical exponent](../../../../../../order-parameter-critical-exponent.md) and [magnetic-susceptibility critical exponent](../../../../../../magnetic-susceptibility-critical-exponent.md). The [correlation-length critical exponent](../../../../../../correlation-length-critical-exponent.md) follows directly from the length rescaling. Thus

$$
\boxed{\nu=\frac1{y_t},\qquad\alpha=2-\frac D{y_t},\qquad\beta_m=\frac{D-y_h}{y_t},\qquad\gamma=\frac{2y_h-D}{y_t}.}
$$

At $t=0$, choose $b=|h|^{-1/y_h}$. Differentiating $f_s(0,h)\propto |h|^{D/y_h}$ gives $M\propto\operatorname{sgn}(h)|h|^{(D-y_h)/y_h}$, so $\delta=y_h/(D-y_h)$. The [order parameter](../../../../../../order-parameter.md) has scaling dimension $x_M=D-y_h$; therefore its critical [connected correlation function](../../../../../../connected-correlation-function.md) has power $r^{-2x_M}$. Comparing with $r^{-(D-2+\eta)}$ yields

$$
\boxed{\delta=\frac{y_h}{D-y_h},\qquad\eta=D+2-2y_h.}
$$

These formulas express the requested [critical exponents](../../../../../../critical-exponent.md) in terms of the relevant scaling exponents. Their hyperscaling assumptions must be respected: above an [upper critical dimension](../../../../../../upper-critical-dimension.md), a [dangerously irrelevant coupling](../../../../../../dangerously-irrelevant-coupling.md) can invalidate the free-energy homogeneity used here. Applying the formulas to the [Gaussian thinning transformation](../../../../../../gaussian-momentum-shell-scaling.md) in the root solution gives the requested Gaussian indices and their physical qualifications.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
