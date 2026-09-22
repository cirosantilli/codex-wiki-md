<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The maximum boundary slope is $s_{\max}=h_0k_T$, so [subcritical internal-wave reflection](../../../../../../../subcritical-internal-wave-reflection.md) requires

$$
h_0k_T<\frac{|\omega|}{\sqrt{N^2-\omega^2}},
$$

or equivalently

$$
\boxed{
\frac{Nh_0k_T}{\sqrt{1+h_0^2k_T^2}}<|\omega|<N
}.
$$

Take $k,m>0$ without loss of generality, put

$$
\mu=\frac mk=\sqrt{\frac{N^2}{\omega^2}-1},
\qquad
p_j=k+jk_T,
$$

and write the incident field as the imaginary part of $\widetilde w_i e^{i(kx+mz-\omega t)}$. The [kinematic boundary condition](../../../../../../../kinematic-boundary-condition.md) on $z=h(x)$ is

$$
[w-u h_x]_{z=h(x)}=0.
$$

For a flat boundary the reflected wave is $-\widetilde w_i\sin(kx-mz-\omega t)$. Expanding the boundary condition in a [Taylor expansion](../../../../../../../taylor-expansion.md) about $z=0$ creates the [topographic sidebands of an internal gravity wave](../../../../../../../topographic-sideband-of-an-internal-gravity-wave.md). With upward-radiating vertical wavenumber $-\mu|p_j|$, their complex amplitudes through second order are

$$
B_0=-\widetilde w_i
+\frac{\mu^2h_0^2k}{2}
\left(p_1+|p_{-1}|\right)\widetilde w_i,
$$



$$
B_1=-\mu h_0p_1\widetilde w_i,
\qquad
B_{-1}=\mu h_0p_{-1}\widetilde w_i,
$$



$$
B_2=-\frac12\mu^2h_0^2p_1p_2\widetilde w_i,
\qquad
B_{-2}=-\frac12\mu^2h_0^2|p_{-1}|p_{-2}\widetilde w_i.
$$

Thus the general compact result is

$$
w_r(x,z,t)
=\operatorname{Im}\left\{
e^{-i\omega t}
\sum_{j=-2}^{2}B_j
e^{ip_jx-i\mu|p_j|z}
\right\}+O(h_0^3).
$$

For the convenient nondegenerate case $k>2k_T$, all displayed sideband wavenumbers are positive. Defining $\Theta_j=p_jx-\mu p_jz-\omega t$, the same answer is the explicitly real formula

$$
\begin{aligned}
\frac{w_r}{\widetilde w_i}
={}&\left(-1+\mu^2h_0^2k^2\right)\sin\Theta_0\\
&+\mu h_0\left(p_{-1}\sin\Theta_{-1}-p_1\sin\Theta_1\right)\\
&-\frac{\mu^2h_0^2}{2}
\left(p_{-1}p_{-2}\sin\Theta_{-2}+p_1p_2\sin\Theta_2\right)
+O(h_0^3).
\end{aligned}
$$

Validity requires a linear incident wave, an inviscid uniformly stratified bulk, an outgoing-radiation condition, strict separation from critical slopes, and small boundary excursions for every retained mode, in particular $h_0k_T\ll1$ and $\mu h_0\max_{|j|\leq2}|p_j|\ll1$. A vanishing $p_j$ is a degenerate zero-horizontal-wavenumber case and must be treated by taking the corresponding zero-amplitude limit rather than dividing by $p_j$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 345](../../../../paper-345-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
