<h1 id="9a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $P,Q$ are continuously differentiable on a neighbourhood of a bounded region with a positively oriented piecewise smooth simple boundary. To prove [Green theorem](../../../../../../green-theorem.md), first take a region between the graphs $y=f(x)$ and $y=g(x)$, $a\le x\le b$, with $f\le g$. Counterclockwise orientation traverses the lower graph to the right and the upper graph to the left; vertical end pieces contribute nothing to $P\,dx$. Thus the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) gives

$$
\oint_{\partial R}P\,dx=\int_a^b[P(x,f(x))-P(x,g(x))]dx=-\int_a^b\int_{f(x)}^{g(x)}P_y\,dy\,dx.
$$

Likewise, for a region between graphs $x=u(y)$ and $x=v(y)$, the right boundary is traversed upwards and the left one downwards. Horizontal end pieces contribute nothing to $Q\,dy$, so

$$
\oint_{\partial R}Q\,dy=\int_c^d[Q(v(y),y)-Q(u(y),y)]dy=\int_c^d\int_{u(y)}^{v(y)}Q_x\,dx\,dy.
$$

For a polygonal region, triangulate its interior. Each triangle is of both graph types with piecewise linear bounds, so adding the formulae gives the result: the double integrals add and the integrals on internal edges cancel because the adjacent triangles traverse them in opposite directions. For a regular piecewise smooth simple boundary, choose inscribed simple polygonal approximations to its piecewise smooth parametrization. Their line integrals converge to the original [line integral](../../../../../../line-integral.md), since the parametrizations converge uniformly and their piecewise constant tangent vectors converge in the integral norm on each smooth arc. Their regions converge in area: the symmetric difference lies in a shrinking neighbourhood of the original boundary, which has planar measure zero. Boundedness of the continuous integrand then gives convergence of the area integrals. Passing to the limit proves the formula for the stated boundary class. Combining the two identities gives

$$
\boxed{\oint_{\partial R}(P\,dx+Q\,dy)=\iint_R(Q_x-P_y)\,dx\,dy.}
$$

Positive orientation is essential for the sign.

Choose $P=-y/2$ and $Q=x/2$, for which $Q_x-P_y=1$. The [boundary formula for planar area](../../../../../../boundary-formula-for-planar-area.md) is

$$
\boxed{\operatorname{area}(R)=\frac12\oint_{\partial R}(x\,dy-y\,dx).}
$$

For the [ellipse](../../../../../../ellipse.md), take $a,b>0$ so the given increasing-angle parametrization is counterclockwise. Then $dx=-a\sin\theta\,d\theta$ and $dy=b\cos\theta\,d\theta$, so

$$
\operatorname{area}(R)=\frac12\int_0^{2\pi}ab(\cos^2\theta+\sin^2\theta)d\theta=\boxed{\pi ab}.
$$

If signed nonzero parameters are allowed, the unsigned area is $\pi|ab|$, with orientation corrected accordingly.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [9A](../../9a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
