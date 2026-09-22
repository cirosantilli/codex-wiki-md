<h1 id="1/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Choose a representative [Sylow subgroup](../../../../../../sylow-subgroup.md) with generators

$$
r=(1\ 2\ 3\ 4),\qquad s=(1\ 3),\qquad t=(5\ 6).
$$

On the first four points, $r^4=s^2=1$ and $srs=r^{-1}$, so $\langle r,s\rangle$ is the [dihedral group](../../../../../../dihedral-group.md) of order eight. The disjoint [transposition](../../../../../../transposition-permutation.md) $t$ commutes with it and generates an independent factor of order two. Thus $G=\langle r,s,t\rangle\cong D_8\times C_2$ has order 16. Since the power of two dividing $7!$ is $2^{\lfloor7/2\rfloor+\lfloor7/4\rfloor}=2^4$, this is a Sylow 2-subgroup of $S_7$. Any other choice is conjugate to it and has conjugate series.

The dihedral relation gives $[r,s]=r^2$, while $t$ commutes with both generators. Modulo $\langle r^2\rangle$ all three generators commute, so the [commutator subgroup](../../../../../../commutator-subgroup.md) is exactly $\langle r^2\rangle$, and $r^2$ is central. Hence the [lower central series](../../../../../../lower-central-series.md) is

$$
\boxed{\Gamma_1(G)=G,\qquad \Gamma_2(G)=\langle(1\ 3)(2\ 4)\rangle,\qquad \Gamma_3(G)=1.}
$$

Within the dihedral factor only $1,r^2$ commute with both $r$ and $s$. The center of $G$ is therefore $\langle r^2,t\rangle\cong C_2\times C_2$. Its quotient has order four and is abelian, so the [upper central series](../../../../../../upper-central-series.md) is

$$
\boxed{Z_0(G)=1,\qquad Z_1(G)=\langle(1\ 3)(2\ 4),(5\ 6)\rangle,\qquad Z_2(G)=G.}
$$

Both series show that the [nilpotency class](../../../../../../nilpotency-class.md) is two.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
