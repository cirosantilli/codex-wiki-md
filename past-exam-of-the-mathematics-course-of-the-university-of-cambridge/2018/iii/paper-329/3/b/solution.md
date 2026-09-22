<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an axisymmetric [viscous gravity current on a cone](../../../../../../viscous-gravity-current-on-a-cone.md), the cylindrical radius at slant distance $x$ is $x\cos\alpha$. A surface annulus therefore has area $2\pi x\cos\alpha\,dx$. The local downslope [volume flux](../../../../../../volumetric-flow-rate.md) is the same as in part (a), but [conservation of mass](../../../../../../mass-conservation.md) must account for this growing circumference. Thus

$$
\boxed{h_t+\frac Kx\partial_x\left[xh^3(\sin\alpha-\cos\alpha\,h_x)\right]=0,
\qquad V=2\pi\cos\alpha\int_0^{x_N(t)}xh\,dx.}
$$

This is a leading thin-film description away from the apex, with $0<\alpha<\pi/2$ and thickness small relative to the local curvature and streamwise length scales.

The original PDF uses the long-time criterion $x_N\gg(V\csc\alpha)^{1/3}$; the local TeX incorrectly reads $V\cos\alpha$. To see why the PDF criterion is the relevant one, scale $h\sim V/(x_N^2\cos\alpha)$. In the bulk, the hydrostatic-gradient term relative to direct downslope gravity is

$$
\cot\alpha\,|h_x|\sim\frac{V}{x_N^3\sin\alpha}\ll1.
$$

Hence the leading outer evolution, with $\beta=K\sin\alpha$, is

$$
h_t+\frac\beta x\partial_x(xh^3)=0.
$$

For a fixed-volume [similarity solution](../../../../../../similarity-solution.md), let $x_N\propto t^b$ and $h\propto t^a$. [Conservation of mass](../../../../../../mass-conservation.md) gives $a+2b=0$, while the evolution equation gives $a-1=3a-b$. Thus $b=1/5$, $a=-2/5$. Writing $h=t^{-2/5}H(\xi)$, $\xi=x/t^{1/5}$, yields

$$
-\frac25H-\frac15\xi H'+\frac\beta\xi(\xi H^3)'=0.
$$

The positive branch $H=c\sqrt\xi$ satisfies this equation when $c^2=1/(5\beta)$. It gives

$$
\boxed{h(x,t)=\sqrt{\frac{x}{5\beta t}},\qquad 0<x<x_N(t),\qquad
\beta=\frac{\rho g\sin\alpha}{3\mu}.}
$$

The ideal outer current has zero thickness beyond its front. Its mass integral is

$$
V=\frac{2\pi\cos\alpha}{\sqrt{5\beta t}}\int_0^{x_N}x^{3/2}\,dx
=\frac{4\pi\cos\alpha}{5\sqrt{5\beta t}}x_N^{5/2}.
$$

Therefore

$$
\boxed{x_N(t)=\left(\frac{125\beta V^2t}{16\pi^2\cos^2\alpha}\right)^{1/5}
=\left(\frac{125\rho g\sin\alpha\,V^2t}{48\pi^2\mu\cos^2\alpha}\right)^{1/5}.}
$$

The reduced equation is a [conservation law](../../../../../../conservation-law.md) after multiplication by $x$. Its front obeys the [Rankine-Hugoniot condition](../../../../../../rankine-hugoniot-conditions.md), $\dot x_N=\beta h_N^2=x_N/(5t)$, consistent with the mass-derived front position. The outer profile has a finite jump at the front; the omitted hydrostatic-gradient term resolves a narrow front region. There is also a small apex region where the outer gradient and conical curvature violate the local approximations. Neither region sets the leading conserved-volume scaling above.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
