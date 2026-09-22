<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a [primitive Dirichlet character](../../../../../../primitive-dirichlet-character.md) the previous formula gives $|\widehat\chi(a)|=|\chi(a)|\,|\widehat\chi(1)|$. The [Plancherel theorem](../../../../../../plancherel-theorem.md) for the unitary finite transform yields

$$
\varphi(q)=\sum_{n\bmod q}|\chi(n)|^2
=\sum_{a\bmod q}|\widehat\chi(a)|^2
=\varphi(q)|\widehat\chi(1)|^2.
$$

Thus $|\widehat\chi(1)|=1$, the normalized [Gauss sum of a Dirichlet character](../../../../../../gauss-sum-of-a-dirichlet-character.md) magnitude.

For an imprimitive character modulo $p^k$ with $k\ge2$, its values on residues are periodic modulo $p^{k-1}$: descent preserves the values on units, and divisibility by $p$ is unchanged by that shift. Splitting the sum into these [residue classes](../../../../../../residue-class.md) gives a factor $\sum_{j=0}^{p-1}e(-j/p)=0$. Hence $\widehat\chi(1)=0$. If $k=1$, the only imprimitive character is principal, and its Gauss sum is $\sum_{n=1}^{p-1}e(-n/p)=-1$, giving $|\widehat\chi(1)|=p^{-1/2}$. All cases satisfy the required bound.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
