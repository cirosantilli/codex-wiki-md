<h1 id="4/a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**The normalized ray produces a secure key; the literal printed vector is not normalized.** The squared norm of the coefficients in the PDF is $8/9+1/81=73/81$. Thus the physical [pure state](../../../../../../../pure-state.md) on that ray has normalized coefficients $6\sqrt2/\sqrt{73}$ and $1/\sqrt{73}$. This is a genuine [entangled state](../../../../../../../entangled-state.md) with two nonzero [Schmidt coefficients](../../../../../../../schmidt-coefficient.md), and Eve is independent of it by [purity decouples a subsystem from its purification](../../../../../../../purity-decouples-a-subsystem-from-its-purification.md).

For an explicit way to obtain uniform key bits, Alice applies a two-outcome local [measurement in quantum mechanics](../../../../../../../quantum-measurement-split.md) with [Kraus operators](../../../../../../../kraus-operator.md)

$$
K_s=\begin{pmatrix}1/(6\sqrt2)&0\\0&1\end{pmatrix},\qquad K_f=\begin{pmatrix}\sqrt{71/72}&0\\0&0\end{pmatrix}.
$$

Their squared products sum to the identity. The successful unnormalized state is $(|00\rangle+|11\rangle)/\sqrt{73}$, so

$$
\boxed{p_s=2/73,\qquad p_f=71/73.}
$$

Alice announces only success or failure. Success leaves an exact [Bell pair](../../../../../../../bell-pair.md), yielding one uniform secret bit; failure leaves $|00\rangle$ and is discarded. With many copies the successful fraction is positive. Alternatively, direct [computational basis](../../../../../../../computational-basis.md) measurements give a shared biased bit with probabilities $72/73$ and $1/73$, from which [privacy amplification](../../../../../../../privacy-amplification.md) can extract uniform secret bits. The coefficient $1/9$ has not been silently replaced by $1/3$.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 53](../../../../paper-53-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
