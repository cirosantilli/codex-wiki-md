<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With $W=0$ and $V>0$, $Q=Q_0$ and $\phi=e^{-kx}$, where $k=V/Q_0$. No carrier [momentum](../../../../../../momentum.md) is withdrawn; hence the integrated [momentum flux](../../../../../../momentum-flux.md) is exactly constant:

$$
\boxed{\frac{Q_0^2}{h}+\frac12g'_0e^{-kx}h^2=K,\qquad K=\frac{Q_0^2}{h_0}+\frac12g'_0h_0^2.}
$$

On an initially small-[Froude number](../../../../../../froude-number.md) branch, the [pressure](../../../../../../pressure.md) term dominates. At leading order

$$
\boxed{h(x)\sim h_0e^{kx/2},\qquad u(x)\sim u_0e^{-kx/2}.}
$$

A slightly more accurate large-distance amplitude is $\sqrt{2K/g'_0}$, so $h\sim\sqrt{2K/g'_0}\,e^{kx/2}$. The [Froude number](../../../../../../froude-number.md) satisfies $\operatorname{Fr}^2\sim\operatorname{Fr}_0^2e^{-kx/2}$ and remains small. The growing depth can eventually violate confinement or the [shallow water](../../../../../../shallow-water-approximation.md) assumption; this does not make the asymptotic [momentum](../../../../../../momentum.md) calculation inconsistent within its intended regime.

On an initially large-[Froude number](../../../../../../froude-number.md) branch, horizontal [momentum flux](../../../../../../momentum-flux.md) dominates instead. The leading depth is constant, $\boxed{h\sim h_0}$, while the decaying [reduced gravity](../../../../../../reduced-gravity-split.md) makes the [Froude number](../../../../../../froude-number.md) still larger. To resolve the small change, put $\delta=\operatorname{Fr}_0^{-2}\ll1$ and $y=h/h_0$:

$$
\frac1y+\frac\delta2e^{-kx}y^2=1+\frac\delta2,
$$

so

$$
\boxed{\frac h{h_0}=1+\frac\delta2(e^{-kx}-1)+O(\delta^2).}
$$

The depth decreases slightly and tends exactly to $h_\infty=Q_0^2/K=h_0/(1+\delta/2)$. Its [Froude number](../../../../../../froude-number.md) grows like $\operatorname{Fr}_0e^{kx/2}$. Both approximations agree with the exact depth equation $h'=kh/[2(1-\operatorname{Fr}^2)]$: the [subcritical flow](../../../../../../subcritical-flow.md) deepens, while the [supercritical flow](../../../../../../supercritical-flow.md) thins.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Section B](../../section-b.md)
4. [Paper 52](../../../paper-52-split.md)
5. [Iii](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
