<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [matrices](../../../../matrix.md) obey $Q^5=P^2=I$ and $PQP=Q^{-1}$. Moving every $P$ to the right therefore reduces every product to $Q^k$ or $Q^kP$, with $0\leq k<5$. The five diagonal [matrices](../../../../matrix.md) $Q^k$ are distinct because $\alpha$ is a primitive fifth [root of unity](../../../../root-of-unity.md); the five $Q^kP$ are distinct and off-diagonal. Thus

$$
\boxed{G=\{Q^k,Q^kP:0\leq k<5\},\qquad |G|=10.}
$$

This is the [dihedral group](../../../../dihedral-group.md) of the regular pentagon, with $Q$ a rotation and $P$ a reflection.

Conjugation by $P$ interchanges $Q^k$ and $Q^{-k}$, while conjugation by a power of $Q$ fixes rotations. Also

$$
Q^j(Q^kP)Q^{-j}=Q^{k+2j}P.
$$

Since multiplication by $2$ permutes the residues modulo $5$, all five reflections form one [conjugacy class](../../../../conjugacy-class.md). The full list of [conjugacy classes](../../../../conjugacy-class.md) is

$$
\boxed{\{I\},\quad\{Q,Q^4\},\quad\{Q^2,Q^3\},\quad\{P,QP,Q^2P,Q^3P,Q^4P\}.}
$$

To prove the [representation](../../../../group-representation.md) is [irreducible](../../../../irreducible-representation.md) over $\mathbb C$, any proper nonzero [invariant subspace](../../../../invariant-subspace.md) would be a line invariant under $Q$. Its two distinct [eigenvalues](../../../../eigenvalue.md) force such a line to be one of its coordinate [eigenspaces](../../../../eigenspace.md). But $P$ exchanges those two lines, so neither is $G$-invariant. Hence the given [complex representation](../../../../complex-representation.md) is [irreducible](../../../../irreducible-representation.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../b/solution.md)
