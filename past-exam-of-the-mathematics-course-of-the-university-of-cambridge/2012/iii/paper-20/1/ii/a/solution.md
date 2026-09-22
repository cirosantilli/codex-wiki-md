<h1 id="1/ii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Poisson bracket](../../../../../../../poisson-bracket.md) in the original coordinates is

$$
\boxed{\{F,G\}_{q,p}=\sum_{j=1}^n(F_{q_j}G_{p_j}-F_{p_j}G_{q_j}).}
$$

For $z=(q,p)$, set

$$
J=\begin{pmatrix}0&I_n\\-I_n&0\end{pmatrix},\qquad A=Df(z).
$$

Then $\omega_0(u,v)=u^T Jv$ and $\{F,G\}=\nabla F^T J\nabla G$. The pullback definition of a [canonical transformation](../../../../../../../canonical-transformation.md) gives the pointwise [matrix](../../../../../../../matrix.md) condition

$$
\boxed{A^TJA=J.}
$$

Since $A$ is invertible, this is equivalent to $AJA^T=J$. Indeed, invert $A^TJA=J$ and use $J^{-1}=-J$ to obtain $A^{-1}JA^{-T}=J$, then multiply by $A$ and $A^T$. Applying the same calculation to the inverse implication gives equivalence. These are the two equivalent [symplectic matrix](../../../../../../../symplectic-matrix.md) identities that connect the [symplectic form](../../../../../../../symplectic-form.md) with [Poisson brackets](../../../../../../../poisson-bracket.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Ii](../../ii.md)
3. [1](../../../1.md)
4. [Paper 20](../../../../paper-20-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
