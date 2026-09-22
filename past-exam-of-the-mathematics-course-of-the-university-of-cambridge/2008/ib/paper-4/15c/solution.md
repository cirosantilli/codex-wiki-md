<h1 id="15c/solution">Solution</h1>

↑ **Parent:** [15C](../15c.md)

Choose the principal [branch of the complex logarithm](../../../../../branch-of-the-complex-logarithm.md) on $H$, with $-\pi<\arg z<\pi$. Then

$$
\log z=\log|z|+i\arg z,\qquad w=-i\log z=\arg z-i\log|z|.
$$

Thus $-\pi<\operatorname{Re}w<\pi$ and the imaginary part ranges over all real numbers. Conversely, for $w=x+iy$ in the strip, $z=e^{iw}=e^{-y}e^{ix}$ is in $H$ and its principal logarithm is $iw$. Therefore $\boxed{w=-i\log z:H\longrightarrow S}$ is an analytic bijection, with analytic inverse $z=e^{iw}$. Every other continuous branch on the connected domain is $\log z+2\pi ik$ for some fixed integer $k$, so its image is the translated strip $\boxed{S+2\pi k}$.

For $G$, introduce the [Möbius transformation](../../../../../mobius-transformation.md) $\zeta=(z-1)/(z+1)$, whose inverse is $z=(1+\zeta)/(1-\zeta)$. Writing $\zeta=a+ib$, its defining circle inequalities transform as follows:

$$
|z|<1\iff |1+\zeta|<|1-\zeta|\iff a<0,
$$

and

$$
|z+i|>\sqrt2\iff |(1+i)+(1-i)\zeta|^2>2|1-\zeta|^2\iff a+b>0.
$$

Hence $G$ maps bijectively onto the wedge $\pi/2<\arg\zeta<3\pi/4$. The principal [branch of the complex logarithm](../../../../../branch-of-the-complex-logarithm.md) is analytic throughout this wedge. Multiplying its logarithm by $-8i$ expands the interval of real parts to $(4\pi,6\pi)$, and subtracting $5\pi$ centers it at zero. The required [conformal map](../../../../../conformal-map.md) is therefore

$$
\boxed{W(z)=-8i\log\left(\frac{z-1}{z+1}\right)-5\pi,\qquad z\in G.}
$$

Its real part is $8\arg\zeta-5\pi\in(-\pi,\pi)$, and its imaginary part $-8\log|\zeta|$ takes every real value. More explicitly, its inverse on $S$ is obtained from $\zeta=\exp(i(W+5\pi)/8)$ and $z=(1+\zeta)/(1-\zeta)$, which verifies both surjectivity and injectivity.

## ↑ Ancestors (10)

1. [15C](../15c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
