<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The four displayed matrices fail [closure](../../../../../closure-topology.md): for example $\sigma_x\sigma_y=i\sigma_z$ is not one of them. Thus they do not form a [group](../../../../../group-split.md) by themselves.

Let $\sigma_0=I$ and $\mu_4=\{1,-1,i,-i\}$. The enlarged set is the single-qubit [Pauli group](../../../../../pauli-group.md)

$$
\boxed{\mathcal P_1=\{\eta\sigma_a:\eta\in\mu_4,\ a\in\{0,x,y,z\}\}.}
$$

There are 16 distinct matrices: $I,\sigma_x,\sigma_y,\sigma_z$ are linearly independent, so two different ones cannot be scalar multiples, and the four phases are distinct for each nonzero matrix.

The [Pauli matrices](../../../../../pauli-matrices.md) satisfy

$$
\sigma_a\sigma_b=\delta_{ab}I+i\epsilon_{abc}\sigma_c\quad(a,b\in\{x,y,z\}),\qquad\sigma_a^2=I.
$$

Here $\delta$ is the [Kronecker delta](../../../../../kronecker-delta.md) and $\epsilon$ the [Levi-Civita symbol](../../../../../levi-civita-symbol.md). Thus any product of two Pauli matrices is another Pauli matrix or the identity times a phase in $\mu_4$. Multiplying by the two original phases preserves membership in $\mu_4$, proving [closure](../../../../../closure-topology.md) of all 16 matrices.

[Associativity](../../../../../associative-property.md) is inherited from [matrix multiplication](../../../../../matrix-multiplication.md), the identity is $I$, and

$$
(\eta\sigma_a)^{-1}=\eta^{-1}\sigma_a\in\mathcal P_1.
$$

This proves every group axiom. The resulting group is non-Abelian, since reversing $\sigma_x\sigma_y$ changes its sign.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
