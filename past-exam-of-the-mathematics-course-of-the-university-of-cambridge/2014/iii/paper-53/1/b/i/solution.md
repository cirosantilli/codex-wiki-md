<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a centered [Gaussian random field](../../../../../../../gaussian-random-field.md), [Wick's theorem](../../../../../../../wick-s-theorem.md) says that every odd moment vanishes and every even moment is the sum over all pairings of products of two-point functions. For six fields there are $15$ pairings. In the connected three-point function at nonzero external momenta, each of the three external fields must pair with a distinct field at the cubic interaction. There are $3!=6$ such [Wick contractions](../../../../../../../wick-contraction.md). Choosing the undifferentiated field gives three possibilities; interchanging the two differentiated fields gives a further factor of two. The remaining nine pairings involve an external-external pair and an internal pair and belong to tadpole/disconnected contributions. Define the background so the one-point function vanishes, or equivalently subtract these contributions.

It is useful to keep a coefficient $\mathcal C$ multiplying the cubic Hamiltonian: its literal printed value is $1$, whereas the standard dimensionally normalized curvature interaction has $\mathcal C=M_{\mathrm{Pl}}^2$. This distinction will matter for the final amplitude. With

$$
\zeta(\boldsymbol x,\tau)=\int\frac{d^3p}{(2\pi)^3}\zeta_{\boldsymbol p}(\tau)e^{i\boldsymbol p\cdot\boldsymbol x},
$$

and $dt=a\,d\tau$, $\dot\zeta=\zeta'/a$, the interaction entering the time integral is

$$
H_{\mathrm{int}}\,dt=-\mathcal C\epsilon^2a^2d\tau
\int\prod_{a=1}^3\frac{d^3p_a}{(2\pi)^3}
(2\pi)^3\delta^{(3)}(\boldsymbol p_1+\boldsymbol p_2+\boldsymbol p_3)
\zeta_{\boldsymbol p_1}\zeta'_{\boldsymbol p_2}\zeta'_{\boldsymbol p_3}.
$$

In the [interaction picture](../../../../../../../interaction-picture.md), the unequal-time vacuum contraction required by the [in-in formalism](../../../../../../../keldysh-formalism.md) is

$$
\langle\zeta_{\boldsymbol k}(0)\zeta_{\boldsymbol p}(\tau)\rangle
=(2\pi)^3\delta^{(3)}(\boldsymbol k+\boldsymbol p)u_k(0)u_k^*(\tau).
$$

For a differentiated internal field replace $u_k^*$ by $u_k^{*\prime}$. The equal-time [power spectrum](../../../../../../../power-spectrum.md) fixes its magnitude; the displayed free [De Sitter curvature mode functions](../../../../../../../de-sitter-curvature-mode-function.md) and vacuum choice fix its unequal-time phase.

Performing the three momentum integrations imposes $\boldsymbol p_a=-\boldsymbol k_a$ for each assignment and leaves one overall momentum delta function. Put $U=u_{k_1}(0)u_{k_2}(0)u_{k_3}(0)$, which is real here, and define

$$
I_i^*=\int_{\mathcal C_+}d\tau\,a^2 u_{k_i}^*(\tau)u_{k_j}^{*\prime}(\tau)u_{k_l}^{*\prime}(\tau),\qquad (i,j,l)\text{ cyclic}.
$$

The upper early-time contour $\mathcal C_+$ runs from $-\infty(1-i\delta)$ to $0$, with $\delta>0$. The Hamiltonian's minus sign and the six connected [Wick contractions](../../../../../../../wick-contraction.md) then give

$$
\boxed{\langle\zeta_1\zeta_2\zeta_3\rangle_c
=(2\pi)^3\delta^{(3)}(\boldsymbol k_1+\boldsymbol k_2+\boldsymbol k_3)
\operatorname{Re}\left[4i\mathcal C\epsilon^2U\sum_{i=1}^3 I_i^*\right].}
$$

This is equivalently $\operatorname{Re}[-4i\mathcal C\epsilon^2U\sum I_i]$ with unconjugated [De Sitter curvature mode functions](../../../../../../../de-sitter-curvature-mode-function.md) and the conjugate lower contour $\mathcal C_-$. Before momentum integration, the same result consists of the three cyclic delta assignments, each with the extra factor of two for the identical differentiated legs.

The PDF's intermediate formula writes only three cyclic assignments without that factor of two. Taken literally it undercounts the connected contractions. Its unconjugated modes must also use the conjugate contour, rather than the upper contour of the original in-in expression. Both points are required for a consistent [in-in bispectrum conjugation rule](../../../../../../../in-in-bispectrum-conjugation-rule.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 53](../../../../paper-53-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
