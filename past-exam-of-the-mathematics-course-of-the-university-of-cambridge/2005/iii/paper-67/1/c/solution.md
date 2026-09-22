<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
D=\{k:\operatorname{Re}\omega(k)<0\}=\{k:\operatorname{Im}k^3<0\},\qquad D_\pm=D\cap\{\pm\operatorname{Im}k>0\}.
$$

The upper domain is the sector $\pi/3<\arg k<2\pi/3$; the lower domain consists of the sectors $\pi<\arg k<4\pi/3$ and $5\pi/3<\arg k<2\pi$. Orient their boundaries with the corresponding domain to the left. For $0<x<L$ and $0<t<T$, the [Fokas method](../../../../../../fokas-method.md) gives the **integral representation**

$$
\boxed{\begin{aligned}
q(x,t)={}&\frac1{2\pi}\int_{\mathbb R}e^{ikx-\omega(k)t}Q_0(k)dk\\
&-\frac1{2\pi}\int_{\partial D_+}e^{ikx-\omega(k)t}\mathcal F(k,T)dk\\
&-\frac1{2\pi}\int_{\partial D_-}e^{ik(x-L)-\omega(k)t}\mathcal G(k,T)dk.
\end{aligned}}
$$

Here $\mathcal F,\mathcal G$ are the combinations of all six [finite-time spectral boundary transforms](../../../../../../finite-time-spectral-boundary-transform.md) defined above. Initially, [Fourier inversion](../../../../../../fourier-inversion-theorem.md) of the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) gives the first integral together with $-\int_{\mathbb R}e^{ikx-\omega t}\mathcal F/(2\pi)$ and $+\int_{\mathbb R}e^{ik(x-L)-\omega t}\mathcal G/(2\pi)$. For the left endpoint, deform through the upper complementary sectors, where the spatial exponential decays and

$$
e^{-\omega t}F_j(k,t)=\int_0^te^{-\omega(t-s)}f_j(s)ds
$$

is bounded. This replaces the real line by $\partial D_+$. For the right endpoint, deform in the lower half-plane; the real portions of $\partial D_-$ run from right to left. Thus its integral is the negative of the real-line integral, explaining the minus sign in the last displayed term. The arc contributions vanish by spatial exponential decay and [integration by parts](../../../../../../integration-by-parts.md) in the transforms. Oscillatory real-line integrals can equivalently be defined by a decaying cutoff and its limit.

Finally use the [finite-horizon extension of a boundary transform](../../../../../../finite-horizon-extension-of-a-boundary-transform.md). The difference between upper limits $t$ and $T$ contains $\int_t^Te^{\omega(s-t)}f_j(s)ds$, bounded in $D$, while the appropriate spatial factor decays inside $D_+$ or $D_-$. The [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md) makes this difference vanish. Keeping $T>t$ also avoids an artificial endpoint half-value in temporal inversion. The [integral representation](../../../../../../integral-representation.md) at this stage deliberately includes the unknown traces; the rotated [global relations](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) eliminate them in the next step.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
