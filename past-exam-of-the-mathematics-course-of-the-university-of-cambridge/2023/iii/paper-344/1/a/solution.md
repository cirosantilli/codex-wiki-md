<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Because $\phi$ is a conserved composition density, an infinitesimal material displacement $\mathbf r\mapsto\mathbf r+\mathbf u$ changes it at fixed position by

$$
\delta\phi=-\nabla\mathbin\cdot(\phi\mathbf u)
=-\mathbf u\mathbin\cdot\nabla\phi-\phi\nabla\mathbin\cdot\mathbf u.
$$

The second term is essential when the deformation is compressible. By the definition of the [chemical potential](../../../../../../chemical-potential.md), and taking $\mathbf u$ to vanish on the boundary,

$$
\delta F=\int\mu\,\delta\phi\,d\mathbf r
=-\int\mu\nabla\mathbin\cdot(\phi\mathbf u)d\mathbf r
=\int\phi\nabla_j\mu\,u_jd\mathbf r.
$$

The same free-energy change written in terms of the [stress tensor](../../../../../../stress.md) is

$$
\delta F=\int\Sigma_{ij}\nabla_i u_jd\mathbf r
=-\int(\nabla_i\Sigma_{ij})u_jd\mathbf r.
$$

Since $\mathbf u$ is arbitrary,

$$
\boxed{\nabla_i\Sigma_{ij}=-\phi\nabla_j\mu.}
$$

This is the [Korteweg force](../../../../../../korteweg-force.md) density of a diffuse-interface mixture.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
