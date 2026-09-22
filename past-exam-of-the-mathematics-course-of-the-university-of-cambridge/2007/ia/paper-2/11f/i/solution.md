<h1 id="11f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The statement is true.** Put $C_k=\bigcap_{r=1}^k A_r$. The assumed $P(C_{n-1})>0$ ensures that every conditioning event $C_{k-1}$, $2\leq k\leq n$, has positive probability. By the definition of [conditional probability](../../../../../../conditional-probability.md),

$$
P(A_k\mid C_{k-1})=\frac{P(C_k)}{P(C_{k-1})}.
$$

Multiplying makes the fractions telescope, giving

$$
\prod_{k=2}^nP(A_k\mid C_{k-1})=\frac{P(C_n)}{P(A_1)}
=P\left(\bigcap_{k=2}^n A_k\mid A_1\right).
$$

This proves the [chain rule for probabilities](../../../../../../chain-rule-for-probabilities.md) here without any assumption of [independence](../../../../../../independent-random-variables.md). The final numerator $P(C_n)$ may be zero; all denominators remain positive.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
