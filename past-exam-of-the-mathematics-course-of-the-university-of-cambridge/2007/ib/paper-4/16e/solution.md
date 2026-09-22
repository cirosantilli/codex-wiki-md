<h1 id="16e/solution">Solution</h1>

↑ **Parent:** [16E](../16e.md)

For fixed endpoints, the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is $F_y-\frac d{dx}F_{y'}=0$. Since $F$ has no explicit dependence on $x$, differentiating gives

$$
\frac d{dx}(F-y'F_{y'})=F_yy'+F_{y'}y''-y''F_{y'}-y'\frac d{dx}F_{y'}=y'\left(F_y-\frac d{dx}F_{y'}\right)=0.
$$

Thus **$F-y'F_{y'}=C$**, the [Beltrami identity](../../../../../beltrami-identity.md).

With $r'=dr/d\theta$, the [arc length](../../../../../arc-length.md) element and the prescribed speed give the travel-time [functional](../../../../../functional.md)

$$
\boxed{T[r]=\frac1k\int_0^{\pi/2}\frac{\sqrt{r'^2+r^2}}{r^2}\,d\theta.}
$$

For the circular road $r=a$, this is **$T_{\mathrm{circle}}=\pi/(2ka)$**.

For the integrand $F=\sqrt{r'^2+r^2}/r^2$, the [Beltrami identity](../../../../../beltrami-identity.md) simplifies to

$$
F-r'F_{r'}=\frac1{\sqrt{r'^2+r^2}}=C.
$$

The candidate $r=a(\cos\theta+\sin\theta)$ has $r'^2+r^2=2a^2$ and the required endpoints. To prove it really minimizes the travel time, rather than merely satisfies a [first integral](../../../../../first-integral.md), put $u=1/r$. Then

$$
\frac{\sqrt{r'^2+r^2}}{r^2}=\sqrt{u'^2+u^2}.
$$

This is the Euclidean [arc length](../../../../../arc-length.md) integrand for the inverted curve $(X,Y)=(u\cos\theta,u\sin\theta)$, whose endpoints are $(1/a,0)$ and $(0,1/a)$. Every connecting curve has length at least their [Euclidean distance](../../../../../euclidean-distance.md) $\sqrt2/a$, by the [triangle inequality](../../../../../triangle-inequality.md). Equality is attained by the straight [line segment](../../../../../line-segment.md) $X+Y=1/a$. In polar form it gives $u(\cos\theta+\sin\theta)=1/a$, hence the proposed $r$. It stays strictly positive throughout the interval. Consequently

$$
\boxed{r(\theta)=a(\cos\theta+\sin\theta),\qquad T_{\min}=\frac{\sqrt2}{ka}.}
$$

This [travel-time minimization with speed proportional to squared radius](../../../../../travel-time-minimization-with-speed-proportional-to-squared-radius.md) is globally solved by the inversion: its minimum is strictly less than $\pi/(2ka)$.

## ↑ Ancestors (10)

1. [16E](../16e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
