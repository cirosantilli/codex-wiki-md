<h1 id="24f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\zeta=e^{2\pi i/7}$ and define

$$
\phi(x,y)=(\zeta^3x,\zeta y).
$$

Each term in the defining polynomial is multiplied by $\zeta^3$:

$$
(\zeta^3x)^3(\zeta y)+(\zeta y)^3+\zeta^3x
=\zeta^3(x^3y+y^3+x).
$$

Thus $\phi$ is a holomorphic automorphism of $X'$, with inverse obtained by replacing $\zeta$ by $\zeta^{-1}$. By the assumption it extends to a holomorphic automorphism of $X$; in the projective model it is

$$
[X:Y:Z]\longmapsto[\zeta^3X:\zeta Y:Z].
$$

It has order exactly seven because $\zeta$ is primitive and $y$ is not identically zero. Hence $\operatorname{Aut}(X)$ contains an element of order seven.

The extended coordinate function $\pi_x:X\to\mathbb C_\infty$ is a [meromorphic function as a holomorphic map to the Riemann sphere](../../../../../../meromorphic-function-as-a-holomorphic-map-to-the-riemann-sphere.md). Compose it with the seventh-power map of the sphere and set

$$
\pi=\pi_x^7.
$$

This map is nonconstant and holomorphic as a map to $\mathbb C_\infty$. Since $\pi_x\circ\phi=\zeta^3\pi_x$,

$$
\boxed{\pi\circ\phi
=(\zeta^3\pi_x)^7
=\pi_x^7
=\pi}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [24F](../../24f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
