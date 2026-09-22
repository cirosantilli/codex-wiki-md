<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**For every nontrivial dimension $d\ge2$, no such [pure state](../../../../../pure-state.md) exists. The literal claim needs this qualification: for $d=1$, the only measurement outcome is necessarily the same for both parties.** The contradiction below requires allowing all complex [orthonormal bases](../../../../../orthonormal-basis.md), as quantum theory does.

If equal outcomes were certain in the [computational basis](../../../../../computational-basis.md), all amplitudes with different labels would vanish, so the normalized joint state would have the form

$$
|\Psi\rangle=\sum_{j=0}^{d-1}c_j|j\rangle|j\rangle.
$$

Choose distinct labels $j,k$ and replace their computational [vectors](../../../../../vector.md) in both local bases by $|+\rangle_{jk}=(|j\rangle+|k\rangle)/\sqrt2$ and $|-\rangle_{jk}=(|j\rangle-|k\rangle)/\sqrt2$, leaving all other [vectors](../../../../../vector.md) fixed. The joint amplitude for the _different_ outcomes $+,-$ is $(c_j-c_k)/2$. Certainty of equal outcomes would force $c_j=c_k$.

Now use the complex pair $|+i\rangle_{jk}=(|j\rangle+i|k\rangle)/\sqrt2$ and $|-i\rangle_{jk}=(|j\rangle-i|k\rangle)/\sqrt2$ in the same way on both systems. The amplitude for different outcomes $+i,-i$ is $(c_j+c_k)/2$, because the conjugated bra factors on the $|kk\rangle$ term multiply to $(-i)(i)=1$. Thus equal outcomes would also force $c_j=-c_k$. Combining the two requirements gives $c_j=c_k=0$. Every label belongs to such a pair when $d\ge2$, forcing the zero [vector](../../../../../vector.md) and contradicting [normalization](../../../../../normalization.md). This proves [impossibility of universal identical-basis perfect correlations](../../../../../impossibility-of-universal-identical-basis-perfect-correlations.md).

The maximally [entangled state](../../../../../entangled-state.md) $d^{-1/2}\sum_j|jj\rangle$ is not a counterexample: it correlates matching labels when one party uses a basis and the other its coordinatewise [complex conjugate](../../../../../complex-conjugate.md) basis. Requiring the two complex bases to be identical is different. This distinction also follows from [conjugate-state steering from a maximally entangled pair](../../../../../conjugate-state-steering-from-a-maximally-entangled-pair.md); restricting attention to real bases would miss the contradiction.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Quantum information](../../../quantum-information-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
