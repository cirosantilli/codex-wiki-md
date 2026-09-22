<h1 id="6c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [modular congruence](../../../../../../modular-congruence.md) $x^4\equiv1$ first implies $x\not\equiv0$. Multiplication by such an $x$ permutes the nonzero [residue classes](../../../../../../residue-class.md) modulo the prime $p$: if $xa\equiv xb$, cancellation gives $a\equiv b$. Multiply all these residues and cancel their nonzero product to obtain $x^{p-1}\equiv1$, the usual short proof of [Fermat little theorem](../../../../../../fermat-little-theorem.md).

Now $(x^2-1)(x^2+1)\equiv0$. By the [Euclid lemma](../../../../../../euclid-lemma.md), either $x^2\equiv1$ or $x^2\equiv-1$. In the latter case, because $p-1=4k+2$,

$$
x^{p-1}=(x^2)^{2k+1}\equiv(-1)^{2k+1}=-1\pmod p,
$$

contradicting the preceding product argument, since $p$ is odd. Thus

$$
\boxed{x^2\equiv1\pmod p}.
$$

No unproved assertion about the number of fourth roots is needed.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6C](../../6c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
