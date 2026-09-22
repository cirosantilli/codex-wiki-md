<h1 id="18g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The identity is one [conjugacy class](../../../../../../conjugacy-class.md). In $N\setminus\{1\}$, conjugation by $c$ pairs each element with its inverse, giving four classes represented by $a,b,ab,ab^2$, each of size two. All nine elements of $Nc$ are conjugate, since conjugation by $n\in N$ changes the reflection component by $n^2$ and squaring is a bijection of $N$.

There are two [linear characters](../../../../../../linear-character.md): the trivial character and the character equal to one on $N$ and minus one on $Nc$. Write $\omega=e^{2\pi i/3}$. The remaining four irreducible [characters of a representation](../../../../../../character-of-a-representation.md) are induced from the nontrivial characters $a^i b^j\mapsto\omega^{ri+sj}$ of $N$, pairing $(r,s)$ with $(-r,-s)$. They are exactly the two-dimensional representations already proved irreducible. Taking representatives $(1,0),(0,1),(1,1),(1,2)$ yields the [character table](../../../../../../character-table.md)

$$
\begin{array}{c|rrrrrr}
&1&a&b&ab&ab^2&c\\\hline
\text{class size}&1&2&2&2&2&9\\\hline
1&1&1&1&1&1&1\\
\mathrm{sgn}&1&1&1&1&1&-1\\
\chi_{10}&2&-1&2&-1&-1&0\\
\chi_{01}&2&2&-1&-1&-1&0\\
\chi_{11}&2&-1&-1&-1&2&0\\
\chi_{12}&2&-1&-1&2&-1&0
\end{array}
$$

Indeed the induced value on $a^i b^j$ is $\omega^{ri+sj}+\omega^{-(ri+sj)}$, equal to two or minus one, and is zero off $N$. The squared dimensions sum to $1+1+4\cdot4=18$, so this is the complete table.

An element of $N$ centralizes $c$ only if it equals its inverse, hence only if it is the identity. No reflection centralizes $a$. Thus $Z(E)=\{1\}$ is cyclic, but the two linear representations kill $N$ and each two-dimensional irreducible has a nontrivial [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md) of order three. Therefore **a cyclic centre does not imply a faithful [irreducible representation](../../../../../../irreducible-representation.md)**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18G](../../18g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
