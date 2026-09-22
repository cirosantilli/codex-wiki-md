<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [decomposition matrix](../../../../../../decomposition-matrix-modular-representation-theory.md) separates into two connected components. The first contains $\phi_1,\phi_2$ and $\chi_1,\chi_{3A},\chi_{3B},\chi_4$; it is the principal block $B_0$. The second contains only $\phi_3$ and $\chi_5$; since $\phi_3(1)=5$ contains the full 5-part of $|A_5|=60$, this is a [defect-zero representation](../../../../../../defect-zero-representation.md) and its block $B_1$ has defect group $1$.

For $D=1$, the [normalizer](../../../../../../normalizer.md) is $N_G(1)=G$, so the [Brauer correspondence](../../../../../../brauer-correspondence.md) is the identity and $B_1$ corresponds to itself.

The defect group of the principal block is a Sylow 5-subgroup $P\cong C_5$. There are six Sylow 5-subgroups in $A_5$, so the [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md) gives

$$
|N_{A_5}(P)|=\frac{60}{6}=10.
$$

The [centralizer](../../../../../../centralizer.md) of a 5-cycle in $A_5$ is $P$, and an involution in the normalizer acts on $P$ by inversion. Hence

$$
N=N_{A_5}(P)\cong C_5\rtimes C_2\cong D_{10}.
$$

In characteristic five the simple $kN$-modules are inflated from $N/P\cong C_2$: their [Brauer characters](../../../../../../brauer-character.md) are $\psi_+=(1,1)$ and $\psi_-=(1,-1)$ on the identity and involution classes. If $1,\varepsilon,\rho_1,\rho_2$ are the two one-dimensional and two two-dimensional ordinary characters of $D_{10}$, their reductions are

$$
1\mapsto\psi_+,
\qquad
\varepsilon\mapsto\psi_-,
\qquad
\rho_1,\rho_2\mapsto\psi_++\psi_-.
$$

The resulting [decomposition matrix](../../../../../../decomposition-matrix-modular-representation-theory.md) is connected, so these characters form the unique 5-block $b_0$ of $N$, with defect group $P$. By the [Brauer first main theorem](../../../../../../brauer-first-main-theorem.md),

$$
\boxed{B_0\longleftrightarrow b_0\text{ for }D=C_5,
\qquad B_1\longleftrightarrow B_1\text{ for }D=1.}
$$

This is the complete [5-modular blocks of A5](../../../../../../5-modular-blocks-of-a5.md) correspondence.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
