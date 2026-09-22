<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the compatible open semicircles and set $r=\sqrt{x^2+y^2}$. The [characteristic curve](../../../../../characteristic-curve.md) through $(\cos\theta,\sin\theta,-1)$ has

$$
z(s)=-(1-s)^{-1/3},\qquad s<1.
$$

The condition $s<1$ is essential: at $s=1$ there is [finite-time blowup](../../../../../finite-time-blowup.md), so the opposite branch cannot be reached from the data. From $r=(1-s\sin\theta)^{-1}$ and $y=r\sin\theta$,

$$
s=\frac{r-1}{y}.
$$

Eliminating $s$ yields

$$
\boxed{z(x,y)=-\left(\frac{y}{1+y-\sqrt{x^2+y^2}}\right)^{1/3}.}
$$

The ratio inside the [cube root](../../../../../cube-root.md) is positive precisely on the two data-determined regions

$$
\boxed{\begin{aligned}
D_+&=\{(x,y):y>0,\ r<1+y\}
=\{(x,y):y>0,\ y>(x^2-1)/2\},\\
D_-&=\{(x,y):y<0,\ r>1+y\}
=\{(x,y):y<0,\ y<(x^2-1)/2\}.
\end{aligned}}
$$

On $D_+$ each point traces to the upper semicircle, and on $D_-$ to the lower semicircle, with $s<1$. To check the parameter ranges explicitly, for $\eta=\sin\theta>0$ they are $-\infty<s<1$, whereas for $\eta<0$ they are $1/\eta<s<1$. At the latter lower endpoint the planar projection escapes to infinity. The [inverse function theorem](../../../../../inverse-function-theorem.md) and uniqueness for the characteristic [ordinary differential equations](../../../../../ordinary-differential-equation.md) give a unique smooth solution on each region. Equivalently, each point has the unique foot $(x/r,y/r)$ and parameter $(r-1)/y$.

A direct check is particularly short. For $s=(r-1)/y$, let $\mathcal D=xy\partial_x+y^2\partial_y$. Then $\mathcal Dr=yr$, $\mathcal Dy=y^2$, and

$$
\mathcal Ds=\frac{(yr)y-(r-1)y^2}{y^2}=1.
$$

Since $dz/ds=-z^4/3$, the displayed formula solves the [partial differential equation](../../../../../partial-differential-equation-split.md), and $r=1$ gives $z=-1$ on both open semicircles. The finite boundary where $r=1+y$, away from the axis, is the [parabola](../../../../../parabola.md) $y=(x^2-1)/2$ and corresponds to blowup. Points on $y=0$ cannot be added to a classical continuation of these regions: where they are approached from a data-determined region, the height behaves like a nonzero multiple of $|y|^{1/3}$, or has incompatible limits at the endpoints. The formula is therefore the complete classical answer for the compatible arcs, while the full-circle problem as printed has no classical solution.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
