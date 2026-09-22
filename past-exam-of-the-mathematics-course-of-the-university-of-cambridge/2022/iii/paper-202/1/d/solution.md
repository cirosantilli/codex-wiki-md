<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\mathcal M_c^2$ be the continuous $L^2$-bounded martingales starting at zero, modulo indistinguishability, with norm $\|N\|_{\mathcal M^2}=\|N_\infty\|_2$. For a fixed $M\in\mathcal M_c^2$, define a finite measure on $\mathcal P$ by

$$
\nu_M(C)=\mathbb E\int_0^\infty\mathbf1_C(\omega,s)\,d[M]_s,
$$

and let $L^2(M)=L^2(\mathcal P,\nu_M)$. The [Itô isometry](../../../../../../ito-isometry.md) is the isometric extension

$$
I_M:L^2(M)\longrightarrow\mathcal M_c^2,
\qquad
H\longmapsto H\mathbin\cdot M,
$$

satisfying

$$
\mathbb E|(H\mathbin\cdot M)_\infty|^2
=\mathbb E\int_0^\infty H_s^2\,d[M]_s.
$$

For the simple process in part b, orthogonality gives the sum there. Conditional on $\mathcal F_{t_i}$, the martingale identity for $M^2-[M]$ gives

$$
\mathbb E\!\left[
H_i^2(M_{t_{i+1}}-M_{t_i})^2\right]
=\mathbb E\!\left[H_i^2([M]_{t_{i+1}}-[M]_{t_i})\right].
$$

Summing proves the isometry. Part c then supplies the unique extension to all of $L^2(M)$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
