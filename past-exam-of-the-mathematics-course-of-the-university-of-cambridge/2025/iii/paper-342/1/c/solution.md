<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The block matrix is

$$
K=\begin{pmatrix}0&M\\M&0\end{pmatrix},
\qquad
K^{-1}=\begin{pmatrix}0&M^{-1}\\M^{-1}&0\end{pmatrix}.
$$

If both $q\in\mathcal L$ and $q'$ condense, choose their boundary excursions so that the two string operators cross once. Their commutator is their mutual full-braiding phase:

$$
W_qW_{q'}=exp(2\pi i q^TK^{-1}q')W_{q'}W_q.
$$

Both operators act as the identity on every ground state, so consistency requires

$$
q^TK^{-1}q'\in\mathbb Z
\qquad\hbox{for every }q=(q_1,q_2,0,0)^T\in\mathcal L.
$$

Writing $q'=(q'_{\rm top},q'_{\rm bot})$, this says

$$
M^{-1}q'_{\rm bot}\in\mathbb Z^2.
$$

Set $l_{\rm top}=M^{-1}q'_{\rm bot}$ and choose $l_{\rm bot}=0$. Then $Kl=(0,q'_{\rm bot})^T$, and

$$
u=q'-Kl=(q'_{\rm top},0)^T\in\mathcal L.
$$

Therefore every additionally condensable anyon has the form

$$
\boxed{q'=u+Kl,\qquad u\in\mathcal L,\quad l\in\mathbb Z^4.}
$$

The $Kl$ term is a local particle in the [anyon lattice of an Abelian Chern--Simons theory](../../../../../../anyon-lattice-of-an-abelian-chern-simons-theory.md), so the condensate is maximal modulo local excitations, as required for a [Lagrangian subgroup of Abelian anyons](../../../../../../lagrangian-subgroup-of-abelian-anyons.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
