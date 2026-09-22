<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $k_0$ be the unique [discrete logarithm](../../../../../../../discrete-logarithm-problem.md) of the measured value $c_0$, so that $c_0=g^{k_0}$. The [fiber](../../../../../../../fiber-of-a-function.md) calculation gives exactly the pairs $(yb+k_0,b)$ with $b\in\mathbb Z_M$, where $M=p-1$. The initial amplitude of each pair is $1/M$, so the [Born rule](../../../../../../../born-rule.md) assigns probability $M/M^2=1/M$ to this outcome.

After [projective measurement](../../../../../../../projective-measurement.md) and normalization, the first two [quantum registers](../../../../../../../quantum-register.md) are in the [coset state](../../../../../../../coset-state.md)

$$
\boxed{|C_{k_0}\rangle=\frac1{\sqrt M}\sum_{b=0}^{M-1}|yb+k_0\bmod M\rangle|b\rangle.}
$$

The measured third [quantum register](../../../../../../../quantum-register.md) factors as $|c_0\rangle$ and may be omitted. There is no loss of coherence between the $M$ terms in this [post-measurement state](../../../../../../../post-measurement-state.md): the [measurement in quantum mechanics](../../../../../../../quantum-measurement-split.md) reveals the common function value, not an individual input pair.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
