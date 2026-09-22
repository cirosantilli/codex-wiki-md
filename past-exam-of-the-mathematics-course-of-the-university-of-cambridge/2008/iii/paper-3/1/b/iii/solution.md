<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the positive simple-root [raising operators](../../../../../../../raising-operator.md) $E_{12}=x_1\partial_{x_2}$ and $E_{23}=x_2\partial_{x_3}$. On the weight space of $2L_1-L_3$, the first maps both $s_{11}\otimes s_{12}$ and $s_{12}\otimes s_{11}$ to $s_{11}\otimes s_{11}$, while the second annihilates both. Consequently

$$
\boxed{v=s_{11}\otimes s_{12}-s_{12}\otimes s_{11}}
$$

is a nonzero [highest-weight vector](../../../../../../../highest-weight-vector.md); the remaining positive-root operator $E_{13}=[E_{12},E_{23}]$ also annihilates it. Its [Dynkin labels](../../../../../../../dynkin-label.md) are $(2,1)$, and the generated submodule $Z$ is the irreducible [highest-weight representation](../../../../../../../highest-weight-representation.md) with that highest weight.

Put $F_1=E_{21}=x_2\partial_{x_1}$ and $F_2=E_{32}=x_3\partial_{x_2}$, acting on both tensor factors. Direct calculation gives

$$
F_1v=s_{11}\otimes s_{22}-s_{22}\otimes s_{11},\qquad
F_2v=s_{11}\otimes s_{13}-s_{13}\otimes s_{11}.
$$

Define the linearly independent tensors

$$
A=s_{11}\otimes s_{23}-s_{23}\otimes s_{11},\qquad
B=s_{12}\otimes s_{13}-s_{13}\otimes s_{12}.
$$

They both have weight $L_1$, and

$$
F_2F_1v=2A,\qquad F_1F_2v=A+2B.
$$

Therefore $A,B\in Z_{L_1}$. To prove that they exhaust this [weight space](../../../../../../../weight-space.md), its weight differs from the highest weight by $(L_1-L_2)+(L_2-L_3)$. The [Poincaré-Birkhoff-Witt theorem](../../../../../../../poincare-birkhoff-witt-theorem.md) expresses all descendants at that difference using $F_2F_1v$ and $F_1F_2v$: the third possible operator $E_{31}=[F_2,F_1]$ is their difference. Hence the space has dimension at most two, and the two independent vectors already found give

$$
\boxed{Z_{L_1}=\operatorname{span}\{A,B\}.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
