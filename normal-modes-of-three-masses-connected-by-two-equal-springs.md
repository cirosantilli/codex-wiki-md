# Normal modes of three masses connected by two equal springs

↑ **Parent:** [Generalized eigenvalue problem for small oscillations](generalized-eigenvalue-problem-for-small-oscillations.md)

For three collinear masses $m,\mu m,m$, with $m>0$, $\mu>0$, connected consecutively by two springs of stiffness $k>0$ and with free ends, let $x$ denote displacements from an [equilibrium](equilibrium-point-of-a-dynamical-system.md). The [kinetic energy](kinetic-energy.md) and [potential energy](potential-energy.md) are $T=\dot x^TM\dot x/2$, $V=x^TKx/2$, where

$$
M=m\operatorname{diag}(1,\mu,1),\qquad K=k\begin{pmatrix}1&-1&0\\-1&2&-1\\0&-1&1\end{pmatrix}.
$$

The [generalized eigenvalue problem for small oscillations](generalized-eigenvalue-problem-for-small-oscillations.md) $Kv=\omega^2Mv$ has

$$
\begin{array}{c|c|c}
&v&\omega^2\\\hline
0&(1,1,1)^T&0\\
1&(1,0,-1)^T&k/m\\
2&(1,-2/\mu,1)^T&(k/m)(1+2/\mu)
\end{array}.
$$

Direct substitution verifies each pair; the three distinct [eigenvalues](eigenvalue.md) exhaust the three-dimensional problem. The zero [normal mode](normal-mode.md) translates the complete system without extending either spring. The second holds the middle mass fixed while the end masses move oppositely. The third moves the end masses together and the middle mass oppositely, leaving the [centre of mass](center-of-mass.md) fixed.

For [mass-matrix orthogonality of normal modes](mass-matrix-orthogonality-of-normal-modes.md), the squared norms $v^TMv$ are respectively $m(\mu+2)$, $2m$ and $m(2+4/\mu)$. Dividing each shape by its corresponding square root gives $q_i^TMq_j=\delta_{ij}$. The general motion is a linear combination of the two oscillatory modes and $(A+Bt)v_0$; the latter describes free translation with constant velocity.

**Table of contents**

- [Impulse on an end mass of a free symmetric three-mass chain](impulse-on-an-end-mass-of-a-free-symmetric-three-mass-chain.md)

## ↑ Ancestors (7)

1. [Generalized eigenvalue problem for small oscillations](generalized-eigenvalue-problem-for-small-oscillations.md)
2. [Small oscillation](small-oscillation.md)
3. [Lagrangian mechanics](lagrangian-mechanics-split.md)
4. [Classical mechanics](classical-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-2/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2/7/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2/7/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a/section-d/d14/solution.md)
