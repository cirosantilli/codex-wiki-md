<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

**First integral.** If $F$ has no explicit $x$ dependence, the [chain rule](../../../../chain-rule.md) gives

$$
\frac d{dx}\left(F-y'F_{y'}\right)=F_yy'+F_{y'}y''-y''F_{y'}-y'\frac d{dx}F_{y'}=y'\left(F_y-\frac d{dx}F_{y'}\right).
$$

The [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) makes this zero without requiring division by $y'$. Hence the [Beltrami identity](../../../../beltrami-identity.md) is

$$
\boxed{F-y'\frac{\partial F}{\partial y'}=k\quad\text{constant}.}
$$

**Optical paths.** By [Fermat principle](../../../../fermat-principle.md), a ray makes the [optical path length](../../../../optical-path-length.md) stationary. Within the strip $0<y\leq1$, its [functional](../../../../functional.md) for a graph $y(x)$ is

$$
I=\int\mu(y)\,ds=\int\frac{\sqrt{1+(y')^2}}y\,dx.
$$

The [Beltrami identity](../../../../beltrami-identity.md) gives

$$
F-y'F_{y'}=\frac1{y\sqrt{1+(y')^2}}=k.
$$

For a nonvertical segment $k>0$, write $R=1/k$. Then $(y')^2=(R^2-y^2)/y^2$, so

$$
\frac{dx}{dy}=\pm\frac y{\sqrt{R^2-y^2}},\qquad x-c=\mp\sqrt{R^2-y^2}.
$$

Thus the [optical rays in a reciprocal-height refractive index](../../../../optical-rays-in-a-reciprocal-height-refractive-index.md) satisfy

$$
\boxed{(x-c)^2+y^2=R^2,\qquad y>0,}
$$

restricted to the part in the strip. They are arcs of [circles](../../../../circle.md) centered on $y=0$. Vertical lines are the additional solutions, obtained as a limiting case or directly from the constant horizontal optical momentum. The same curves are [geodesics](../../../../geodesic.md) of the [Poincaré half-plane model](../../../../poincare-half-plane-model.md), whose length element is $ds/y$.

**Horizontal displacement.** Let the ray enter at $(x_0,1)$, travelling to the right and downward at angle $0<\theta<\pi/2$ to the vertical. The [refractive index](../../../../refractive-index.md) is continuous at $y=1$, so there is no instantaneous angular jump at entry. The tangent has $(dx/ds,dy/ds)=(\sin\theta,-\cos\theta)$; hence $y'(x_0)=-\cot\theta$. The first integral gives $k=\sin\theta$, or $R=\csc\theta$. The circle derivative $y'=-(x-c)/y$ then fixes $c=x_0-\cot\theta$.

As $y\downarrow0$, the rightward ray approaches $x=c+R$. The total limiting horizontal distance is therefore

$$
\boxed{D=R-\cot\theta=\csc\theta-\cot\theta=\tan\frac\theta2.}
$$

For vertical incidence, $D=0$ by continuity. For a leftward ray the displacement has the opposite sign, with the same magnitude. Since $\tan(\theta/2)$ increases on $[0,\pi/2]$,

$$
\boxed{D\leq1,\qquad D_{\max}=1\text{ in the grazing-incidence limit }\theta\to\pi/2.}
$$

If entry is required to have a strictly downward component, this is a supremum rather than an attained maximum. A horizontal tangent at entry gives the limiting unit-radius arc, which immediately bends downward in the medium.

<a id="10/image-light-rays-entering-a-medium-with-refractive-index-equal-to-reciprocal-height"></a>
![](../../../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1-reciprocal-height-rays.png)

**[Figure 1](#10/image-light-rays-entering-a-medium-with-refractive-index-equal-to-reciprocal-height). Light rays entering a medium with refractive index equal to reciprocal height**. Original circular-ray construction for entry at x equal to zero and y equal to one. Rays bend toward the singular lower boundary; their limiting horizontal displacements are tan of half the entry angle, bounded by one.

The lower boundary is a limit, rather than a point reached in finite optical travel time. On a nonvertical circular ray, $ds/dy=R/\sqrt{R^2-y^2}\to1$ as $y\downarrow0$. Thus the [optical path length](../../../../optical-path-length.md) contains a divergent integral proportional to $\int dy/y$. The horizontal distance stays finite even though propagation toward $y=0$ takes infinite time.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 1](../../paper-1-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
