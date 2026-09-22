<h1 id="37c/solution">Solution</h1>

↑ **Parent:** [37C](../37c.md)

The initial [Fourier transform](../../../../../fourier-transform.md) is $\widehat\zeta(k,0)=2b\zeta_0/(1+b^2k^2)$. Initial rest gives zero [time derivative](../../../../../time-derivative.md), so each wave mode evolves by $\cos(\sqrt{g|k|}t)$. [Fourier inversion](../../../../../fourier-inversion-theorem.md) therefore gives

$$
\boxed{\zeta(x,t)=\frac{2b\zeta_0}{\pi}\int_0^\infty\frac{\cos(kx)\cos(\sqrt{gk}t)}{1+b^2k^2}\,dk.}
$$

On $x=Vt$, the product of cosines produces phases $\varphi_\pm(k)=Vk\pm\sqrt{gk}$ with prefactor $b\zeta_0/\pi$. Only the minus phase has a [stationary point](../../../../../stationary-point.md):

$$
k_*=\frac g{4V^2},\qquad\varphi_-(k_*)=-\frac g{4V},\qquad\varphi_-''(k_*)=\frac{2V^3}{g}>0.
$$

Expanding quadratically there and evaluating the Gaussian [oscillatory integral](../../../../../oscillatory-integral.md) gives the stationary-phase factor $\sqrt{2\pi/(t\varphi_-''(k_*))}$ and phase shift $+\pi/4$. The other phase has no [stationary point](../../../../../stationary-point.md). Using $q=\sqrt k$ makes both endpoint phases smooth with nonzero endpoint derivative and amplitude vanishing at zero, so endpoint contributions are smaller. Thus

$$
\boxed{\zeta(Vt,t)=\frac{b\zeta_0}{1+(bg/(4V^2))^2}\sqrt{\frac g{\pi V^3t}}\cos\left(\frac{gt}{4V}-\frac\pi4\right)+o(t^{-1/2}).}
$$

The selected wavenumber has [group velocity](../../../../../group-velocity.md) $V$, explaining why it determines the long-time signal on this ray.

## ↑ Ancestors (10)

1. [37C](../37c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
