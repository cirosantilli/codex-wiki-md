<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For fixed $\gamma>1$, the linear term $1-\gamma+\gamma x$ vanishes at $x_*=1-1/\gamma$. Put $L_*=\log(1+1/\gamma)>0$ and resolve its neighborhood using $x=x_*+(\varepsilon L_*/\gamma)s$. The [integral](../../../../../../../integral.md) is dominated by the resulting narrow peak:

$$
I\sim\frac1{\gamma\varepsilon L_*}\int_{-\infty}^{\infty}\frac{ds}{1+s^2}
=\boxed{\frac\pi{\gamma\varepsilon\log(1+1/\gamma)}.}
$$

The local [Taylor expansion](../../../../../../../taylor-expansion.md) of the [logarithm](../../../../../../../logarithm.md) changes it by a vanishing relative amount on this width, while both endpoints are many peak widths away for fixed $\gamma>1$.

There is no additional breakdown when $\gamma\gg1$: the peak approaches $x=1$, but its distance from that endpoint is $d=1/\gamma$, whereas its width is $w=\varepsilon L_*/\gamma\sim\varepsilon/\gamma^2$. Thus $w/d=\varepsilon L_*\sim\varepsilon/\gamma\ll1$. The relative [logarithm](../../../../../../../logarithm.md) variation over a width is $O(\varepsilon/\gamma)$, also improving as $\gamma$ grows. For $\gamma\geq1+c$ with fixed $c>0$ these separation conditions hold uniformly, including arbitrarily large $\gamma$. In particular

$$
\boxed{I\sim\frac\pi\varepsilon\qquad(\gamma\gg1).}
$$

The only endpoint transition requiring a new [distinguished limit](../../../../../../../distinguished-limit.md) is the earlier one near $\gamma=1$, where the peak approaches $x=0$. Moving toward an endpoint is not by itself a reason for nonuniformity; the peak width must be compared with its endpoint distance.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 336](../../../../paper-336-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
