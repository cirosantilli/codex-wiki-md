<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

For a [finite group](../../../../../finite-group.md), the [conjugacy classes](../../../../../conjugacy-class.md) partition the [group](../../../../../group-split.md), and a class is a singleton exactly when its element belongs to the [centre of a group](../../../../../center-of-a-group.md). Since the centre is trivial, the [class equation](../../../../../class-equation.md) becomes

$$
|G|=1+\sum_j |\mathcal C_j|,
$$

where the $\mathcal C_j$ are all the nonidentity [conjugacy classes](../../../../../conjugacy-class.md). If the [prime number](../../../../../prime-number.md) $p$ divided every $|\mathcal C_j|$, reduction modulo $p$ would give $0=1$, because $p\mid |G|$. Therefore at least one of these class sizes is not divisible by $p$. Primality now gives

$$
\boxed{\gcd(|\mathcal C_j|,p)=1.}
$$

Its size is greater than one because the centre is trivial. This proves the [prime-to-p conjugacy class lemma](../../../../../prime-to-p-conjugacy-class-lemma.md).

**The conclusion requires $p$ to be prime.** The printed question does not explicitly impose this hypothesis. If arbitrary composite divisors are allowed, take the [symmetric group](../../../../../symmetric-group.md) $S_3$ and $p=6$: its centre is trivial, its two nonidentity [conjugacy classes](../../../../../conjugacy-class.md) have sizes $3$ and $2$, and neither is [coprime](../../../../../coprime-integers.md) to $6$. Thus the argument proves the intended prime case and also identifies why the unrestricted literal reading is false.

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
