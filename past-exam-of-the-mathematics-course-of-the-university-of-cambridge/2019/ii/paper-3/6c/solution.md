<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

With the [travelling wave](../../../../../travelling-wave.md) coordinate $\xi=x-ct$, the [reaction–diffusion system](../../../../../reaction-diffusion-system.md) becomes

$$
D f''+cf'+rf(1-f)=0,
\qquad f(-\infty)=1,quad f(+\infty)=0.
$$

At the advancing leading edge the healthy-tissue density is small. Put $f(\xi)\sim e^{-\lambda\xi}$ with $\lambda>0$. The [linearization](../../../../../linearization.md) at $f=0$ gives

$$
D\lambda^2-c\lambda+r=0,
$$

so a nonoscillatory decaying front requires real positive roots,

$$
\lambda=\frac{c\pm\sqrt{c^2-4Dr}}{2D},
\qquad c\geq2\sqrt{Dr}.
$$

The [pulled travelling front](../../../../../pulled-travelling-front.md) selects the [Fisher-KPP minimum wave speed](../../../../../fisher-kpp-minimum-wave-speed.md), and therefore

$$
\boxed{c_{\min}=2\sqrt{Dr}.}
$$

For the initial wound $0<x<W$, two mirror-image fronts enter from its endpoints. The left front moves right from $x=0$ and the right front moves left from $x=W$, each with speed approximately $c_{\min}$. A sequence of sketches would show the initial rectangular depression becoming two smooth monotone transition layers, the zero-density plateau shrinking, and the two layers meeting near $x=W/2$ before the profile relaxes to $S=1$. Their meeting time is

$$
\boxed{t_{\rm heal}\approx\frac{W/2}{c_{\min}}
=\frac{W}{4\sqrt{Dr}}.}
$$

There is an additional local relaxation time of order $1/r$ if “close to one” is assigned a fixed numerical tolerance, so the displayed estimate is the dominant healing time when $W$ is large compared with the front width $\sqrt{D/r}$.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
