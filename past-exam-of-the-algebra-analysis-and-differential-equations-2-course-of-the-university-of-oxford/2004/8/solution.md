<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

The [method of characteristics](../../../method-of-characteristics.md) uses

$$
\frac{dx}{ds}=a(x,y,u),\qquad\frac{dy}{ds}=b(x,y,u),\qquad\frac{du}{ds}=c(x,y,u).
$$

For a graph parametrized by $(x,y,u(x,y))$, a [normal vector](../../../normal-vector.md) is $N=(-u_x,-u_y,1)$. The PDE says $N\cdot(a,b,c)=0$, so the characteristic vector is tangent to the solution surface. Flowing a suitable initial curve along these directions constructs a surface; where its projection to the $(x,y)$ plane has nonzero [Jacobian determinant](../../../jacobian-determinant.md), the [inverse function theorem](../../../inverse-function-theorem.md) makes it a graph. Local uniqueness of this general flow needs the usual regularity assumptions beyond mere continuity. The particular characteristic system below is smooth and can be solved explicitly.

Label the initial points by $\eta\ge0$. Since $dx/ds=1$, take $x=s$. The other two equations integrate to

$$
u=1+\sin\eta+\frac{x^2}{2},\qquad
y=\eta+x(1+\sin\eta)+\frac{x^3}{6}.
$$

Eliminating $\eta=y-xu+x^3/3$ gives the implicit solution

$$
\boxed{u=1+\frac{x^2}{2}+\sin\!\left(y-xu+\frac{x^3}{3}\right).}
$$

For each fixed $|x|<1$, the [derivative](../../../derivative.md) of the displayed $y$ with respect to $\eta$ is $1+x\cos\eta\ge1-|x|>0$. It increases from its value at $\eta=0$ to infinity, so it is a bijection from $[0,\infty)$ onto $[y_L(x),\infty)$, where

$$
\boxed{y_L(x)=x+\frac{x^3}{6}.}
$$

Thus there is exactly one characteristic label, and hence one solution value, throughout the requested region, including the initial-label boundary as a trace.

The [characteristic fold for sinusoidal data in a forced Burgers equation](../../../characteristic-fold-for-sinusoidal-data-in-a-forced-burgers-equation.md) is seen by differentiating with respect to $y$:

$$
u_y=\frac{\cos\eta}{1+x\cos\eta}.
$$

For a fixed [integer](../../../integer-split.md) $k\ge0$, let $y_*=(2k+1)\pi+7/6$. As $x\to1^-$ at this fixed $y_*$, the label tends to $(2k+1)\pi$, giving $u_y\to-\infty$. To justify the label limit, the limiting map at $x=1$ is strictly increasing despite isolated zero [derivatives](../../../derivative.md), so its inverse has a unique continuous limit. Similarly, at any fixed $y_*=2k\pi-7/6$ with $k\ge1$, the limit as $x\to-1^+$ has $\eta\to2k\pi$ and $u_y\to+\infty$. These fixed values lie within the region near the respective boundary, proving the requested gradient blow-up.

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2004](../../2004-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
