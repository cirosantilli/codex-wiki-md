<h1 id="27l/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\Pi$ be a Poisson point process on $\mathbb R^d$ with intensity measure

$$
\mu(A)=\int_A\lambda(x)\,dx,
$$

where $\lambda$ is nonnegative and locally integrable. Let $f:\mathbb R^d\to\mathbb R^s$ be measurable and suppose its pushforward measure

$$
\nu(B)=\mu(f^{-1}(B))
=\int_{f^{-1}(B)}\lambda(x)\,dx
$$

is locally finite. The [mapping theorem for Poisson point processes](../../../../../../mapping-theorem-point-process.md) says that the image counting measure

$$
f(\Pi)=\sum_{x\in\Pi}\delta_{f(x)}
$$

is a Poisson random measure with intensity $\nu$.

For $f(\Pi)$ to be a spatial Poisson process in the usual simple sense, one also assumes that $\nu$ is diffuse:

$$
\nu(\{y\})=0\qquad(y\in\mathbb R^s).
$$

This prevents collisions with positive probability. If $\nu$ is absolutely continuous, its Radon--Nikodym derivative $\widetilde\lambda$ is the image intensity function, characterized by

$$
\boxed{\int_B\widetilde\lambda(y)\,dy
=\int_{f^{-1}(B)}\lambda(x)\,dx.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27L](../../27l.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
