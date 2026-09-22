<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the paper's mode normalization, effectively $M_p=1$, and set $C=\epsilon+1-c_s^2$, $K=k_1+k_2+k_3$, $s_2=k_1k_2+k_1k_3+k_2k_3$, $s_3=k_1k_2k_3$. Write $\langle\zeta_1\zeta_2\zeta_3\rangle_c=(2\pi)^3\delta^3(\sum\mathbf k_i)B$. There are two source consistency issues: the supplied [interaction picture](../../../../../../interaction-picture.md) expansion makes an external-before-vertex [Wick contraction](../../../../../../wick-contraction.md) contain $u_k(\tau')$, with positive exponential $e^{ikc_s\tau'}$; it converges at $-\infty(1-i0)$, whereas the PDF prints $-\infty(1+i\varepsilon)$. Also the stated positive interaction has the opposite overall bispectrum sign from the printed target. The following calculation identifies both issues directly.

For the stated mode expansion, the ordered contraction is

$$
\langle\zeta_I(\mathbf k,0)\zeta_I(\mathbf p,\tau')\rangle=(2\pi)^3\delta^3(\mathbf k+\mathbf p)\frac{H^2}{4\epsilon c_s k^3}(1-ikc_s\tau')e^{ikc_s\tau'}.
$$

A spatial derivative at the vertex supplies $ip_j$; the two differentiated legs consequently give $-\mathbf k_i\cdot\mathbf k_j$. There are two [Wick contractions](../../../../../../wick-contraction.md) for each choice of the undifferentiated external leg. The extra $a(\tau')$ in the stipulated [in-in formalism](../../../../../../keldysh-formalism.md) integral makes the vertex coefficient $a^2\epsilon C/c_s^2$, using $a^2=1/(H^2\tau'^2)$. This is consistent if the named $H_{\rm int}$ is the cosmic-time generator expressed as a function of $\tau$, since $dt=a\,d\tau$; if it were already the conformal-time generator, that extra $a$ would have to be removed.

For the [spatial-gradient cubic curvature bispectrum](../../../../../../spatial-gradient-cubic-curvature-bispectrum.md), define the [late-time scalar gradient vertex integral](../../../../../../late-time-scalar-gradient-vertex-integral.md)

$$
I=\int_{-\infty(1-i0)}^{\tau_f}\frac{d\tau'}{\tau'^2}(1-ic_sk_1\tau')(1-ic_sk_2\tau')(1-ic_sk_3\tau')e^{ic_sK\tau'},\qquad \tau_f\to0^-.
$$

With $\omega=c_sK$, the first two terms of the product obey $(\tau'^{-2}-i\omega\tau'^{-1})e^{i\omega\tau'}=-\partial_{\tau'}(e^{i\omega\tau'}/\tau')$. The other two use $\int_{-\infty}^0e^{i\omega\tau'}d\tau'=-i/\omega$ and $\int_{-\infty}^0\tau'e^{i\omega\tau'}d\tau'=1/\omega^2$, with the same vacuum prescription. The endpoint divergence $-1/\tau_f$ is real, while

$$
\operatorname{Im}I=c_s\left(-K+\frac{s_2}{K}+\frac{s_3}{K^2}\right)=c_s Q.
$$

In particular the finite $-K$ term comes from the endpoint of the total derivative and must not be discarded along with the real divergence.

Let $S=\mathbf k_1\cdot\mathbf k_2+\mathbf k_1\cdot\mathbf k_3+\mathbf k_2\cdot\mathbf k_3$. The ordered vertex expectation, after stripping the momentum delta, is $Z=-2SH^4C I/(64\epsilon^2c_s^5k_1^3k_2^3k_3^3)$. Since $\operatorname{Re}(-2iZ)=2\operatorname{Im}Z$, the literal positive Hamiltonian gives

$$
\boxed{B_{\rm literal}=-\frac{H^4C}{16\epsilon^2c_s^4k_1^3k_2^3k_3^3}\,S\left(-K+\frac{s_2}{K}+\frac{s_3}{K^2}\right).}
$$

**The printed positive-sign target is obtained by replacing the displayed interaction Hamiltonian by its negative**, with the convergent contour above. This is also the expected sign if a positive cubic $\zeta(\partial\zeta)^2$ coefficient was intended as a Lagrangian term, by the [interaction Hamiltonian](../../../../../../interaction-hamiltonian.md) relation proved in question 3(a). Under that explicit repair,

$$
\boxed{B_{\rm intended}=+\frac{H^4C}{16\epsilon^2c_s^4k_1^3k_2^3k_3^3}\,S\left(-K+\frac{s_2}{K}+\frac{s_3}{K^2}\right).}
$$

Restoring the overall $(2\pi)^3\delta^3(\sum\mathbf k_i)$ reproduces all three cyclic terms in the requested expression. An [equilateral bispectrum configuration](../../../../../../equilateral-bispectrum-configuration.md) is a concrete sign check: for $k_i=k$, $S=-3k^2/2$, $Q=-17k/9$, so $SQ=17k^3/6>0$. The literal interaction gives $B=-17H^4C/(96\epsilon^2c_s^4k^6)$, while the printed target is positive. This cannot be repaired by merely changing the overall definition of $\zeta$, because its field expansion and interaction were specified together. The contour typo and Hamiltonian sign are therefore documented source repairs, rather than silently altered contractions.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
