<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Length functional.** On the unit [sphere](../../../../../sphere.md), write the [position vector](../../../../../position-vector.md) in [spherical coordinates](../../../../../spherical-coordinate-system.md) as

$$
r(\theta,\phi)=(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta).
$$

Its two coordinate [tangent vectors](../../../../../tangent-vector-split.md) satisfy $r_\theta\cdot r_\phi=0$, $|r_\theta|=1$ and $|r_\phi|=\sin\theta$. Consequently the induced [Riemannian metric](../../../../../riemannian-metric-split.md) is $ds^2=d\theta^2+\sin^2\theta\,d\phi^2$. On a segment for which $\theta$ increases and $\phi=\phi(\theta)$,

$$
\boxed{S=\int_{\theta_1}^{\theta_2}\sqrt{1+\sin^2\theta\,(\phi')^2}\,d\theta.}
$$

Segments where $\theta$ is not monotone require another parameter or a subdivision. Endpoint turning points can be handled by a limit.

**First integral.** With $F=\sqrt{1+\sin^2\theta\,(\phi')^2}$, there is no explicit $\phi$ dependence. The [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) therefore says that

$$
\frac{\partial F}{\partial\phi'}=\frac{\sin^2\theta\,\phi'}{\sqrt{1+\sin^2\theta\,(\phi')^2}}=c
$$

is constant. For $c\ne0$, put $k=1/|c|$ and solve:

$$
\boxed{\phi'=\frac{\operatorname{sgn}c}{\sin\theta\sqrt{k^2\sin^2\theta-1}},\qquad\phi(\theta)-\phi(\theta_1)=\operatorname{sgn}c\int_{\theta_1}^{\theta}\frac{d\vartheta}{\sin\vartheta\sqrt{k^2\sin^2\vartheta-1}}.}
$$

The radicand must be nonnegative along the chosen segment. The printed expression with both limits fixed at $\theta_1,\theta_2$ describes a longitude difference between endpoints; a formula for $\phi(\theta)$ needs the variable upper limit and the additive constant shown here. The case $c=0$ gives a [meridian](../../../../../meridian-of-a-sphere.md) with constant longitude. The [equator](../../../../../equator.md) is also a stationary route, although it cannot be parameterized using changing $\theta$.

**Integration and geometric meaning.** Put $t=\cot\theta$, so $d\theta=-dt/(1+t^2)$ and

$$
\sin\theta\sqrt{k^2\sin^2\theta-1}=\frac{\sqrt{k^2-1-t^2}}{1+t^2}.
$$

For a nonconstant segment $k>1$, and writing $K=\sqrt{k^2-1}$, the [integral](../../../../../integral-split.md) becomes

$$
\phi-\phi_0=\mp\arcsin\frac{\cot\theta}K.
$$

Rearranging, and absorbing phase and sign into two constants, gives

$$
\boxed{\cot\theta=A\cos\phi+B\sin\phi.}
$$

Multiplying by $\sin\theta$ shows that the corresponding [Cartesian coordinates](../../../../../cartesian-coordinate-system.md) satisfy $z=Ax+By$. Thus every such stationary route lies in a [plane](../../../../../plane.md) through the sphere's center: it is a [great circle](../../../../../great-circle.md), the [geodesic](../../../../../geodesic.md) of the [sphere](../../../../../sphere.md). The meridians and equator are the limiting or separately parameterized cases of the same description.

**Rome to Singapore.** Use exactly the approximate coordinates supplied in the question: $(\theta,\phi)=(\pi/4,\pi/12)$ at departure and $(\pi/2,7\pi/12)$ at arrival. Inserting them into the preceding relation determines

$$
\boxed{\cot\theta=\cos(\phi-\pi/12),\qquad\frac\pi{12}\leq\phi\leq\frac{7\pi}{12}.}
$$

Indeed the right side is one at Rome and zero at Singapore. This corresponds to $K=1$, $k=\sqrt2$. In latitude $\ell=\pi/2-\theta$, the route is $\ell=\arctan[\cos(\phi-\pi/12)]$: it starts at $45^\circ$ north with an initially eastward heading and then curves southward to the equator. The first-integral expression in $\theta$ has an integrable endpoint singularity at departure, where $\theta$ has a turning point; the longitude parameter is regular there.

<a id="10/b/image-shortest-spherical-route-for-the-approximate-rome-and-singapore-coordinates-in-the-question"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1-great-circle-route.png)

**[Figure 2](#10/b/image-shortest-spherical-route-for-the-approximate-rome-and-singapore-coordinates-in-the-question). Shortest spherical route for the approximate Rome and Singapore coordinates in the question**. Latitude versus longitude for the derived great circle, with endpoints at 45 degrees north and 15 degrees east, and zero degrees north and 105 degrees east. The quarter-circle parameter increases uniformly in spherical distance.

For an explicit regular [arc-length parametrization](../../../../../arc-length-parametrization.md), let $a=r(\pi/4,\pi/12)$ and $b=r(\pi/2,7\pi/12)$. Their [dot product](../../../../../dot-product.md) is $\sin(\pi/4)\cos(\pi/2)=0$. Hence

$$
\boxed{r(s)=a\cos s+b\sin s,\quad0\leq s\leq\frac\pi2,\qquad S_{\min}=\frac\pi2.}
$$

Both $|r(s)|$ and $|r'(s)|$ equal one. The shorter [great circle](../../../../../great-circle.md) arc is the global shortest path: for any unit-speed curve from $a$, its central angle $\alpha=\arccos(a\cdot r)$ satisfies $|d\alpha/ds|\leq1$ by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), since the tangential projection of $a$ has length $\sin\alpha$. Integrating gives length at least the endpoint angle $\pi/2$, which this route attains. For a sphere of radius $R$, the corresponding shortest distance is $\pi R/2$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
