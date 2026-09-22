<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

A [group representation](../../../../group-representation.md) on a vector space $W$ is a [group homomorphism](../../../../group-homomorphism.md) $\rho:G\to GL(W)$: $\rho(gh)=\rho(g)\rho(h)$ and $\rho(e)=I$. An [invariant subspace](../../../../invariant-subspace.md) $U$ obeys $\rho(g)U\subseteq U$ for every $g$. A nonzero representation is [irreducible](../../../../irreducible-representation.md) if its only invariant subspaces are $0$ and $W$. It is a [faithful representation](../../../../faithful-representation.md) if it is injective, equivalently if its [group kernel](../../../../kernel-of-a-group-homomorphism.md) is $\{e\}$. Its [character](../../../../character-of-a-representation.md) is $\chi_\rho(g)=\operatorname{tr}\rho(g)$. For inequivalent complex [irreducible representations](../../../../irreducible-representation.md) of a finite group, [character orthogonality](../../../../character-orthogonality.md) is

$$
\boxed{\frac1{|G|}\sum_{g\in G}\overline{\chi_\alpha(g)}\chi_\beta(g)=\delta_{\alpha\beta}.}
$$

Use right-to-left composition of [permutations](../../../../permutation.md) and assign the matrix labels consistently by

$$
I=e,\quad A=(123),\quad B=(132),\quad C=(13),\quad D=(12),\quad E=(23).
$$

The resulting [Cayley table](../../../../cayley-table.md), with row multiplying column, is

$$
\begin{array}{c|cccccc}
 &I&A&B&C&D&E\\\hline
I&I&A&B&C&D&E\\
A&A&B&I&E&C&D\\
B&B&I&A&D&E&C\\
C&C&D&E&I&A&B\\
D&D&E&C&B&I&A\\
E&E&C&D&A&B&I
\end{array}.
$$

Conjugation relabels the entries of a cycle, preserving its length. Thus the [conjugacy classes](../../../../conjugacy-class.md) are

$$
\boxed{\{I\},\qquad\{A,B\},\qquad\{C,D,E\}.}
$$

Define the [permutation representation](../../../../permutation-representation.md) by $P_\sigma e_j=e_{\sigma(j)}$, or $(P_\sigma)_{ij}=\delta_{i,\sigma(j)}$. Applying it to a basis vector proves $P_\sigma P_\tau=P_{\sigma\tau}$. The six assignments above produce exactly the listed matrices. They are distinct, and $P_\sigma=I$ forces $\sigma(j)=j$ for every $j$, so the representation is faithful.

Every permutation fixes $(1,1,1)$, hence fixes every vector $(c,c,c)$. Therefore $V_0$ is a one-dimensional [invariant subspace](../../../../invariant-subspace.md) carrying the [trivial representation](../../../../trivial-representation.md). Its [orthogonal complement](../../../../orthogonal-complement.md) is

$$
V_0^\perp=\{(v_1,v_2,v_3):v_1+v_2+v_3=0\},
$$

since the inner product with $(c,c,c)$ is $c(v_1+v_2+v_3)$. Permuting coordinates preserves their sum, so this plane is invariant too. Every real vector has the unique decomposition

$$
v=\frac{v_1+v_2+v_3}{3}(1,1,1)+\left[v-\frac{v_1+v_2+v_3}{3}(1,1,1)\right].
$$

Thus the [permutation representation](../../../../permutation-representation.md) is the [direct sum](../../../../direct-sum.md) of [group representations](../../../../group-representation.md) on the line and the plane.

To find the [eigenvectors](../../../../eigenvector.md) of $A$, note that $A(v_1,v_2,v_3)=(v_3,v_1,v_2)$. With $\zeta=e^{2\pi i/3}$, its three [eigenvalues](../../../../eigenvalue.md) and eigenspaces are

$$
\boxed{\begin{array}{c|c}
1&\operatorname{span}(1,1,1)\\
\zeta&\operatorname{span}(1,\zeta^2,\zeta)\\
\zeta^2&\operatorname{span}(1,\zeta,\zeta^2)
\end{array}.}
$$

The only real eigenvalue is one, whose eigenline is $V_0$, so $A$ has no nonzero real [eigenvector](../../../../eigenvector.md) in $V_0^\perp$. A proper nonzero real invariant subspace of that two-dimensional plane would be a line, giving such an eigenvector. Hence the plane representation is irreducible over $\mathbb R$.

For the later complex dimension-count theorem one should also establish irreducibility over $\mathbb C$; real irreducibility alone would not imply it in general. In the complexified plane, the only candidate $A$-invariant lines are its $\zeta$ and $\zeta^2$ eigenlines. But $C$ exchanges them:

$$
C(1,\zeta^2,\zeta)=\zeta(1,\zeta,\zeta^2),\qquad
C(1,\zeta,\zeta^2)=\zeta^2(1,\zeta^2,\zeta).
$$

Neither is invariant under the whole group, proving complex irreducibility as well. The required decomposition is therefore

$$
\boxed{P\cong\mathbf1\oplus W,\qquad \dim W=2,}
$$

where $W$ is the [standard representation of the symmetric group](../../../../standard-representation-of-the-symmetric-group.md) for three letters. Its character is obtained by subtracting one from the number of fixed coordinates: on the three classes it is $(2,-1,0)$.

Finally, the [sign representation](../../../../sign-representation.md) gives a second one-dimensional irreducible, with value $+1$ on $I,A,B$ and $-1$ on the transpositions. These are exactly the two one-dimensional possibilities: if $r=A,s=C$, a one-dimensional representation sends them to commuting nonzero scalars $v,u$. The relations $r^3=s^2=e$ and $srs=r^{-1}$ imply $v^3=u^2=1$ and $v=v^{-1}$. Hence $v=1$ and $u=\pm1$, the trivial and sign choices. Together with the two-dimensional $W$, these give

$$
1^2+1^2+2^2=6=|\Sigma_3|.
$$

The [sum of squares of irreducible representation dimensions](../../../../sum-of-squares-of-irreducible-representation-dimensions.md) leaves room for no other irreducible. Thus there are **exactly two one-dimensional and one two-dimensional complex irreducible representations**.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 2](../../paper-2-split.md)
3. [2010](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
