<h1 id="10d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The known circuit from part (b) lets us apply $U_{\mathcal I}$ without querying the faulty oracle. Their composition satisfies

$$
U_{\mathcal I}U_f|x\rangle|y\rangle
=
\begin{cases}
|x\rangle|y\rangle,&x\ne x_0,\\
|x\rangle|y\mathbin\oplus a\rangle,&x=x_0.
\end{cases}
$$

Because $a=00\cdots01$, only the last answer qubit is flipped in the exceptional case.

Prepare the answer register as

$$
|0\rangle^{\otimes(n-1)}|-\rangle,
\qquad
|-\rangle=\frac{|0\rangle-|1\rangle}{\sqrt2}.
$$

Since $X|-\rangle=-|-\rangle$, [quantum phase kickback](../../../../../../phase-kickback.md) gives, for an arbitrary search-register state,

$$
(U_{\mathcal I}U_f)
|x\rangle|0^{n-1}\rangle|-\rangle
=(-1)^{[x=x_0]}
|x\rangle|0^{n-1}\rangle|-\rangle.
$$

The answer register is unchanged and factors out. The induced operation on the first register is therefore

$$
\boxed{I_{x_0}=I-2|x_0\rangle\langle x_0|}.
$$

This is the [marked-state phase oracle from a single faulty identity-oracle query](../../../../../../marked-state-phase-oracle-from-a-single-faulty-identity-oracle-query.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10D](../../10d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
