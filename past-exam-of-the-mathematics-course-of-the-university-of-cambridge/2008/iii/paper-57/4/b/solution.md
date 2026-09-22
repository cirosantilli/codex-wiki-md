<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $L=2^N$. Applying the inverse [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) to the register in part (a) gives [probability amplitude](../../../../../../probability-amplitude.md) at label $m$ equal to

$$
a_m=\frac1L\sum_{x=0}^{L-1}e^{ix\delta},\qquad\delta=\phi_j-\frac{2\pi m}{L}.
$$

Choose $m$ nearest to $\eta=L\phi_j/(2\pi)$, with $m$ reduced modulo $L$ at the phase boundary. Then the difference can be represented with $|\delta|\leq\pi/L$. For $\delta\ne0$, sum the [finite geometric series](../../../../../../finite-geometric-series.md) to obtain

$$
a_m=e^{i(L-1)\delta/2}\frac{\sin(L\delta/2)}{L\sin(\delta/2)}.
$$

Let $z=L|\delta|/2\leq\pi/2$. On $[0,\pi/2]$, [concavity](../../../../../../concave-function.md) of sine gives $\sin z\geq2z/\pi$, the line through its endpoint values. Also $|\sin(\delta/2)|\leq|\delta|/2$. Therefore

$$
|a_m|\geq\frac{(2/\pi)(L|\delta|/2)}{L|\delta|/2}=\frac2\pi,
$$

and the [Born rule](../../../../../../born-rule.md) proves the [nearest-integer success bound for quantum phase estimation](../../../../../../nearest-integer-success-bound-for-quantum-phase-estimation.md):

$$
\boxed{\Pr(m)=|a_m|^2\geq\frac4{\pi^2}.}
$$

If $\delta=0$, every summand is one and the [probability](../../../../../../probability.md) is exactly one. If the scaled phase is halfway between two integers, either nearest label separately satisfies the displayed bound. Interpreting the measured integer as $m/L$ gives the closest available $N$-bit phase estimate modulo one.

## ↑ Ancestors (11)

1. [B](../b.md)
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
