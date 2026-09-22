<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiate the [Bernoulli equation](../../../../../../bernoulli-equation.md) at fixed discharge, using $u_x/u=-b_x/b-h_x/h$. This gives

$$
(1-F^2)h_x=F^2h\frac{b_x}{b}-H_x.
$$

At a smooth [hydraulic control](../../../../../../hydraulic-control.md), $F=1$ and the right-hand side must vanish. For the specified geometry,

$$
-2\eta x_c=h_c\frac{2\beta(x_c-a)}{1+\beta(x_c-a)^2},\qquad
\boxed{h_c=\frac{\eta x_c[1+\beta(x_c-a)^2]}{\beta(a-x_c)}.}
$$

For the intended positive parameters $\beta,\eta,a>0$, positive finite depth requires

$$
\boxed{0<x_c<a.}
$$

The control lies between the bed summit and the width minimum, rather than necessarily at either one. For $a<0$ the corresponding interval is $a<x_c<0$. If $a=0$, the coincident summit and throat admit $x_c=0$ without imposing a depth through this first-derivative relation. The limiting cases $\beta=0$ or $\eta=0$ must be handled before division: their control is at the bed summit or throat, respectively.

At $x_c=a/2$, the critical-depth formula simplifies to

$$
\boxed{h_c=\frac{\eta}{\beta}\left(1+\frac{\beta a^2}{4}\right),\qquad
Q=b(x_c)\sqrt{g h_c^3}.}
$$

This establishes the requested depth without assuming that the bed summit and throat coincide.

There is a further regularity qualification if a critical candidate is to be a simple, smooth transcritical [hydraulic control](../../../../../../hydraulic-control.md). At fixed $Q$, define the critical-head envelope

$$
T(x)=H(x)+\frac32\left(\frac{Q^2}{gb(x)^2}\right)^{1/3}.
$$

Real depths require $\mathcal H\ge T(x)$. At a control $\mathcal H=T(x_c)$, so $T$ must have a local maximum, not a local minimum. The first condition $T_x=0$ is precisely the compatibility equation above, and

$$
T_{xx}=H_{xx}-h_c\left[\frac{b_{xx}}b-\frac53\left(\frac{b_x}b\right)^2\right].
$$

For the positive-parameter case, a nondegenerate control therefore additionally satisfies

$$
\boxed{3a+\beta(a-x_c)^2(3a-10x_c)>0.}
$$

Indeed $T_{xx}=-2\eta[3a+\beta(a-x_c)^2(3a-10x_c)]/[3(a-x_c)b(x_c)]$. The interval $0<x_c<a$ gives all positive-depth candidates, while this inequality excludes candidates with no smooth critical crossing. At $a/2$ it becomes $\beta a^2<6$ for a simple control; the requested depth relation remains necessary whenever such a control exists. Equality is a degenerate critical point requiring higher-order analysis. For example, $a=1$, $\beta=16$ makes the midpoint a local minimum of $T$, so positivity of the depth alone would incorrectly identify it as a regular control.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 90](../../../paper-90-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
