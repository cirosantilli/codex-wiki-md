<h1 id="15d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Alice adjoins $|0\rangle_{A'}$ and applies a local unitary whose action on the relevant inputs is

$$
|0\rangle|0\rangle\mapsto
\frac st|0\rangle|0\rangle+sqrt{1-\frac{s^2}{t^2}}|1\rangle|0\rangle,
\qquad
|0\rangle|1\rangle\mapsto|0\rangle|1\rangle.
$$

Measuring $A'$ and obtaining zero leaves the unnormalized state

$$
s(|00\rangle+|11\rangle),
$$

so the normalized state is the [Bell state](../../../../../../bell-state-split.md) $|\phi^+\rangle$. The success probability is $2s^2>0$.

Applying this [entanglement concentration](../../../../../../entanglement-concentration.md) independently to $n$ pairs yields an expected $2s^2n$ Bell pairs. Alice and Bob measure successful pairs in the computational basis to obtain identical secret random bits; public communication identifies successful positions without revealing outcomes. These bits form a secret key for a one-time pad of expected length $2s^2n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15D](../../15d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
