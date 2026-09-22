<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [local field](../../../../../../local-field.md) is nondiscrete and locally compact. In the non-Archimedean case its [valuation ring](../../../../../../valuation-ring.md) is compact by the scaling argument in part (b). Any [Cauchy sequence](../../../../../../cauchy-sequence.md) has a tail in a translate of a compact ball, so has a convergent subsequence; the Cauchy property forces the whole sequence to converge. Thus the [field](../../../../../../field.md) is complete. Part (b) gives a [discrete valuation](../../../../../../discrete-valuation.md), a [uniformizer](../../../../../../uniformizer.md) $\pi$, and a finite [residue field](../../../../../../residue-field.md) $k=\mathbb F_q$, $q=p^f$.

We construct the [coefficient](../../../../../../coefficient.md) [field](../../../../../../field.md) rather than presuming it exists. The [polynomial](../../../../../../polynomial-split.md) $T^q-T$ has derivative $-1$ in characteristic $p$. Every residue element therefore has a unique [polynomial root](../../../../../../root-of-a-polynomial.md) lift by [Hensel's lemma](../../../../../../hensel-s-lemma.md). The set $S$ of these $q$ lifts is a [field](../../../../../../field.md): qth powers preserve addition and multiplication, so sums and products remain [polynomial root](../../../../../../root-of-a-polynomial.md) lifts; a nonzero lift has inverse $a^{q-2}$. Reduction identifies $S$ with $\mathbb F_q$. This is the [finite coefficient field in positive-characteristic local fields](../../../../../../finite-coefficient-field-in-positive-characteristic-local-fields.md).

For $x\in\mathcal O_K$, choose $a_0\in S$ with the same residue, write $x=a_0+\pi x_1$, and repeat with $x_1\in\mathcal O_K$. Completeness gives

$$
x=\sum_{j\ge0}a_j\pi^j,\qquad a_j\in S.
$$

The first nonzero [coefficient](../../../../../../coefficient.md) determines the [valuation](../../../../../../valuation.md), so the expansion is unique. Multiplying an arbitrary [field](../../../../../../field.md) element by a suitable power of $\pi$ reduces it to this case. Consequently substitution $T\mapsto\pi$ gives a valued-field isomorphism

$$
\boxed{K\cong\mathbb F_{p^f}((T)),\qquad f\ge1.}
$$

Addition and multiplication agree with those of [Laurent series](../../../../../../laurent-series.md) by convergence, and a nonzero series has a nonzero leading [coefficient](../../../../../../coefficient.md), establishing injectivity as well as surjectivity.

Conversely, $\mathbb F_q((T))$ is complete for its T-adic [absolute value on a field](../../../../../../absolute-value-algebra.md). Its [valuation ring](../../../../../../valuation-ring.md) $\mathbb F_q[[T]]$ is compact: fixing finitely many [coefficients](../../../../../../coefficient.md) gives the finite partitions into balls, and the successive [coefficient](../../../../../../coefficient.md) choices realize the [inverse limit](../../../../../../inverse-limit.md) of the finite rings $\mathbb F_q[T]/(T^n)$. Equivalently it is the product of countably many finite discrete [coefficient](../../../../../../coefficient.md) sets. Thus it is a non-Archimedean [local field](../../../../../../local-field.md). Distinct $q$ give nonisomorphic valued [fields](../../../../../../field.md) because their [residue fields](../../../../../../residue-field.md) have different sizes. Replacing $|T|$ by any number in $(0,1)$ gives an equivalent [absolute value on a field](../../../../../../absolute-value-algebra.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
