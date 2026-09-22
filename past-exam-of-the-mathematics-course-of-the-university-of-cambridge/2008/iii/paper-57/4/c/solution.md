<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose an [orthonormal](../../../../../../orthonormal-set.md) eigenbasis of $V$, with [eigenphases](../../../../../../eigenphase.md) $\phi_0,\phi_1$, counting multiplicity. The [maximally mixed state](../../../../../../maximally-mixed-state.md) is [basis](../../../../../../basis.md) independent, so

$$
\rho=\frac12|v_0\rangle\langle v_0|+\frac12|v_1\rangle\langle v_1|.
$$

[Linearity](../../../../../../linearity.md) means that the experiment is the equal mixture of the two [eigenstate](../../../../../../eigenstate.md) experiments. After the inverse [quantum Fourier transform](../../../../../../quantum-fourier-transform.md), the joint state is $\frac12\sum_{j=0}^1|\chi_j\rangle\langle\chi_j|\otimes|v_j\rangle\langle v_j|$, where $|\chi_j\rangle=\sum_m a_m(\phi_j)|m\rangle$ and

$$
a_m(\phi)=\frac1L\sum_{x=0}^{L-1}e^{ix(\phi-2\pi m/L)}.
$$

Thus the exact output distribution for [quantum phase estimation with a maximally mixed target](../../../../../../quantum-phase-estimation-with-a-maximally-mixed-target.md) is

$$
\boxed{\Pr(m)=\frac12|a_m(\phi_0)|^2+\frac12|a_m(\phi_1)|^2,\qquad m=0,\ldots,L-1.}
$$

For a nonzero phase mismatch, the squared [probability amplitude](../../../../../../probability-amplitude.md) is $\sin^2[L(\phi-2\pi m/L)/2]/\{L^2\sin^2[(\phi-2\pi m/L)/2]\}$, with value one at an exact match. If both [eigenphases](../../../../../../eigenphase.md) are exactly representable on the $L$-point grid, their two labels occur with [probability](../../../../../../probability.md) $1/2$ each; coincident labels have their [probabilities](../../../../../../probability.md) added. For general [eigenphases](../../../../../../eigenphase.md) there can be nonzero [probabilities](../../../../../../probability.md) at other labels, so it would not be exact to list only the two best approximations with [probability](../../../../../../probability.md) $1/2$ each. Each [eigenphase](../../../../../../eigenphase.md) is sampled with spectral weight $1/2$, and its nearest-label event has [conditional probability](../../../../../../conditional-probability.md) at least $4/\pi^2$. In particular a nearest label for one [eigenphase](../../../../../../eigenphase.md) has unconditional [probability](../../../../../../probability.md) at least $2/\pi^2$, with additional contributions possible from the other phase.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
