<h1 id="10d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [no-cloning theorem for two pure states](../../../../../../no-cloning-theorem-for-two-pure-states.md) states that, for distinct nonorthogonal states $|c_0\rangle$ and $|c_1\rangle$, there is no [unitary operator](../../../../../../unitary-operator.md) $U$ and fixed blank state $|0\rangle$ such that

$$
U\bigl(|c_j\rangle|0\rangle\bigr)
=|c_j\rangle|c_j\rangle,
\qquad j=0,1.
$$

To derive this from state discrimination, let

$$
s=|\langle c_0|c_1\rangle|,
\qquad 0<s<1,
$$

and suppose such a cloner existed. Applying it repeatedly would produce $N$ copies. The [inner product](../../../../../../inner-product.md) of the two possible $N$-copy states has magnitude $s^N$, so their optimal success probability under the [Helstrom-Holevo bound](../../../../../../helstrom-holevo-bound.md) would be

$$
P_N=\frac12\left(1+\sqrt{1-s^{2N}}\right).
$$

Already for $N=2$,

$$
P_2>P_1
=\frac12\left(1+\sqrt{1-s^2}\right),
$$

because $0<s<1$ implies $s^4<s^2$. But cloning followed by the two-copy [Helstrom measurement for two pure states](../../../../../../helstrom-measurement-for-two-pure-states.md) would itself be a quantum procedure applied to the original single state, contradicting the optimal one-copy bound $P_1$. Hence the assumed unitary cloner cannot exist.

Equivalently, [clone-assisted asymptotic state discrimination](../../../../../../clone-assisted-asymptotic-state-discrimination.md) would give $P_N\to1$, although two nonorthogonal states are not [perfectly distinguishable](../../../../../../perfect-distinguishability-of-pure-states.md). Thus the Helstrom--Holevo theorem implies the no-cloning theorem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10D](../../10d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
