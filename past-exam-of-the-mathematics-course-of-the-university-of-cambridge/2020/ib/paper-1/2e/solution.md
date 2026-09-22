<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

For an oriented smooth embedded surface, the [Gauss map](../../../../../gauss-map.md) sends each point to its chosen unit normal. This surface is the ring torus with major radius two and minor radius one. Its outward Gauss map is

$$
\boxed{f(u,v)=(\cos v\cos u,\cos v\sin u,\sin v)}.
$$

On the $y=0$ cross-section, the normal points radially away from the center of each generating circle, which gives this formula for $u=0,\pi$ and then rotational symmetry gives it for all $u$.

The upper hemisphere condition is $\sin v>0$, hence $0<v<\pi$. For this torus, the [Gaussian curvature](../../../../../gaussian-curvature.md) and area element are

$$
K=\frac{\cos v}{2+\cos v},
\qquad
dA=(2+\cos v)\,du\,dv.
$$

Therefore the positive outer and negative inner contributions cancel:

$$
\boxed{\int_{f^{-1}(U)}K\,dA
=\int_0^{2\pi}\int_0^\pi\cos v\,dv\,du=0}.
$$

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
