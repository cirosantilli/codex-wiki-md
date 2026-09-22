<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $n=n_0+y\mathcal L n_0+O(y^2)$, with $n_0=(e^x-1)^{-1}$ and $\mathcal L=x^{-2}\partial_x(x^4\partial_x)$. Differentiating the [Planck photon distribution](../../../../../../planck-photon-distribution.md) gives

$$
n_0'=-\frac{e^x}{(e^x-1)^2},\qquad
\mathcal L n_0=\frac{x e^x}{(e^x-1)^2}
\left[x\frac{e^x+1}{e^x-1}-4\right].
$$

Dividing by $n_0$ proves the first-order [thermal Sunyaev-Zeldovich effect](../../../../../../thermal-sunyaev-zeldovich-effect.md):

$$
\boxed{\frac{\Delta n}{n_0}
=y\frac{x e^x}{e^x-1}\left[x\coth(x/2)-4\right].}
$$

In the [Rayleigh-Jeans law](../../../../../../rayleigh-jeans-law.md) limit, $xe^x/(e^x-1)\to1$ and $x\coth(x/2)\to2$, so **$\Delta n/n_0\to-2y$**. In the [Wien approximation](../../../../../../wien-approximation.md), the prefactor approaches $x$ and the bracket approaches $x-4$, so **$\Delta n/n_0\sim yx(x-4)\sim yx^2$**. The last limit is an asymptotic description of the first-order coefficient: a perturbative prediction at large $x$ still requires $yx^2\ll1$.

Hot electrons transfer [energy](../../../../../../energy.md) to the [cosmic microwave background](../../../../../../cosmic-microwave-background.md), removing low-frequency [photons](../../../../../../photon.md) and enhancing the high-frequency tail. The first-order distortion crosses zero where $x\coth(x/2)=4$, at $x\simeq3.830$; for today's [CMB](../../../../../../cosmic-microwave-background.md) this is near $217\,\mathrm{GHz}$. Photon conservation follows directly from the boundary term

$$
\int_0^\infty x^2\Delta n\,dx=y[x^4n_0']_0^\infty=0.
$$

In contrast, [integration by parts](../../../../../../integration-by-parts.md) gives $\int x^3\Delta n\,dx=4y\int x^3n_0\,dx$, so radiation gains a fraction $4y$ of its original [energy](../../../../../../energy.md). The [thermal Sunyaev-Zeldovich effect](../../../../../../thermal-sunyaev-zeldovich-effect.md) is thus a spectral distortion, not simply a new [blackbody](../../../../../../blackbody.md) temperature.

A [galaxy cluster](../../../../../../galaxy-cluster.md) with bulk [peculiar velocity](../../../../../../peculiar-velocity.md) along the [line of sight](../../../../../../line-of-sight.md) additionally produces the [kinetic Sunyaev-Zeldovich effect](../../../../../../kinetic-sunyaev-zeldovich-effect.md). Define $v_\parallel>0$ for recession and $\tau=\int n_e\sigma_Td\ell$. To first order in velocity and [optical depth](../../../../../../optical-depth.md), $\Delta T/T=-\tau v_\parallel/c$: receding gas gives a decrement and approaching gas an increment. Its [occupation number](../../../../../../occupation-number.md) perturbation is $(\Delta T/T)xe^x/(e^x-1)^2$, the spectrum of a small [blackbody](../../../../../../blackbody.md) temperature change. It remains nonzero at the thermal null and therefore complicates measurements near that [frequency](../../../../../../frequency.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
