<h1 id="1/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Prepare the uniform [pure state](../../../../../../pure-state.md)

$$
|s\rangle=\frac1{\sqrt d}\sum_{j=0}^{d-1}|j\rangle.
$$

Every [permutation matrix](../../../../../../permutation-matrix.md) fixes this [vector](../../../../../../vector.md), so `RandomPermute` returns $|s\rangle$ with certainty. Choose an [orthonormal basis](../../../../../../orthonormal-basis.md) with first [vector](../../../../../../vector.md) $|\psi_0\rangle=|s\rangle$, for example the [quantum Fourier transform](../../../../../../quantum-fourier-transform-split.md) basis. Under `RandomReset`, the returned state is $I/d$, which gives each of the $d$ measurement labels [probability](../../../../../../probability.md) $1/d$.

Guess `RandomPermute` on label 0 and `RandomReset` on every other label. Then

$$
\boxed{P_{\rm success}=\frac12\cdot1+\frac12\cdot\frac{d-1}{d}=1-\frac1{2d}.}
$$

This is [invariant-pure-state discrimination against a maximally mixed reset](../../../../../../invariant-pure-state-discrimination-against-a-maximally-mixed-reset.md). It also agrees with the [Holevo–Helstrom theorem](../../../../../../holevo-helstrom-theorem.md): the [eigenvalues](../../../../../../eigenvalue.md) of $|s\rangle\langle s|-I/d$ are $1-1/d$ once and $-1/d$ with [multiplicity](../../../../../../multiplicity-mathematics.md) $d-1$, giving optimal equal-prior success $1/2+\|\rho_P-\rho_R\|_1/4=1-1/(2d)$. This confirms optimal discrimination of these returned states, in addition to constructing the requested strategy.[§3.1.1, Theorem 3.4 and equation (3.20), optimal binary-state discrimination](../../../../../../the-theory-of-quantum-information-by-john-watrous.md) For $d=1$, the actions coincide and the formula correctly gives random-guessing success $1/2$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
