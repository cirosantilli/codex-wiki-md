<h1 id="4b/solution">Solution</h1>

↑ **Parent:** [4B](../4b.md)

On the simply connected domain $\mathbb R^3$, a continuously differentiable [differential one-form](../../../../../one-form.md) is [exact](../../../../../exact-differential.md) if its mixed partial derivatives agree, equivalently if its associated vector field has zero [curl](../../../../../curl.md). Here one can verify exactness directly by observing that

$$
F(x,y,z)=(x^2+z^2)e^{(x+y)z}
$$

satisfies

$$
\frac{\partial F}{\partial x}=u,
\qquad
\frac{\partial F}{\partial y}=v,
\qquad
\frac{\partial F}{\partial z}=w.
$$

Thus $u\,dx+v\,dy+w\,dz=dF$. By the [fundamental theorem for line integrals](../../../../../fundamental-theorem-for-line-integrals.md), its integral is [path independent](../../../../../path-independence.md) and equals

$$
F(1,0,1)-F(-1,0,1)=2e-2e^{-1}.
$$

Consequently, for every path with the stated endpoints,

$$
\boxed{\int_{(-1,0,1)}^{(1,0,1)}(u\,dx+v\,dy+w\,dz)=4\sinh1}.
$$

## ↑ Ancestors (10)

1. [4B](../4b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
