<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Select the [causal Green function](../../../../../../../causal-green-function.md), zero for $t<0$; otherwise the impulse equation permits arbitrary homogeneous additions. Use the spatial [Fourier transform](../../../../../../../fourier-transform.md) convention $e^{-ikx}$ and the temporal [Laplace transform](../../../../../../../laplace-transform.md) boundary convention $e^{i\omega t}$. The transformed impulse equation is

$$
\widehat G(k,\omega)=\frac1{-i\omega+iUk-\mu+\gamma k^2}.
$$

If $\mu>0$, a literal real-frequency [Fourier transform](../../../../../../../fourier-transform.md) of the growing response need not exist. Its causal inverse instead starts on $\operatorname{Im}\omega=c>\max(\mu,0)$ and is continued from there. For $t>0$ close the frequency contour below; its clockwise orientation and the [pole](../../../../../../../pole.md) [residue](../../../../../../../residue.md) $1/(-i)=i$ give $e^{-i\omega(k)t}$. For $t<0$ the upper closure contains no [pole](../../../../../../../pole.md). The remaining inverse spatial transform is a [Gaussian integral](../../../../../../../gaussian-integral.md):

$$
G(x,t)=\frac{H(t)e^{\mu t}}{2\pi}\int_{\mathbb R}
 e^{-\gamma tk^2+ik(x-Ut)}\,dk
=\boxed{\frac{H(t)}{\sqrt{4\pi\gamma t}}
\exp\left[\mu t-\frac{(x-Ut)^2}{4\gamma t}\right]}.
$$

The unit-mass [Gaussian heat kernel](../../../../../../../gaussian-heat-kernel.md) tends to $\delta(x)$ at $t\downarrow0$, giving the required impulse normalization.

At the advected center $x=Ut$, its [amplitude](../../../../../../../wave-amplitude.md) is $e^{\mu t}/\sqrt{4\pi\gamma t}$. At a fixed spatial point,

$$
G(x,t)=\frac{e^{Ux/(2\gamma)}}{\sqrt{4\pi\gamma t}}
\exp\left[\left(\mu-\frac{U^2}{4\gamma}\right)t-\frac{x^2}{4\gamma t}\right].
$$

Thus $\mu>0$ permits growth of the moving [wave packet](../../../../../../../wave-packet.md), but it is [convective hydrodynamic instability](../../../../../../../convective-hydrodynamic-instability.md) if the fixed-position rate is negative. A positive fixed-position rate is [absolute hydrodynamic instability](../../../../../../../absolute-hydrodynamic-instability.md). At its equality threshold the $t^{-1/2}$ factor decays, explaining the marginal exponential classification. This directly verifies the physically selected [Briggs-Bers criterion](../../../../../../../briggs-bers-criterion.md) saddle rather than assuming its accessibility.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 76](../../../../paper-76-split.md)
5. [Iii](../../../../split.md)
6. [2004](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
