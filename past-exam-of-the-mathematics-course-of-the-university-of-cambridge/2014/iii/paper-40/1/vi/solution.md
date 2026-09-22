<h1 id="1/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

There are two closely related objects to distinguish. Inverting the quadratic [Proca action](../../../../../../proca-action.md) gives the usual covariant [Proca propagator](../../../../../../proca-propagator.md). After [integration by parts](../../../../../../integration-by-parts.md), its kernel is

$$
K^{ab}=\eta^{ab}(\Box-m^2)-\partial^a\partial^b,
\qquad K^{ab}(q)=-(q^2+m^2)\eta^{ab}+q^aq^b.
$$

The [matrix inverse](../../../../../../matrix-inverse.md) with the [Feynman i-epsilon prescription](../../../../../../feynman-i-epsilon-prescription.md) gives

$$
\widetilde\Delta^{\rm cov}_{ab}(q)
=\frac{-i}{q^2+m^2-i0}\left(\eta_{ab}+\frac{q_aq_b}{m^2}\right).
$$

Multiplication by $K^{ab}$ gives $i\delta^a_b$ in the distributional limit. The numerator agrees with the [polarization sum for a massive vector boson](../../../../../../polarization-sum-for-a-massive-vector-boson.md) at the poles, but is not a transverse [linear projection](../../../../../../projection-linear-algebra.md) at arbitrary [four-momentum](../../../../../../four-momentum.md).

For the literal canonical [time-ordered product](../../../../../../time-ordered-product.md) of $A_a$ and $A_b$, the nondynamical component $A_0$ produces the [Proca time-ordering contact term](../../../../../../proca-time-ordering-contact-term.md). In the chosen time coordinate the full answer is

$$
\boxed{\Delta_{ab}(x,y)=\int\frac{d^4q}{(2\pi)^4}\,e^{iq\cdot(x-y)}
\left[\frac{-i(\eta_{ab}+q_aq_b/m^2)}{q^2+m^2-i0}
-\frac{i}{m^2}\delta_a^0\delta_b^0\right]}.
$$

To see the local term directly, the three physical [polarization vectors](../../../../../../polarization-vector.md) give $\sum_\lambda\epsilon_{\lambda0}^2=|\boldsymbol q|^2/m^2$. The canonical $00$ [two-point correlation function](../../../../../../two-point-correlation-function.md) therefore has [Fourier transform](../../../../../../fourier-transform.md)

$$
\widetilde\Delta_{00}(q)=\frac{-i|\boldsymbol q|^2}{m^2(q^2+m^2-i0)}.
$$

By contrast, $\eta_{00}+q_0^2/m^2=|\boldsymbol q|^2/m^2-(q^2+m^2)/m^2$, so the covariant expression contains an additional $i/m^2$. The mixed and spatial components have no additional contact term. Thus

$$
\Delta^{\rm cov}_{ab}(x,y)=\Delta_{ab}(x,y)
+\frac{i}{m^2}\delta_a^0\delta_b^0\delta^{(4)}(x-y).
$$

If $T$ is used to mean covariant time ordering, commonly denoted $T^*$, the conventional answer is instead just $\Delta^{\rm cov}$. Both conventions have the same propagating poles and agree away from coincidence; explicitly separating them respects the printed definition as an ordinary [time-ordered product](../../../../../../time-ordered-product.md).

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [1](../../1.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
