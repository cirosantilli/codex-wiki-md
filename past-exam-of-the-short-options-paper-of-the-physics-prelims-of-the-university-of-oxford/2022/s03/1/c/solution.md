<h1 id="s03/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the stated ordered propagation basis, a downward input is transmitted downward and reflected upward, giving the first column $(1,1)^T/\sqrt2$. An upward input is reflected downward with the opposite reflection phase and transmitted upward, giving the second column $(-1,1)^T/\sqrt2$. Therefore

$$
\boxed{B=\frac{1}{\sqrt2}\begin{pmatrix}1&-1\\1&1\end{pmatrix}.}
$$

Equal [mirror](../../../../../mirror.md) reflection phases exchange the two directions. Choosing a phase of $\pi$ per reflection gives

$$
\boxed{M=-\begin{pmatrix}0&1\\1&0\end{pmatrix}.}
$$

Each path encounters one [mirror](../../../../../mirror.md), so $M$ describes both arms together, not two successive reflections of each [photon](../../../../../photon.md). Changing its common phase leaves all detection [probabilities](../../../../../probability.md) unchanged. Direct multiplication gives $B^\dagger B=M^\dagger M=I$, so both are [unitary matrices](../../../../../unitary-matrix.md). They preserve the norm of a [quantum state](../../../../../quantum-state.md) and hence total [probability](../../../../../probability.md) for these lossless optical elements.

Ideal detectors are represented by measurement matrices, but detection itself is not unitary evolution within the two traveling modes. With $e_1=(1,0)^T$ and $e_2=(0,1)^T$, the [projective measurement](../../../../../projective-measurement.md) operators are

$$
\boxed{P_2=e_1e_1^\dagger=\begin{pmatrix}1&0\\0&0\end{pmatrix},\qquad
P_1=e_2e_2^\dagger=\begin{pmatrix}0&0\\0&1\end{pmatrix}.}
$$

They give [Born rule](../../../../../born-rule.md) [probabilities](../../../../../probability.md) $\langle\psi|P_j|\psi\rangle$ and sum to $I$. An absorbing detector maps the incident [photon](../../../../../photon.md) to an excited detector and vacuum field; a complete physical description includes those additional degrees of freedom.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [S03](../../../s03.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../../split.md)
6. [Short options paper of the physics Prelims of the University of Oxford](../../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
