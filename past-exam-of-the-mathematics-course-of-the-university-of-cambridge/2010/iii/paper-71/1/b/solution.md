<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the ambient fluid has zero downslope velocity, no bed drag, and an [entrainment coefficient](../../../../../../entrainment-coefficient.md) $\alpha>0$. The [entraining shallow-water layer](../../../../../../entraining-shallow-water-layer.md) receives volume at rate $\alpha|u|$, but neither excess buoyancy nor downslope momentum from that ambient fluid. Consequently [volume conservation](../../../../../../volume-conservation.md), conservation of excess buoyancy, and [momentum conservation](../../../../../../momentum-conservation.md) give

$$
\boxed{\begin{aligned}
h_t+(hu)_x&=\alpha|u|,\\
(bh)_t+(bhu)_x&=0,\\
(hu)_t+\left(hu^2+\tfrac12bh^2\cos\theta\right)_x&=bh\sin\theta.
\end{aligned}}
$$

The pressure contribution is the integral of the [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) from part (a). The last source is the downslope component of the gravitational force.

With $D=\partial_t+u\partial_x$, the equivalent equations are

$$
Dh+hu_x=\alpha|u|,\qquad
Db=-\frac{\alpha|u|}{h}b,\qquad
Du+b\cos\theta\,h_x+\frac h2\cos\theta\,b_x
=b\sin\theta-\frac{\alpha|u|u}{h}.
$$

The last term is the momentum required to accelerate newly entrained fluid. For variables $(h,u,b)$, the matrix of the spatial derivatives is

$$
A=\begin{pmatrix}
u&h&0\\
b\cos\theta&u&h\cos\theta/2\\
0&0&u
\end{pmatrix},
\qquad
\boxed{\lambda=u,\quad u\pm\sqrt{bh\cos\theta}.}
$$

Thus it is a strictly [hyperbolic system](../../../../../../hyperbolic-system.md) for $h,b>0$ and $0\leq\theta<\pi/2$. At $\theta=\pi/2$ all three [characteristic speeds](../../../../../../characteristic-speed.md) coincide and the matrix is not diagonalizable. The exclusion of that angle presumes the physical range with $\cos\theta\geq0$: allowing an overhanging channel with $\cos\theta<0$ would also destroy [hyperbolicity](../../../../../../hyperbolicity.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
