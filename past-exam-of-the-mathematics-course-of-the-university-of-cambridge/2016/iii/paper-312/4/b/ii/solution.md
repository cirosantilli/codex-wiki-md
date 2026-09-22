<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $A_k=H/\sqrt{4\epsilon M_{\mathrm{Pl}}^2k^3}$, so $u_k(0)=A_k$. For the cyclic term with the first field undifferentiated, insertion into the [in-in formalism](../../../../../../../keldysh-formalism.md) gives

$$
a^2\prod_ru_{k_r}(0)\,u_{k_1}^*u_{k_2}^{*\prime}u_{k_3}^{*\prime}=\frac{H^4}{64\epsilon^3M_{\mathrm{Pl}}^6(k_1k_2k_3)^3}\,k_2^2k_3^2(1-ik_1\tau)e^{iK\tau},
$$

where $K=k_1+k_2+k_3>0$. The two differentiated modes contribute $\tau^2$, cancelling the $\tau^{-2}$ in $a^2$.

Along the vacuum-selected contour, the lower boundary vanishes. The elementary integrals are

$$
\int_{-\infty(1-i\varepsilon)}^0e^{iK\tau}\,d\tau=-\frac{i}{K},\qquad \int_{-\infty(1-i\varepsilon)}^0\tau e^{iK\tau}\,d\tau=\frac{1}{K^2},
$$

and therefore

$$
\int_{-\infty(1-i\varepsilon)}^0(1-ik_1\tau)e^{iK\tau}\,d\tau=-i\left(\frac1K+\frac{k_1}{K^2}\right).
$$

Multiplying by $4iM_{\mathrm{Pl}}^2\epsilon^2$, taking the real part and summing the three cyclic choices gives the [curvature bispectrum from a zeta zeta-prime-squared interaction](../../../../../../../curvature-bispectrum-from-a-zeta-zeta-prime-squared-interaction.md):

$$
\boxed{\begin{aligned}
\langle\zeta_1\zeta_2\zeta_3\rangle_c&=(2\pi)^3\delta^{(3)}(\mathbf k_1+\mathbf k_2+\mathbf k_3)B^{\mathrm{sf}},\\
B^{\mathrm{sf}}&=\frac{H^4}{16\epsilon M_{\mathrm{Pl}}^4(k_1k_2k_3)^3}\sum_{\mathrm{cyc}}k_2^2k_3^2\left(\frac1K+\frac{k_1}{K^2}\right).
\end{aligned}}
$$

This matches the final normalization. The coefficient requires all six connected [Wick contractions](../../../../../../../wick-contraction.md).

The calculation assumes the Gaussian [Bunch-Davies vacuum](../../../../../../../bunch-davies-vacuum.md), tree order in the specified cubic interaction, effectively constant $H$ and $\epsilon$ during the integral, the approximate de Sitter [scale factor](../../../../../../../scale-factor-cosmology.md), and observation after the modes freeze as $\tau\to0^-$. The contour tilt is kept until the early boundary has been eliminated; an undamped real-axis integral cannot simply discard that boundary. The [reduced Planck mass](../../../../../../../reduced-planck-mass.md) convention is the one in the supplied [De Sitter curvature mode function](../../../../../../../de-sitter-curvature-mode-function.md). Other cubic interactions and nonlinear field redefinitions are outside the specified model, so this is not by itself the complete bispectrum of a general single-field action.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 312](../../../../paper-312-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
