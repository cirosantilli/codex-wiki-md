<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Besides the [Gaussian fixed point](../../../../../../gaussian-fixed-point.md), solve the nonzero-coupling fixed-point equations. The quartic equation gives $\lambda_*=2\epsilon(1+\rho_*)^2/(3K_D)$. Substitute into the mass equation to get $2\rho_*+\epsilon(1+\rho_*)/3=0$, hence $\rho_*=-\epsilon/(6+\epsilon)$ within the displayed one-loop truncation. Since $K_4=2\pi^2/(2\pi)^4=1/(8\pi^2)$,

$$
\boxed{\rho_*=-\epsilon/6+O(\epsilon^2),\qquad
\lambda_*=16\pi^2\epsilon/3+O(\epsilon^2).}
$$

These are the [Wilson-Fisher fixed point](../../../../../../wilson-fisher-fixed-point.md) coordinates in this cutoff scheme. The higher terms obtained by solving the truncated equations exactly should not be regarded as a full higher-order epsilon calculation.

The attraction claim in the PDF needs a thermal qualification. The [stability matrix of a renormalization-group fixed point](../../../../../../stability-matrix-of-a-renormalization-group-fixed-point.md) at this solution has entries

$$
J=\begin{pmatrix}
2-\epsilon/3&K_D/[2(1+\rho_*)]\\
3K_D\lambda_*^2/(1+\rho_*)^3&-\epsilon
\end{pmatrix}.
$$

The lower-left entry is $O(\epsilon^2)$, so its [eigenvalues](../../../../../../eigenvalue.md) are

$$
\boxed{y_t=2-\epsilon/3+O(\epsilon^2)>0,\qquad
y_g=-\epsilon+O(\epsilon^2)<0.}
$$

Increasing $\ell$ means approaching the infrared. The quartic scaling direction is attractive, but a perturbation in the thermal scaling direction grows as $e^{y_t\ell}$. Therefore the [Wilson-Fisher fixed point](../../../../../../wilson-fisher-fixed-point.md) is an infrared attractor **on its tuned [critical surface](../../../../../../critical-surface.md)**, not an attractive fixed point of the entire two-dimensional coupling plane. In the plane it is a saddle; an arbitrary small thermal perturbation is a concrete counterexample to unconditional attraction. This is the [thermal relevant direction at the Wilson-Fisher fixed point](../../../../../../thermal-relevant-direction-at-the-wilson-fisher-fixed-point.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
