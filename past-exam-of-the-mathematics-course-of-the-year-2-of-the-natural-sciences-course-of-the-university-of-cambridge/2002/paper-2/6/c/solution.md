<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Contract the given [isotropic fourth-rank tensor](../../../../../isotropic-fourth-rank-tensor.md) with the [strain](../../../../../strain.md) array. The [stress tensor](../../../../../cauchy-stress-tensor.md) is

$$
P_{ij}=\lambda\delta_{ij}p_{kk}+\mu p_{ij}+\nu p_{ji}.
$$

Write $p_{ij}=p\delta_{ij}+s_{ij}+\epsilon_{ijk}a_k$, where $s_{ij}$ is symmetric and traceless. Then $p_{kk}=3p$ and $p_{ji}=p\delta_{ij}+s_{ij}-\epsilon_{ijk}a_k$. Substitution gives

$$
P_{ij}=(3\lambda+\mu+\nu)p\delta_{ij}+(\mu+\nu)s_{ij}+(\mu-\nu)\epsilon_{ijk}a_k.
$$

By uniqueness of the [scalar, symmetric-traceless and axial tensor decomposition](../../../../../scalar-symmetric-traceless-and-axial-tensor-decomposition.md),

$$
\boxed{P=(3\lambda+\mu+\nu)p,\qquad S_{ij}=(\mu+\nu)s_{ij},\qquad A_k=(\mu-\nu)a_k.}
$$

This is [isotropic elasticity on tensor components](../../../../../isotropic-elasticity-on-tensor-components.md): the three tensor sectors do not mix. If the [strain](../../../../../strain.md) is symmetric, $a_k=0$, hence $A_k=0$ and $\boxed{P_{ij}=P_{ji}}$. No equality between $\mu$ and $\nu$ is needed for that conclusion.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
