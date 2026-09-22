<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [P(X, phi) scalar field theory](../../../../../../p-x-phi-scalar-field-theory.md), the background pressure is $p=P$ and the [energy density](../../../../../../energy-density.md) is $\rho=2XP_X-P$. Differentiating at fixed $\phi$ gives $p_X=P_X$ and $\rho_X=P_X+2XP_{XX}$, so the [Sound speed of a P(X, phi) scalar perturbation](../../../../../../sound-speed-of-a-p-x-phi-scalar-perturbation.md) is

$$
\boxed{c_s^2=\frac{p_X}{\rho_X}=\frac{P_X}{P_X+2XP_{XX}}}.
$$

This is the propagation speed of the scalar fluctuation; the derivative is taken at fixed field, rather than along an arbitrary background trajectory.

On the fixed expanding metric,

$$
X=\frac12\dot{\bar\phi}^{\,2}+\dot{\bar\phi}\,\delta\dot\phi+
\frac12(\delta\dot\phi)^2-\frac1{2a^2}(\partial_i\delta\phi)^2.
$$

Write the [comoving curvature perturbation](../../../../../../comoving-curvature-perturbation.md) in the paper's convention as $\zeta=-H\delta\phi/\dot{\bar\phi}$. Neglecting [slow-roll](../../../../../../slow-roll-approximation.md) derivatives of $H$ and $\dot{\bar\phi}$ yields

$$
\boxed{\delta X=\frac{\bar X}{H^2}
\left[-2H\dot\zeta+\dot\zeta^2-a^{-2}(\partial_i\zeta)^2\right]}.
$$

With $\delta X_1=-2\bar X\dot\zeta/H$ and $\delta X_2=\bar X[\dot\zeta^2-a^{-2}(\partial_i\zeta)^2]/H^2$, the only cubic terms are

$$
P_{XX}\delta X_1\delta X_2+\frac16P_{XXX}\delta X_1^3
=\frac{2\bar X^2P_{XX}}{H^3}\dot\zeta\,a^{-2}(\partial_i\zeta)^2
-\left(\frac{2\bar X^2P_{XX}}{H^3}+
\frac{4\bar X^3P_{XXX}}{3H^3}\right)\dot\zeta^3.
$$

The identities $\epsilon=\bar XP_X/H^2$ and $(1-c_s^2)/c_s^2=2\bar XP_{XX}/P_X$ give the [cubic curvature action for a P(X, phi) scalar field](../../../../../../cubic-curvature-action-for-a-p-x-phi-scalar-field.md)

$$
\boxed{
S_3=\int dt\,d^3x\,\frac{a^3\epsilon(1-c_s^2)}{Hc_s^2}
\left[a^{-2}\dot\zeta(\partial_i\zeta)^2+\mathcal A\dot\zeta^3\right],
\qquad
\mathcal A=-1-\frac{2\bar XP_{XXX}}{3P_{XX}}}.
$$

If $P_{XX}=0$, the unfactored expression above supplies the regular limiting result.

For the requested [primordial bispectrum](../../../../../../primordial-bispectrum.md), define $C=\epsilon(1-c_s^2)/(Hc_s^2)$ and $\int_{\mathbf p}=\int d^3p/(2\pi)^3$. The cubic Hamiltonian and $dt=a\,d\tau$ combine to give

$$
aH_{\rm int}
=C a\int_{\mathbf p_1,\mathbf p_2,\mathbf p_3}
(2\pi)^3\delta^{(3)}(\mathbf p_1+\mathbf p_2+\mathbf p_3)
(\mathbf p_2\cdot\mathbf p_3)\,
\zeta'_{\mathbf p_1}\zeta_{\mathbf p_2}\zeta_{\mathbf p_3}.
$$

Here the positive sign comes from the two spatial derivatives and $H_{\rm int}=-L_{\rm int}$ at cubic order. [Wick theorem](../../../../../../wick-s-theorem.md) gives two contractions for each choice of which external leg meets $\zeta'$. At the external time zero,

$$
\langle\zeta_{\mathbf k}(0)\zeta_{\mathbf p}(\tau)\rangle
=(2\pi)^3\delta^{(3)}(\mathbf k+\mathbf p)\,
u_k(0)u_k^*(\tau).
$$

Thus, after removing the momentum-conserving delta function, the Hamiltonian contraction is

$$
2Ca\prod_{j=1}^3u_{k_j}(0)
\sum_{\rm cyc}(\mathbf k_2\cdot\mathbf k_3)
u_{k_1}^{*\,\prime}(\tau)u_{k_2}^*(\tau)u_{k_3}^*(\tau).
$$

Put $A_k=H/\sqrt{4\epsilon c_sk^3}$. Then $u_k(0)=A_k$ and $u_k^{*\,\prime}=A_kc_s^2k^2\tau e^{ikc_s\tau}$. The $\tau$ cancels the $1/\tau$ in $a=-1/(H\tau)$; moreover,

$$
\mathbf k_2\cdot\mathbf k_3=\frac{k_1^2-k_2^2-k_3^2}{2}.
$$

Inserting these expressions into the [in-in formalism](../../../../../../keldysh-formalism.md) and conjugating the expression inside the real part gives

$$
\boxed{
\begin{aligned}
\langle\zeta_{\mathbf k_1}(0)\zeta_{\mathbf k_2}(0)\zeta_{\mathbf k_3}(0)\rangle
={}&(2\pi)^3\delta^{(3)}(\mathbf k_1+\mathbf k_2+\mathbf k_3)
\frac{(1-c_s^2)H^4}{32\epsilon^2c_s^3(k_1k_2k_3)^3}\\
&\times\operatorname{Re}\left[
-i\int_{-\infty(1+i0^+)}^0d\tau\,e^{-iKc_s\tau}
\sum_{\rm cyc} k_1^2(k_1^2-k_2^2-k_3^2)
(1+ik_2c_s\tau)(1+ik_3c_s\tau)\right],
\end{aligned}}
$$

where $K=k_1+k_2+k_3$. Conjugating the integrand also conjugates the contour: the original positive-frequency-product integral has lower limit $-\infty(1-i0^+)$, whereas the negative exponential displayed here requires $-\infty(1+i0^+)$. This supplies the convergent interpretation of the paper's integral.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
