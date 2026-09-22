<h1 id="17f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Here one must distinguish two conventions for a [radical extension](../../../../../../radical-extension.md). The solvability theorem says that a finite extension with solvable normal-closure [Galois group](../../../../../../galois-group.md) is contained in a tower of radical adjunctions. Under the convention that this containment defines a radical extension, this is the requested assertion.

Let $N/K$ be the finite normal closure and let $m$ be divisible by the orders of its [Galois group](../../../../../../galois-group.md) elements. Adjoin a primitive $m$th [root of unity](../../../../../../root-of-unity.md), obtaining $K'=K(\zeta_m)$, which itself is a radical adjunction since $\zeta_m^m=1$. The [Galois group](../../../../../../galois-group.md) of $NK'/K'$ embeds in the solvable group of $N/K$, so it is solvable. A composition series with cyclic prime-order quotients gives a tower of cyclic prime-degree extensions above $K'$. Each is a radical adjunction, as the following argument shows.

For a cyclic extension $E/F$ of prime degree $p$ containing $\zeta_p$, let $\sigma$ generate its [Galois group](../../../../../../galois-group.md). The $F$-linear operator $\sigma$ satisfies $X^p-1$, a product of distinct linear factors in characteristic zero. Thus it is diagonalizable. Because $\sigma\ne1$, it has an eigenvector $a\ne0$ with eigenvalue $\zeta_p^j\ne1$. Then $a^p\in F$ and $a\notin F$, so $E=F(a)$ by primeness of the degree. Applying this at every step produces a radical tower containing $L$.

If “radical extension” instead means that $L/K$ itself must be such a tower, the printed statement is false without this qualification. For example the real cubic subfield of $\mathbb Q(\zeta_7)$ is cyclic and solvable, but contains no nonrational $a$ with $a^n\in\mathbb Q$: all three conjugates are real roots of the same equation $X^n=a^n$, which has at most two real roots, while any nonrational element of the cubic field has three distinct conjugates. Consequently no nontrivial radical adjunction can start a tower inside it. **Containment in a radical tower is the valid general conclusion.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [17F](../../17f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
