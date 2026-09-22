<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Here the true [multiplicative order](../../../../../../multiplicative-order.md) is four, and it divides every power-of-two Fourier-register size $Q\geq4$, including the $Q=256$ choice from part (ii). A second-register measurement produces one of the four periodic cosets

$$
\sqrt{\frac4Q}\sum_{k=0}^{Q/4-1}|x_0+4k\rangle.
$$

Its [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) has nonzero amplitudes only at $j=0,Q/4,Q/2,3Q/4$, and each has squared modulus $1/4$. The inverse transform only changes phases or permutes these four labels. Hence the measured ratios $0,1/4,1/2,3/4$ are equally likely.

For $1/4$ or $3/4$, [continued-fraction recovery in quantum order finding](../../../../../../continued-fraction-recovery-in-quantum-order-finding.md) returns denominator four. Part (i) then gives factors three and five. For $1/2$, the reduced denominator is two. Although two is not a period, the [candidate-denominator gcd post-processing](../../../../../../candidate-denominator-gcd-post-processing.md) in part (ii) still gives a factor:

$$
z=7^{2/2}=7,\qquad\gcd(7-1,15)=3,\quad\gcd(7+1,15)=1.
$$

The zero outcome produces no useful even candidate and the run fails. **For the factor-extraction procedure specified above, three of the four outcomes succeed**:

$$
\boxed{\Pr(\text{nontrivial factor in one run})=\frac34.}
$$

There is an important convention behind this answer. A version that rejects a candidate unless $7^q\equiv1\pmod{15}$ before attempting any gcd rejects $q=2$, since $7^2\equiv4$. Under that validated-period convention only the two odd-numerator phases succeed, giving

$$
\boxed{\Pr(\text{one-run success with a prior period check})=\frac12.}
$$

Thus the probability of recovering the true [multiplicative order](../../../../../../multiplicative-order.md) is $1/2$, whereas the probability of finding a factor with direct gcd post-processing is $3/4$. The printed question does not specify this classical post-processing detail; stating it avoids identifying these two different events.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
