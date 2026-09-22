<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let

$$
l=\frac\pi L,
\qquad
\Theta(z)=1-\mathcal H(z-H),
$$

where $\mathcal H$ is the [Heaviside step function](../../../../../../heaviside-step-function.md). Then

$$
\nabla\mathbin\cdot\overline{\mathbf F}
=-F_0\delta(z-H)\sin^2(ly),
$$

so the [Eliassen equation for residual circulation](../../../../../../eliassen-equation-for-residual-circulation.md) is

$$
f_0^2\overline\chi_{a,zz}^*
+N^2\overline\chi_{a,yy}^*
=f_0F_0\delta'(z-H)\sin^2(ly).
$$

Take no normal residual flow at $y=0,L$ and $z=0$, decay as $z\to\infty$, and choose the streamfunction constant on the connected rigid boundary to be zero. Thus

$$
\overline\chi_a^*=0
\quad\text{on }y=0,L\text{ and }z=0,
\qquad
\overline\chi_a^*\to0
\quad(z\to\infty).
$$

The required [Fourier series](../../../../../../fourier-series-split.md) in sine modes is

$$
\sin^2\frac{\pi y}{L}
=\sum_{\substack{n\geq1\\n\text{ odd}}}
b_n\sin\frac{n\pi y}{L},
\qquad
\boxed{
b_n=\frac8{\pi n(4-n^2)}}.
$$

Define

$$
\lambda_n=\frac{Nn\pi}{|f_0|L},
\qquad
C_n=\frac{F_0b_n}{f_0}.
$$

For each mode, the vertical equation is

$$
\chi_n''-\lambda_n^2\chi_n
=C_n\delta'(z-H).
$$

The [Dirac delta function](../../../../../../dirac-delta-function.md) requires

$$
[\chi_n]_{H^-}^{H^+}=C_n,
\qquad
[\chi_n']_{H^-}^{H^+}=0.
$$

The solution satisfying the boundary conditions is therefore

$$
\boxed{
\overline\chi_a^*(y,z)
=\frac{F_0}{f_0}
\sum_{\substack{n\geq1\\n\text{ odd}}}
b_nS_n(z)\sin\frac{n\pi y}{L}},
$$

where

$$
\boxed{
S_n(z)=
\begin{cases}
-e^{-\lambda_nH}\sinh(\lambda_nz),&0<z<H,\\
\cosh(\lambda_nH)e^{-\lambda_nz},&z>H.
\end{cases}}
$$

The momentum equation gives

$$
\overline u_t
=f_0\overline\chi_{a,z}^*
-F_0\delta(z-H)\sin^2\frac{\pi y}{L}.
$$

The jump of $\overline\chi_a^*$ supplies an equal positive delta function in $f_0\overline\chi_{a,z}^*$, so the singular terms cancel. The regular acceleration is

$$
\boxed{
\overline u_t
=-F_0
\sum_{\substack{n\geq1\\n\text{ odd}}}
b_n\lambda_nR_n(z)
\sin\frac{n\pi y}{L}},
$$

where

$$
R_n(z)=
\begin{cases}
e^{-\lambda_nH}\cosh(\lambda_nz),&0<z<H,\\
\cosh(\lambda_nH)e^{-\lambda_nz},&z>H.
\end{cases}
$$

Finally, the transformed density equation gives

$$
\boxed{
\overline\rho_t
=\frac{d\rho_s}{dz}
\overline\chi_{a,y}^*
=\frac{d\rho_s}{dz}
\frac{F_0}{f_0}
\sum_{\substack{n\geq1\\n\text{ odd}}}
b_n\frac{n\pi}{L}S_n(z)
\cos\frac{n\pi y}{L}}.
$$

These exponentially decaying modes are the balanced mean response to [wave-activity deposition](../../../../../../wave-activity-deposition.md) at $z=H$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
