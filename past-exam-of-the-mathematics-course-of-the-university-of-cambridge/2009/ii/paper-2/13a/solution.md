<h1 id="13a/solution">Solution</h1>

↑ **Parent:** [13A](../13a.md)

For a positive-speed [travelling wave](../../../../../travelling-wave.md), the nutrient equation gives $a'=kb/c$. Integrating the bacterial equation once, with zero flux in the uncolonized limit, gives

$$
Db'-\chi b\frac{a'}a=-cb.
$$

Hence

$$
\boxed{b'=\frac{b}{cD}\left(\frac{k\chi b}{a}-c^2\right),\qquad a'=\frac{kb}{c}.}
$$

In the region where $b>0$, divide the two equations. With $\gamma=\chi/D$,

$$
\frac{db}{da}-\frac\gamma a b=-\frac{c^2}{kD}.
$$

The condition $b(1)=0$ fixes the integration constant, giving

$$
\boxed{b(a)=\frac{c^2}{k(\chi-D)}(a-a^{\chi/D})\quad(\chi\ne D).}
$$

At $\chi=D$ the limiting expression is $b=-(c^2/kD)a\log a$. These formulas are positive between zero and one. For $\chi<D$ the nutrient reaches zero at a finite rear coordinate, so the strictly positive smooth whole-line ansatz with logarithmic chemotactic sensitivity needs a separate zero-nutrient interpretation there; for $\chi\geq D$ it reaches zero only as $z\to-\infty$.

For $\chi=2D$, the nutrient equation reduces to $a'=(c/D)a(1-a)$ and integration gives

$$
\boxed{a(z)=\frac1{1+Ke^{-cz/D}},\qquad b(z)=\frac{c^2K}{kD}\frac{e^{-cz/D}}{(1+Ke^{-cz/D})^2}.}
$$

The factor $K$ in the bacterial numerator is required by $a'=kb/c$; it is absent in the printed expression unless $K=1$. A translation of $z$ sets $K=1$, which is the version plotted below. The nutrient rises monotonically from zero behind the band to one ahead, while bacteria form a localized pulse with maximum $c^2/(4kD)$ at the nutrient half-height. Its total population is $\int b\,dz=c/k$. The band advances into fresh nutrient, consumes it and leaves a depleted region behind; [chemotaxis](../../../../../chemotaxis.md) draws bacteria up the nutrient gradient while diffusion spreads them.

<a id="13a/image-travelling-bacterial-pulse-and-nutrient-front-for-logarithmic-chemotaxis-with-chi-equal-to-twice-d-plotted-in-dimensionless-travelling-coordinates"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2-chemotactic-band.png)

**[Figure 2](#13a/image-travelling-bacterial-pulse-and-nutrient-front-for-logarithmic-chemotaxis-with-chi-equal-to-twice-d-plotted-in-dimensionless-travelling-coordinates). Travelling bacterial pulse and nutrient front for logarithmic chemotaxis with chi equal to twice D, plotted in dimensionless travelling coordinates**.

## ↑ Ancestors (10)

1. [13A](../13a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
