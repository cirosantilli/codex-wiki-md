<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the physical [refractive index](../../../../../../refractive-index.md) convention $k=k_0n$, with $k_0$ the background [wavenumber](../../../../../../wavenumber.md) and time dependence $e^{-i\omega t}$. Treat $B$ as a bounded region in $\mathbb R^3$; the printed $B\in\mathbb R^3$ should be $B\subset\mathbb R^3$. Define the contrast $q=n^2-1=2n_\epsilon+n_\epsilon^2$ and the outgoing [Green function](../../../../../../green-s-function.md)

$$
G_{k_0}(\mathbf r,\mathbf r')=\frac{e^{ik_0|\mathbf r-\mathbf r'|}}{4\pi|\mathbf r-\mathbf r'|},\qquad
(\Delta+k_0^2)G_{k_0}=-\delta.
$$

The [Sommerfeld radiation condition](../../../../../../sommerfeld-radiation-condition.md) selects this sign of the outgoing [wave phase](../../../../../../phase-waves.md). Since $(\Delta+k_0^2)\psi=-k_0^2q\psi$, the [Lippmann-Schwinger equation](../../../../../../lippmann-schwinger-equation.md) is

$$
\psi=\psi_i+T_q\psi,\qquad
(T_q\phi)(\mathbf r)=k_0^2\int_BG_{k_0}(\mathbf r,\mathbf r')q(\mathbf r')\phi(\mathbf r')\,d\mathbf r'.
$$

The positive sign in this integral follows from the minus sign in the defining [Green function](../../../../../../green-s-function.md) equation. One may instead define the [scattering potential](../../../../../../scattering-potential.md) with the opposite sign, provided both equations change consistently.

If $\|T_q\|<1$ on the chosen field space inside $B$, its [Neumann series](../../../../../../neumann-series.md) converges. The [Born series](../../../../../../born-series.md) for the scattered field is

$$
\boxed{\psi_s=\psi-\psi_i=\sum_{m=1}^\infty T_q^m\psi_i.}
$$

For observation points outside $B$, restrict the intermediate factors to $B$ and use the same outgoing integral for the final factor. For example, the first two terms are

$$
\begin{aligned}
\psi_s^{(1)}(\mathbf r)&=k_0^2\int_BG_{k_0}(\mathbf r,\mathbf r_1)q(\mathbf r_1)\psi_i(\mathbf r_1)\,d\mathbf r_1,\\
\psi_s^{(2)}(\mathbf r)&=k_0^4\int_B\int_BG_{k_0}(\mathbf r,\mathbf r_1)q(\mathbf r_1)G_{k_0}(\mathbf r_1,\mathbf r_2)q(\mathbf r_2)\psi_i(\mathbf r_2)\,d\mathbf r_2\,d\mathbf r_1.
\end{aligned}
$$

The $m$th term describes $m$ successive scattering interactions. The first [Born approximation for scalar wave scattering](../../../../../../born-approximation-for-scalar-wave-scattering.md) keeps one interaction and replaces the field inside the medium by the incident field. Higher terms describe [multiple scattering](../../../../../../multiple-scattering.md) and the resulting feedback on the internal field.

A concrete sufficient condition follows on $L^\infty(B)$. If $d_B$ is the diameter of $B$, then for $\mathbf r\in B$ the region lies in the ball of radius $d_B$ about $\mathbf r$, and

$$
\|T_q\|_{\infty\to\infty}\leq k_0^2\|q\|_\infty\sup_{\mathbf r\in B}\int_B\frac{d\mathbf r'}{4\pi|\mathbf r-\mathbf r'|}
\leq\frac12k_0^2d_B^2\|q\|_\infty=:\rho.
$$

Thus $\boxed{\rho\ll1}$ is a conservative sufficient condition for the first [Born approximation for scalar wave scattering](../../../../../../born-approximation-for-scalar-wave-scattering.md). When $\rho<1$, the omitted internal-field terms satisfy

$$
\|\psi_s-T_q\psi_i\|_\infty\leq\frac{\rho^2}{1-\rho}\|\psi_i\|_\infty.
$$

The bound ignores cancellation in the oscillatory [Green function](../../../../../../green-s-function.md), so it is sufficient, not necessary. A common physical small-contrast criterion for an extended weak medium is small accumulated extra [wave phase](../../../../../../phase-waves.md), $k_0\ell\|n_\epsilon\|_\infty\ll1$, together with weak scattering and no resonant internal enhancement. Small local contrast alone is not enough for an arbitrarily large or resonant object.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
