# Central spring stiffness matrix

↑ **Parent:** [Spring](spring.md)

For point masses joined by unstretched central [springs](spring.md) obeying [Hooke's law](hooke-s-law.md), let $n_{ij}$ be the equilibrium [unit vector](unit-vector.md) along an edge and $u_i$ the small [displacement](displacement.md) of its endpoint. The leading extension is $n_{ij}\cdot(u_j-u_i)$, so its quadratic [elastic potential energy](elastic-energy.md) is $k_{ij}[n_{ij}\cdot(u_j-u_i)]^2/2$. Consequently the block [stiffness matrix](stiffness-matrix.md) has off-diagonal blocks $K_{ij}=-k_{ij}n_{ij}n_{ij}^T$ and diagonal blocks $K_{ii}=\sum_jk_{ij}n_{ij}n_{ij}^T$, with absent edges contributing zero. It is [symmetric](symmetric-relation.md) and [positive semidefinite](positive-semidefinite-matrix.md). The [normal modes](normal-mode.md) solve $Kq=\omega^2Mq$, where $M$ is the [mass matrix](mass-matrix.md). Rigid translations and infinitesimal rotations are [rigid-motion zero modes of a spring framework](rigid-motion-zero-modes-of-a-spring-framework.md). A prestressed spring can add transverse quadratic terms, so the unstretched assumption matters.

## ↑ Ancestors (8)

1. [Spring](spring.md)
2. [Hooke's law](hooke-s-law.md)
3. [Linear elasticity](linear-elasticity.md)
4. [Elasticity (physics)](elasticity-physics-split.md)
5. [Continuum mechanics](continuum-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2/7/solution.md)
