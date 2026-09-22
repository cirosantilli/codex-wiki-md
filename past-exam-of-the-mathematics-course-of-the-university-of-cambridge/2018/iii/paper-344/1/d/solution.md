<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md) give [Fourier modes](../../../../../../fourier-mode.md) $q=n\pi/L$, including the spatially uniform mode $q=0$. In the frame translating with the mean deposition height, that mode has no restoring force and obeys

$$
dh_0=\sigma\,dW_t,\qquad
h_0(t)=h_0(0)+\sigma W_t,
\qquad \boxed{\operatorname{Var}h_0(t)=\operatorname{Var}h_0(0)+\sigma^2t}.
$$

Here $W_t$ is [Brownian motion](../../../../../../brownian-motion-split.md), independent of the initial height. More generally $\langle h_0(t)^2\rangle=\langle h_0(0)^2\rangle+\sigma^2t$ when these [second moments](../../../../../../second-moment.md) exist. Removing the mean deposition drift does not remove the [Gaussian white noise](../../../../../../gaussian-white-noise.md).

The [Brownian zero mode of a fluctuating interface](../../../../../../brownian-zero-mode-of-a-fluctuating-interface.md) has no [stationary distribution](../../../../../../stationary-distribution.md) on the real height axis for $\sigma^2>0$. This conclusion does not depend on assuming finite [variance](../../../../../../variance-split.md): a stationary [characteristic function](../../../../../../characteristic-function.md) would satisfy $\widehat\mu(k)=\widehat\mu(k)e^{-\sigma^2k^2t/2}$, hence vanish for every $k\ne0$, contradicting its continuity at zero and $\widehat\mu(0)=1$. Any stationary joint distribution of the whole height would have a stationary zero-mode marginal, which is impossible. Thus **the full unpinned height has no Boltzmann equilibrium**. Pinning the mean height, or retaining only the nonzero [Fourier modes](../../../../../../fourier-mode.md), removes this obstruction. The PDF has $\dot h_q$; the TeX's $\hbar_q$ is a transcription error.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
