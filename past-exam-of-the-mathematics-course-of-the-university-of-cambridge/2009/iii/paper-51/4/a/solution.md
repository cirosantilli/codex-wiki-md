<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For nonnegative integers $n$, assume the storage channel over successive intervals of length $\tau$ composes as $D_\epsilon^n$. This is the memoryless interpretation of the specified storage law. In the [computational basis](../../../../../../computational-basis.md), write the [density operator](../../../../../../density-matrix.md) as

$$
\rho=\begin{pmatrix}u&z\\\overline z&1-u\end{pmatrix}.
$$

Conjugation by the [Pauli Z gate](../../../../../../pauli-z-gate.md) reverses the off-diagonal entries and leaves the diagonal entries unchanged, so

$$
D_\epsilon(\rho)=\begin{pmatrix}u&(1-2\epsilon)z\\(1-2\epsilon)\overline z&1-u\end{pmatrix}.
$$

After $n$ applications of the [phase-flip channel](../../../../../../phase-flip-channel.md), the multiplier is $(1-2\epsilon)^n$. Comparing with the multiplier $1-2\epsilon_n$ of a single [phase-flip channel](../../../../../../phase-flip-channel.md) gives

$$
\boxed{D_\epsilon^n=D_{\epsilon_n},\qquad\epsilon_n=\frac{1-(1-2\epsilon)^n}{2}.}
$$

For $n=0$ this gives the identity channel. Equivalently, composing two consecutive phase errors cancels them because $Z^2=I$, so their effective probability obeys $\epsilon_{n+1}=\epsilon+(1-2\epsilon)\epsilon_n$. The same expression solves this recurrence. The [iterated phase-flip channel](../../../../../../iterated-phase-flip-channel.md) formula presumes this composition law; specifying a channel at one time alone would not constrain a memory-bearing environment at later times.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
