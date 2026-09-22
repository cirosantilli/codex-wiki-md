<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $N$ labelled particles with collisions excluded, [Newtonian gravity](../../../../../../gravitational-acceleration.md) has

$$
L=\frac12\sum_i m_i|\dot{\mathbf q}_i|^2+G\sum_{i<j}\frac{m_im_j}{|\mathbf q_i-\mathbf q_j|}.
$$

Simultaneously translating every position or applying the same time-independent spatial rotation preserves both [kinetic energy](../../../../../../kinetic-energy.md) and the distance-dependent potential. The conserved [momentum](../../../../../../momentum.md) and [angular momentum](../../../../../../angular-momentum.md) obtained from [Noether's theorem](../../../../../../noether-conserved-quantity-for-a-mechanical-point-symmetry.md) are

$$
\boxed{\mathbf P=\sum_i\mathbf p_i,\qquad\mathbf L=\sum_i\mathbf q_i\times\mathbf p_i.}
$$

Time translations give the conserved Hamiltonian. Galilean boosts change the Lagrangian by a total derivative, rather than leaving it strictly unchanged; they give the conserved centre-of-mass quantity $M\mathbf R-t\mathbf P$, where $M=\sum_i m_i$ and $\mathbf R=M^{-1}\sum_i m_i\mathbf q_i$. Thus absolute uniform velocity is not singled out by the isolated dynamics.

Translations can be separated explicitly. Put $\mathbf r_i=\mathbf q_i-\mathbf R$, so $\sum_i m_i\mathbf r_i=0$. Then

$$
\frac12\sum_i m_i|\dot{\mathbf q}_i|^2=\frac12M|\dot{\mathbf R}|^2+\frac12\sum_i m_i|\dot{\mathbf r}_i|^2,
$$

with the cross-term vanishing. The potential depends only on $\mathbf r_i-\mathbf r_j$. The centre-of-mass motion is therefore a decoupled free motion; at fixed $\mathbf P$ its energy is $\mathbf P^2/(2M)$ and it can be eliminated from the internal equations. Choosing a centre-of-mass rest frame sets $\mathbf P=0$.

One can then quotient internal configurations by simultaneous rotations. On generic noncollinear configurations with $N\ge3$ the resulting [relational shape space](../../../../../../relational-shape-space.md) has dimension $3N-6$; collinear configurations have stabilizers and belong to singular strata. For two particles only the separation remains, so that generic dimension formula is inapplicable. This configuration quotient identifies absolute placement and orientation, but it does not by itself specify all the reduced dynamics.

At the phase-space level, [symplectic reduction](../../../../../../symplectic-reduction.md) is performed at a fixed moment-map value: $J^{-1}(\mu)/G_\mu$, where $G_\mu$ is the coadjoint [stabilizer](../../../../../../stabilizer-subgroup.md). In particular, at fixed nonzero [angular momentum](../../../../../../angular-momentum.md) one does not simply divide the [momentum](../../../../../../momentum.md) level by every rotation. The reduction retains the appropriate angular-momentum data and centrifugal effects. Even for two gravitating particles, specifying $r$ and $\dot r$ alone is insufficient unless the angular-momentum parameter is supplied:

$$
\ddot r=\frac{\ell^2}{\mu_r^2r^3}-\frac{G(m_1+m_2)}{r^2},\qquad\mu_r=\frac{m_1m_2}{m_1+m_2}.
$$

Systems with identical instantaneous separation and radial velocity but different $\ell$ have different radial futures. Eliminating orientation while discarding this parameter would not be a faithful reduction.

These results support a relational treatment of overall position and orientation: isolated configurations differing only by one fixed translation or rotation have the same internal predictions. However, a [symmetry](../../../../../../symmetry-physics.md) and a declared gauge equivalence are conceptually different, and the quotient alone does not settle the ontology of space. Arbitrary time-dependent rotations are not [symmetries](../../../../../../symmetry-physics.md) of the original inertial equations; a rotating coordinate description brings Coriolis and centrifugal terms. Newtonian inertial structure and absolute acceleration therefore cannot be eliminated merely by citing rotational invariance. A relational theory may encode that structure through additional dynamical or connection data, but it must reproduce these effects rather than erase them.

**The [symmetries](../../../../../../symmetry-physics.md) license mathematically controlled elimination of collective variables, with [momentum](../../../../../../momentum.md) and regularity qualifications; they do not alone prove either absolute space or complete relationalism.** This distinguishes redundant descriptions of a solution from genuinely different possible motions.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
