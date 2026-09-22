<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the [parton model](../../../../../../parton-model.md), the incoming parton has $k=\xi P_H$ and the outgoing massless parton has $k'=\xi P_H+q$. Neglecting $P_H^2$ and imposing its on-shell condition gives

$$
0=(\xi P_H+q)^2=2\xi P_H\cdot q+q^2,
\qquad \boxed{\xi=\frac{-q^2}{2P_H\cdot q}=x.}
$$

Thus the [Bjorken scaling variable](../../../../../../bjorken-scaling-variable.md) measures the struck parton's longitudinal momentum fraction in this approximation. The [inelasticity](../../../../../../inelasticity.md) is unchanged when the hadron momentum is replaced by its parton's collinear momentum:

$$
\boxed{y_q=\frac{\xi P_H\cdot q}{\xi P_H\cdot p}=\frac{P_H\cdot q}{P_H\cdot p}=y.}
$$

Let $S_H=(p+P_H)^2\simeq2p\cdot P_H$. The partonic invariant in part (b) is $s(\xi)=\xi S_H$, and $Q^2=-q^2=xyS_H$. Insert its two parton cross sections into the [parton distribution function](../../../../../../parton-distribution-function.md) convolution:

$$
\frac{d\sigma_H}{dy}=\frac{G_F^2S_H}{\pi}\int_0^1\xi\left[q_d(\xi)+(1-y)^2q_{\bar u}(\xi)\right]d\xi.
$$

Since the event's measured $x$ fixes $\xi=x$, the integrand is the cross-section density in $x$. No additional Jacobian from $y_q$ is needed because $y_q=y$. Therefore

$$
\boxed{\frac{d^2\sigma_H}{dy\,dx}=\frac{G_F^2S_H}{\pi}\,x\left[q_d(x)+(1-y)^2q_{\bar u}(x)\right].}
$$

Equivalently $S_H=2E_\nu E_H(1-\cos\vartheta_{\nu H})$ in the chosen massless-hadron frame. The explicit factor $x$ comes from the partonic energy $s=xS_H$, not from redefining the [parton distribution functions](../../../../../../parton-distribution-function.md). This expression uses the stated two-flavor and low-energy approximations, with masses and generation mixing omitted.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
