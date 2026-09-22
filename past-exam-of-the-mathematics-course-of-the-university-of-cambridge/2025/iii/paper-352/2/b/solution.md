<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $g=\dot\gamma$ denote the constant rate in the [simple shear flow](../../../../../../simple-shear-flow.md)

$$
\mathbf u=(gy,0,0).
$$

Then

$$
\dot{\boldsymbol\gamma}
=\begin{pmatrix}0&g&0\\g&0&0\\0&0&0\end{pmatrix},
\qquad
\boldsymbol\Omega
=\frac12\begin{pmatrix}0&g&0\\-g&0&0\\0&0&0\end{pmatrix}.
$$

When $\xi=1$, the structure equation contains the [Jaumann derivative](../../../../../../jaumann-derivative.md). In a steady homogeneous flow it becomes

$$
-\boldsymbol\Omega\boldsymbol\alpha
+\boldsymbol\alpha\boldsymbol\Omega+c_1\boldsymbol\alpha
=c_2\dot{\boldsymbol\gamma}.
$$

Solving its component equations gives

$$
\alpha_{xy}=\frac{c_1c_2g}{c_1^2+g^2},
\qquad
\alpha_{xx}=-\alpha_{yy}
=\frac{c_2g^2}{c_1^2+g^2},
\qquad
\alpha_{zz}=0.
$$

The $b_2$ term has no $xy$ component because $\alpha_{xx}+\alpha_{yy}=0$. Thus

$$
\tau_{xy}=\eta_0g+b_1\alpha_{xy},
$$

and the shear viscosity is

$$
\boxed{
\eta(g)=\frac{\tau_{xy}}g
=\eta_0+\frac{b_1c_1c_2}{c_1^2+g^2}}.
$$

It exhibits [shear thinning](../../../../../../shear-thinning.md) whenever $b_1c_1c_2>0$: it decreases from $\eta_0+b_1c_2/c_1$ at zero shear rate to the solvent plateau $\eta_0$ at large shear rate. If the product vanishes, the viscosity is constant.

For the diagonal stresses,

$$
\dot{\boldsymbol\gamma}\boldsymbol\alpha+
\boldsymbol\alpha\dot{\boldsymbol\gamma}
-\frac23(\boldsymbol\alpha:\dot{\boldsymbol\gamma})\mathbf I
=\operatorname{diag}\left(\frac23g\alpha_{xy},
\frac23g\alpha_{xy},-\frac43g\alpha_{xy}\right).
$$

The two [normal-stress differences](../../../../../../normal-stress-difference.md) are therefore

$$
\boxed{
N_1=\tau_{xx}-\tau_{yy}
=\frac{2b_1c_2g^2}{c_1^2+g^2}},
$$



$$
\boxed{
N_2=\tau_{yy}-\tau_{zz}
=\frac{c_2g^2}{c_1^2+g^2}
\left(-b_1+2b_2c_1\right)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 352](../../../paper-352-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
