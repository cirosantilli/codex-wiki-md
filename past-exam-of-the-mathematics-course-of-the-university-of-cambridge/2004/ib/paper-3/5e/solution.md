<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

The contour has [winding number](../../../../../winding-number.md) one around the single pole at zero. By the [Cauchy integral formula](../../../../../cauchy-integral-formula.md), or the [residue](../../../../../residue.md) of $1/z$,

$$
\boxed{\oint_C\frac{dz}z=2\pi i.}
$$

Rotation by $z\mapsto iz$ carries each oriented edge to the next oriented edge and leaves $dz/z$ unchanged. The four edge integrals are therefore equal, each $\pi i/2$.

On the right edge use $z=1+it$, $-1\le t\le1$, so

$$
\frac{\pi i}{2}=\int_{-1}^1\frac{i\,dt}{1+it}
=\int_{-1}^1\frac{t+i}{1+t^2}\,dt
=i\int_{-1}^1\frac{dt}{1+t^2}.
$$

The real integrand $t/(1+t^2)$ is odd and integrates to zero. Dividing by $i$ gives **$\int_{-1}^1(1+t^2)^{-1}dt=\pi/2$** without needing its real antiderivative.

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
