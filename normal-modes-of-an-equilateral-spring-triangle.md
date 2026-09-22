# Normal modes of an equilateral spring triangle

↑ **Parent:** [Generalized eigenvalue problem for small oscillations](generalized-eigenvalue-problem-for-small-oscillations.md)

Three equal point [masses](mass.md) $m>0$ move in a plane and are connected pairwise by ideal [springs](spring.md) of equal positive stiffness $k$. At an unstretched [equilateral triangle](equilateral-triangle.md) equilibrium, let $r_i$ be the vertex positions relative to the centre, and let $u_i$ be small displacements. If $e_{ij}=(r_i-r_j)/|r_i-r_j|$, the quadratic [potential energy](potential-energy.md) is $(k/2)\sum_{i<j}[e_{ij}\cdot(u_i-u_j)]^2$, and the [kinetic energy](kinetic-energy.md) is $(m/2)\sum_i|\dot u_i|^2$.

There are three independent zero-frequency motions: two common translations and the infinitesimal rigid rotation $u_i=Jr_i$, where $J(x,y)=(-y,x)$. The uniform radial motion $u_i=r_i$ is the breathing [normal mode](normal-mode.md), with $\omega^2=3k/m$. The two shear modes are $u_i=(r_{ix},-r_{iy})$ and $u_i=(r_{iy},r_{ix})$, each with $\omega^2=3k/(2m)$.

For a compact proof of the spectrum, form the $3\times6$ [matrix](matrix.md) $B$ taking the six displacement components to the three first-order spring extensions, orienting the three edges cyclically. Its row norms squared are two, and every pair of rows has [inner product](inner-product-split.md) $1/2$. Thus $BB^T=(3/2)I+(1/2)\mathbf1\mathbf1^T$, with [eigenvalues](eigenvalue.md) $3,3/2,3/2$. The nonzero [eigenvalues](eigenvalue.md) of $B^TB$ are the same, so the stiffness matrix $kB^TB$ has the three positive values in the title and a three-dimensional [kernel of a linear map](kernel-of-a-linear-map-split.md). The three rigid motions span that kernel. A zero mode has time factor $A+Bt$ rather than a nonconstant periodic oscillation.

## ↑ Ancestors (7)

1. [Generalized eigenvalue problem for small oscillations](generalized-eigenvalue-problem-for-small-oscillations.md)
2. [Small oscillation](small-oscillation.md)
3. [Lagrangian mechanics](lagrangian-mechanics-split.md)
4. [Classical mechanics](classical-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-2/7/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/7/solution.md)
