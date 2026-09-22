<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Maximal [right ideals](../../../../../../right-ideal.md) of $R/J$ correspond to [maximal right ideals](../../../../../../maximal-right-ideal.md) of $R$, all of which contain $J$. Their intersection in the quotient is zero. Hence $R/J$ is a [right Artinian ring](../../../../../../right-artinian-ring.md) with zero [Jacobson radical](../../../../../../jacobson-radical.md), and part (a) makes it semisimple.

Part (b) gives the finite radical filtration

$$
R\supseteq J\supseteq J^2\supseteq\cdots\supseteq J^m=0.
$$

Each factor $J^i/J^{i+1}$ is annihilated by $J$, so it is a right [module](../../../../../../module-mathematics.md) over $R/J$. Every [module](../../../../../../module-mathematics.md) over a semisimple [ring](../../../../../../ring.md) is semisimple: a free [module](../../../../../../module-mathematics.md) is a direct sum of simple summands of copies of the regular [module](../../../../../../module-mathematics.md), and a quotient of a semisimple [module](../../../../../../module-mathematics.md) is again semisimple, because the images of its simple summands are either zero or simple and span the quotient. A maximal independent family of these simple images spans: any simple image not contained in the sum intersects it trivially and could be added. Each factor is also [Artinian](../../../../../../artinian-ring.md), as a subquotient of $R_R$. A semisimple [Artinian module](../../../../../../artinian-module.md) has only finitely many simple summands, since an infinite direct sum would give a descending chain by successively deleting summands. Consequently every factor has finite [module length](../../../../../../length-of-a-module.md).

Concatenating composition series of these finitely many factors makes $R_R$ a [module](../../../../../../module-mathematics.md) of finite [module length](../../../../../../length-of-a-module.md). Such a [module](../../../../../../module-mathematics.md) satisfies both chain conditions, since every strict change consumes a positive amount of length. Therefore **$R$ is right Noetherian**. This is the [Hopkins-Levitzki theorem](../../../../../../hopkins-levitzki-theorem.md), obtained from the two preceding results rather than invoked in their proofs.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
