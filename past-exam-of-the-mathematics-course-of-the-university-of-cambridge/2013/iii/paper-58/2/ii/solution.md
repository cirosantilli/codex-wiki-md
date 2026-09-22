<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [amplitude amplification theorem](../../../../../../amplitude-amplification.md) concerns a known preparation [quantum circuit](../../../../../../quantum-circuit-split.md) $A$ and a good-subspace projector $\Pi$. Write $A|0\rangle=\sin\theta|g\rangle+\cos\theta|b\rangle$, with $\sin^2\theta=p=\|\Pi A|0\rangle\|^2$. Let $S_0=I-2|0\rangle\langle0|$ and $S_\chi=I-2\Pi$. Then

$$
Q=-A S_0A^\dagger S_\chi,\qquad\boxed{\|\Pi Q^jA|0\rangle\|^2=\sin^2((2j+1)\theta).}
$$

The [reflection operators](../../../../../../reflection-operator.md) preserve the two-dimensional good-bad plane and rotate it by $2\theta$, so $O(1/\sqrt p)$ iterations amplify a small known success probability to a constant close to one. Each iteration uses one good-subspace phase test and one use each of $A,A^\dagger$, together with a known reflection. **[Amplitude amplification](../../../../../../amplitude-amplification.md) provides a quadratic improvement in the number of repetitions of a successful preparation.** The query cost of the preparation and its inverse must be included when they themselves use the input oracle. [Exact amplitude amplification](../../../../../../exact-amplitude-amplification.md) uses additional known-overlap preparation or phase matching to avoid integer-iteration overshoot.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
