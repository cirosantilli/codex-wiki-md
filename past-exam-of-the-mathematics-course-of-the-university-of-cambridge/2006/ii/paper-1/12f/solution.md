<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

In curvature-minus-one polar coordinates the [hyperbolic metric](../../../../../hyperbolic-metric.md) is $ds^2=dr^2+\sinh^2r\,d\theta^2$. Thus the area element is $\sinh r\,dr\,d\theta$, giving

$$
\boxed{\operatorname{Area}B(r)=2\pi(\cosh r-1)=4\pi\sinh^2(r/2).}
$$

It is asymptotic to $\pi e^r$.

For a usual locally finite [tessellation](../../../../../tessellation.md) with [compact](../../../../../compact-space.md) congruent tiles of nonempty interior, let their diameter be at most $D$ and choose in each a congruently placed interior ball of radius $r_0>0$. These balls have disjoint interiors. The number of tiles meeting a [geodesic](../../../../../geodesic.md) segment of length one is uniformly bounded: their ball centres lie in a ball of radius $D+1$, and the disjoint $r_0$-balls lie in the larger ball of radius $D+1+r_0$. Comparing areas supplies a constant $K$. A path of length $R$, divided into at most $\lceil R\rceil$ such segments, therefore crosses at most $K(\lceil R\rceil+1)$ tiles. A small generic perturbation avoids vertices if steps are defined by crossing sides.

Consequently the union of tiles at most $n$ steps from the initial tile contains a metric ball of radius $c n-C$ for fixed $c>0,C$. If $A$ is tile area, their number $N(n)$ is at least $\operatorname{Area}B(cn-C)/A$, an exponential lower bound. Conversely any chain of $n$ adjacent tiles lies in $B(D(n+1))$ about a point in the initial tile; the interiors are disjoint, so $AN(n)\leq\operatorname{Area}B(D(n+1))$. Thus **$N(n)$ is bounded above and below by positive exponential functions of $n$**. No precise common growth exponent is claimed.

An explicit example is the regular right-angled pentagon tiling $\{5,4\}$: reflect a regular hyperbolic pentagon with all angles $\pi/2$ in its sides. Four pentagons meet at each vertex, and their interiors tile the plane. Its tiles have area $3\pi-5\pi/2=\pi$ by the [hyperbolic polygon area](../../../../../hyperbolic-polygon-area.md) formula. The [compactness](../../../../../compact-space.md) and ordinary local finiteness assumptions exclude pathological decompositions with degenerate tiles.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
