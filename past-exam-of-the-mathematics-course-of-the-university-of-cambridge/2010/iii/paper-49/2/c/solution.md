<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First expand the result of the first gate in the [computational basis](../../../../../../computational-basis.md):

$$
U(\alpha)|+\rangle
=\frac{|+\rangle+e^{-i\alpha}|-\rangle}{\sqrt2}
=\frac{1+e^{-i\alpha}}2|0\rangle+\frac{1-e^{-i\alpha}}2|1\rangle.
$$

Using $1+e^{-i\alpha}=2e^{-i\alpha/2}\cos(\alpha/2)$ and $1-e^{-i\alpha}=2ie^{-i\alpha/2}\sin(\alpha/2)$, this becomes

$$
e^{-i\alpha/2}\left(\cos(\alpha/2)|0\rangle+i\sin(\alpha/2)|1\rangle\right).
$$

Apply $U(\beta)|0\rangle=|+\rangle$ and $U(\beta)|1\rangle=e^{-i\beta}|-\rangle$ to obtain

$$
\boxed{U(\beta)U(\alpha)|+\rangle
=e^{-i\alpha/2}\left(\cos(\alpha/2)|+\rangle+i e^{-i\beta}\sin(\alpha/2)|-\rangle\right).}
$$

For example, its [quantum measurement in the computational basis](../../../../../../quantum-measurement-in-the-computational-basis.md) has probabilities $\mathbb P(k=0)=(1+\sin\alpha\sin\beta)/2$ and $\mathbb P(k=1)=(1-\sin\alpha\sin\beta)/2$, obtained by squaring the two basis amplitudes.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
