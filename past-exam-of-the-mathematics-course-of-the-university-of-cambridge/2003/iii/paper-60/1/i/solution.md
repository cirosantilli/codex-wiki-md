<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose amplitude coordinates in which a quarter-turn and a diagonal [reflection](../../../../../../reflection-mathematics.md) act as $r(A,B)=(B,-A)$ and $s(A,B)=(-A,B)$. These generate the natural two-dimensional [group representation](../../../../../../group-representation.md) of the [dihedral group](../../../../../../dihedral-group.md) $D_4$. An [equivariant dynamical system](../../../../../../equivariant-dynamical-system.md) satisfies $F(gv)=gF(v)$. The two independent sign changes make $F_A$ odd in $A$ and even in $B$, and $F_B$ odd in $B$ and even in $A$. The quarter-turn equates the two linear coefficients and the two sets of cubic coefficients. No quadratic monomial is allowed. Thus the [square-symmetric cubic steady-state normal form](../../../../../../square-symmetric-cubic-steady-state-normal-form.md) is

$$
\boxed{A_T=\mu A-aA^3-bAB^2+O(|(A,B)|^5),\qquad B_T=\mu B-aB^3-bA^2B+O(|(A,B)|^5).}
$$

The [bifurcation parameter](../../../../../../bifurcation-parameter.md) has been scaled so that the critical linear [eigenvalue](../../../../../../eigenvalue.md) is $\mu$. Nondegeneracy at cubic order means $a\ne0$, $a+b\ne0$ and $a-b\ne0$. The [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) equations factor as $A(\mu-aA^2-bB^2)=B(\mu-aB^2-bA^2)=0$. When both components are nonzero, subtracting the two bracketed expressions gives $(a-b)(A^2-B^2)=0$. Therefore the complete leading list of small steady branches is:

- The zero state, with two linear [eigenvalues](../../../../../../eigenvalue.md) $\mu$.
- Four axial states $(\pm\sqrt{\mu/a},0)$ and $(0,\pm\sqrt{\mu/a})$, when $\mu/a>0$. Their [stability matrix](../../../../../../stability-matrix.md) has [eigenvalues](../../../../../../eigenvalue.md) $-2\mu$ and $\mu(1-b/a)$.
- Four diagonal states $(\pm s,\pm s)$, with independent signs and $s^2=\mu/(a+b)>0$. Their [eigenvalues](../../../../../../eigenvalue.md) are $-2\mu$ and $2\mu(b-a)/(a+b)$.

Each family is one orbit of the [dihedral group](../../../../../../dihedral-group.md). Each nonzero state retains one [reflection](../../../../../../reflection-mathematics.md) fixing its amplitude line; its full spatial symmetry depends also on the chosen planforms. Higher-order terms perturb the branch amplitudes but preserve the nondegenerate local classification. For $\mu>0$, an axial branch is [asymptotically stable](../../../../../../asymptotic-stability.md) precisely when $a>0$ and $b>a$, while a diagonal branch is [asymptotically stable](../../../../../../asymptotic-stability.md) precisely when $a+b>0$ and $b<a$. Every cubic branch lying on $\mu<0$ has a positive radial [eigenvalue](../../../../../../eigenvalue.md) $-2\mu$, so it is unstable. In the exceptional isotropic cubic case $a=b$, the cubic truncation instead has a circle of [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md); higher-order anisotropy is then needed, which is why that case was excluded.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
