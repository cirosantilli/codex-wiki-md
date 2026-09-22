<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To first order about the fixed point,

$$
\boxed{u_t=D_nu_{xx}-\chi n_*v_{xx}-\delta u},
\qquad
\boxed{v_t=D_cv_{xx}+\alpha u-\beta v}.
$$

For a mode proportional to $e^{\sigma t+ikx}$, the linear matrix is

$$
M(k)=\begin{pmatrix}
-\delta-D_nk^2&\chi n_*k^2\\
\alpha&-\beta-D_ck^2
\end{pmatrix}.
$$

Its trace is always negative, so instability occurs exactly when its determinant is negative. Writing $q=k^2$,

$$
\det M=D_nD_cq^2+
\left(\delta D_c+\beta D_n-\frac{\alpha\chi\gamma}{\delta}\right)q
+\delta\beta.
$$

At onset this quadratic touches zero, requiring

$$
\boxed{\chi_c=\frac\delta{\alpha\gamma}
\left(\sqrt{\delta D_c}+\sqrt{\beta D_n}\right)^2}.
$$

The repeated positive root is

$$
q_c=\sqrt{\frac{\delta\beta}{D_nD_c}},
$$

and therefore

$$
\boxed{k_c=\left(\frac{\delta\beta}{D_nD_c}\right)^{1/4}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 355](../../../paper-355-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
