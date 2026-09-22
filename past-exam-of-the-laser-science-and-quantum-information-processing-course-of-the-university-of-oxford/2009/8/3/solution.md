<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Eve's [computational-basis intercept-resend attack](../../../../computational-basis-intercept-resend-attack.md) applies a [projective measurement](../../../../projective-measurement.md) of $Z$ to Bob's photon and discards her outcome from Alice and Bob's description. Their resulting [density matrix](../../../../density-matrix-split.md) is

$$
\rho_{AB}^{\rm Eve}=\frac12|01\rangle\langle01|+\frac12|10\rangle\langle10|.
$$

This [separable state](../../../../separable-quantum-state.md) keeps $\langle Z\otimes Z\rangle=-1$ but removes $\langle X\otimes X\rangle$. Hence

$$
E_{\rm Eve}(\alpha,\beta)=-\cos2\alpha\cos2\beta,
\qquad
(E_{ij}^{\rm Eve})=\begin{pmatrix}
-1&-1/\sqrt2&-1/\sqrt2\\
0&0&0\\
-1/\sqrt2&-1/2&-1/2
\end{pmatrix}.
$$

Using the same signed Bell-test statistic gives

$$
\boxed{S_{\rm Eve}=\sqrt2,\qquad S_{\rm ideal}=2\sqrt2.}
$$

The ideal value is halved, and the attack no longer violates the [CHSH inequality](../../../../chsh-inequality.md).

The key data show why several settings matter. For $(1,1)$, Eve's measurement leaves perfect anticorrelation, so this subset has **zero bit errors** after Bob flips his assignment. For $(3,2)$, $E=-1/2$, so correct anticorrelation has probability $(1-E)/2=3/4$: its [quantum bit error rate](../../../../quantum-bit-error-rate.md) is **$1/4$**. If both key-setting pairs occur equally often, their combined raw-key error rate is **$1/8$**. The Bell-test change detects this attack even though the vertical/horizontal key subset alone would not.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [8](../../8-split.md)
3. [2009](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
