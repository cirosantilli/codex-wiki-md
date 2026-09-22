<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Suppose a [fixed-point combinator](../../../../../../fixed-point-combinator.md) $F$ were typable in the [simply typed lambda calculus](../../../../../../simply-typed-lambda-calculus.md). By the [Weak normalization theorem for simply typed lambda calculus](../../../../../../weak-normalization-theorem-for-simply-typed-lambda-calculus.md), it would have a [beta-normal form](../../../../../../beta-normal-form.md). For a fresh variable $f$, the term $Ff$ would then also possess a beta-normal form, say $N$.

The fixed-point property gives

$$
Ff\equiv_\beta f(Ff).
$$

Reducing the occurrence of $Ff$ on the right to $N$ gives the normal form $fN$. The [Church-Rosser theorem](../../../../../../church-rosser-theorem.md) says that these [beta-equivalent](../../../../../../beta-equivalence.md) terms must have [alpha-equivalent](../../../../../../alpha-equivalence.md) normal forms. This is impossible because $fN$ contains more symbols than $N$. Hence no typing context and simple type can type $F$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
