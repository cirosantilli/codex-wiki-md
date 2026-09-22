<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $\phi=2\pi n/N+\epsilon$, with $|\epsilon|\le\delta\ll2\pi/N$. Decode the measured bits as above. The [probability amplitude](../../../../../../probability-amplitude.md) of label $m$ is

$$
a_m=\frac1N\sum_{k=0}^{N-1}e^{ik\Delta_m},\qquad \Delta_m=\phi-\frac{2\pi m}{N}.
$$

Using the [finite geometric series](../../../../../../finite-geometric-series.md),

$$
a_m=\frac{e^{i(N-1)\Delta_m/2}}N\frac{\sin(N\Delta_m/2)}{\sin(\Delta_m/2)},\qquad P(m)=\frac{\sin^2(N\Delta_m/2)}{N^2\sin^2(\Delta_m/2)}.
$$

Interpret removable singularities by continuity. In particular, [near-grid quantum phase estimation](../../../../../../near-grid-quantum-phase-estimation.md) returns the nearby exact label $n\bmod N$ with [probability](../../../../../../probability.md)

$$
\boxed{P(n)=\frac{\sin^2(N\epsilon/2)}{N^2\sin^2(\epsilon/2)}=1-\frac{N^2-1}{12}\epsilon^2+O(N^4\epsilon^4).}
$$

This is near one under the stated small-offset assumption, but not exactly one when $\epsilon\ne0$.

There is also a rigorous error bound. Taking the squared modulus of the sum gives

$$
1-P(n)=\frac1{N^2}\sum_{k,l=0}^{N-1}\bigl[1-\cos((k-l)\epsilon)\bigr]\le\frac{\epsilon^2}{2N^2}\sum_{k,l=0}^{N-1}(k-l)^2=\frac{N^2-1}{12}\epsilon^2,
$$

where $1-\cos x\le x^2/2$ and the elementary sums of $k$ and $k^2$ evaluate the last expression. Hence

$$
\boxed{P\!\left(\widehat\phi=\frac{2\pi(n\bmod N)}N\right)\ge1-\frac{N^2-1}{12}\delta^2.}
$$

On that event the circular [quantum phase](../../../../../../quantum-phase.md) error is at most $\delta$. For other labels, the exact [probabilities](../../../../../../probability.md) are

$$
P(m)=\frac{\sin^2(N\epsilon/2)}{N^2\sin^2\!\left(\epsilon/2+\pi(n-m)/N\right)},\qquad m\ne n\bmod N.
$$

Their total is $1-P(n)=O(N^2\delta^2)$, describing the leakage from the perfect solution. The physical output bit string remains reversed in the printed circuit; this changes its decoding, not these [probabilities](../../../../../../probability.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
