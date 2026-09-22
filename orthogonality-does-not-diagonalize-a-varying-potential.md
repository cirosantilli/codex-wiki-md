# Orthogonality does not diagonalize a varying potential

↑ **Parent:** [Orthogonal vectors](orthogonal-vectors.md)

In the [Hilbert space](hilbert-space-split.md) $L^2([0,2\pi])$, choose [orthonormal](orthonormal-set.md) functions $\phi_1(x)=\cos x/\sqrt\pi$ and $\phi_2(x)=\sin x/\sqrt\pi$. Their [inner product](inner-product-split.md) is zero, but for the real [potential energy](potential-energy.md) $V(x)=V_0\sin2x$,

$$
\langle\phi_1,V\phi_2\rangle
=\frac{V_0}{\pi}\int_0^{2\pi}\cos x\sin x\sin2x\,dx
=\frac{V_0}{2\pi}\int_0^{2\pi}\sin^2(2x)\,dx
=\boxed{\frac{V_0}{2}}.
$$

Thus ordinary [orthogonality](orthogonal-vectors.md) alone does not remove an off-diagonal [matrix element](matrix-element.md) of a spatially varying [potential energy](potential-energy.md). A constant scalar potential does give zero between distinct [orthonormal](orthonormal-set.md) states. The example separates these two claims; it is not a model of localized atomic orbitals in a particular crystal.

## ↑ Ancestors (7)

1. [Orthogonal vectors](orthogonal-vectors.md)
2. [Inner product](inner-product-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge/2015/paper-1/3/b/solution.md)
