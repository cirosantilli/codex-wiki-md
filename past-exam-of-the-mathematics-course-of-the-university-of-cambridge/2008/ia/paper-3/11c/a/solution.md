<h1 id="11c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [product rule](../../../../../../product-rule.md) gives

$$
\nabla\cdot(f\nabla g)=\nabla f\cdot\nabla g+f\nabla^2g.
$$

Apply the [divergence theorem](../../../../../../divergence-theorem.md), with outward [unit normal](../../../../../../unit-normal.md) $\mathbf n$, and use the vanishing [Laplacian](../../../../../../laplacian.md) of the [harmonic function](../../../../../../harmonic-function.md) $g$:

$$
\int_V\nabla f\cdot\nabla g\,dV=\int_S f\nabla g\cdot\mathbf n\,dS.
$$

The boundary value of $f$ is one. Another application of the [divergence theorem](../../../../../../divergence-theorem.md) therefore gives

$$
\int_S f\nabla g\cdot\mathbf n\,dS=\int_S\nabla g\cdot\mathbf n\,dS=\int_V\nabla^2g\,dV=\boxed{0}.
$$

This is the [gradient pairing with a boundary-constant function and a harmonic function](../../../../../../gradient-pairing-with-a-boundary-constant-function-and-a-harmonic-function.md), obtained directly from [Green's first identity](../../../../../../green-s-first-identity.md). The [harmonic function](../../../../../../harmonic-function.md) must be regular throughout the volume; an interior singularity can supply an additional boundary flux.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11C](../../11c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
