<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $T$ is entanglement breaking, applying it to one half of $|\phi\rangle\langle\phi|$ immediately shows that its [Choi matrix](../../../../../../../choi-matrix.md) is separable.

Conversely suppose

$$
C_T=\sum_kq_k\sigma_k\otimes\tau_k
$$

is separable. The Choi reconstruction formula for the normalized convention is

$$
T(\rho)=d\,\operatorname{Tr}_2[C_T(I\otimes\rho^T)]
=\sum_k\operatorname{Tr}(M_k\rho)\sigma_k,
\qquad
M_k=dq_k\tau_k^T.
$$

The trace-preserving condition $\operatorname{Tr}_1C_T=I/d$ implies $\sum_kM_k=I$, so $\{M_k\}$ is a POVM. Part (i) now proves that $T$ is entanglement breaking. Thus

$$
\boxed{T\text{ is entanglement breaking}
\iff C_T\text{ is separable}}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 323](../../../../paper-323-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
