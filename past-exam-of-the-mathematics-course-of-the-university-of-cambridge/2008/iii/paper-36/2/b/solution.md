<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

After the fixed time $s$, the [mapping-out function](../../../../../../mapping-out-function-of-a-compact-h-hull.md) of the uncentered mapped future is

$$
\bar g_t=g_{s+t}\circ g_s^{-1}.
$$

Its expansion is $\bar g_t(z)=z+2t/z+O(z^{-2})$, so the elapsed time $t$ is still the [half-plane-capacity parameterization](../../../../../../half-plane-capacity-parameterization.md). Differentiating in $t$ yields

$$
\partial_t\bar g_t(z)=\frac2{\bar g_t(z)-\xi_{s+t}},\qquad\bar g_0(z)=z.
$$

Therefore **the [Loewner transform](../../../../../../loewner-driving-function.md) of $\bar\gamma_t=g_s(\gamma_{s+t})$ is $\xi_{s+t}$**, with starting point $\xi_s$.

Centering gives $\tilde g_t(w)=\bar g_t(w+\xi_s)-\xi_s$, whose driver is $\tilde\xi_t=\xi_{s+t}-\xi_s$. By independent stationary [Brownian increments](../../../../../../brownian-increment.md), $(B_{s+t}-B_s)_{t\geq0}$ is a standard [Brownian motion](../../../../../../brownian-motion-split.md) independent of the past through time $s$. Hence

$$
\boxed{(\tilde\gamma_t)_{t\geq0}\text{ is a fresh chordal SLE}(\kappa)
\text{ from }0\text{ to }\infty,\text{ independent of the past}.}
$$

This proves the [domain Markov property of a chordal Loewner chain](../../../../../../domain-markov-property-of-a-chordal-loewner-chain.md) from the [composition rule for chordal Loewner driving functions](../../../../../../composition-rule-for-chordal-loewner-driving-functions.md). For possible contacts with the old hull, the mapped trace is understood through the continuous boundary extension or [prime ends](../../../../../../prime-end.md); on the open half-plane the displayed maps are ordinary [conformal maps](../../../../../../conformal-map.md). The PDF asks first for the driver of the uncentered curve $\bar\gamma$; the centered driver is included as well.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
