<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Galerkin method](../../../../../../galerkin-method.md): substitute the retained trigonometric modes and project onto them with the $L^2$ [inner product](../../../../../../inner-product.md) over the rectangle. Each mode satisfies the printed [boundary conditions](../../../../../../boundary-condition.md). Write $X=\alpha x$, $Z=\pi z$, and abbreviate the four mode prefactors by $C=2\sqrt2\beta/\alpha$, $D=2\sqrt2/\beta$, $V_1=2\sqrt2\sigma\pi R_\Omega/(\alpha\beta)$ and $V_2=\sigma R_\Omega/\alpha$. The [Jacobian determinant](../../../../../../jacobian-determinant.md) in the advection terms is $J(f,g)=f_xg_z-f_zg_x$.

The [stream function](../../../../../../stream-function.md) is a single [Laplacian eigenfunction](../../../../../../laplacian-eigenfunction.md), so $\nabla^2\psi=-\beta^2\psi$ and $J(\psi,\nabla^2\psi)=0$ exactly. For the temperature modes, direct multiplication gives

$$
\begin{aligned}
J(\psi,Db\cos X\sin Z)&=4\pi ab\sin2Z,\\
\operatorname{proj}J(\psi,-c\sin2Z/\pi)&=2\sqrt2\beta ac\cos X\sin Z.
\end{aligned}
$$

For the transverse-velocity modes, the retained products are

$$
\begin{aligned}
J(\psi,V_1d\sin X\cos Z)&=-\frac{4\sigma\pi^2R_\Omega}{\alpha}ad\sin2X,\\
\operatorname{proj}J(\psi,V_2e\sin2X)&=\beta^2V_1ae\sin X\cos Z.
\end{aligned}
$$

For example, $\sin Z\cos2Z=(\sin3Z-\sin Z)/2$ and $\sin X\cos2X=(\sin3X-\sin X)/2$ supply the signs of the two retained $ac$ and $ae$ couplings. The third harmonics are orthogonal to the retained modes and are discarded by this [Galerkin method](../../../../../../galerkin-method.md); they are not claimed to vanish in the full [partial differential equations](../../../../../../partial-differential-equation-split.md).

Before changing time, the five coefficient equations are

$$
\begin{aligned}
\frac{da}{dt}&=-\sigma\beta^2a+\frac{\sigma R\alpha^2}{\beta^4}b-\frac{\sigma^2\pi^2R_\Omega^2}{\beta^4}d,\\
\frac{db}{dt}&=\beta^2(a-b-ac),\\
\frac{dc}{dt}&=4\pi^2(-c+ab),\\
\frac{dd}{dt}&=\beta^2(a-\sigma d-ae),\\
\frac{de}{dt}&=-4\sigma\alpha^2e+4\pi^2ad.
\end{aligned}
$$

Dividing by $\beta^2$ gives the stated [five-mode rotating-convection truncation](../../../../../../five-mode-rotating-convection-truncation.md), with

$$
\boxed{r=\frac{\alpha^2}{\beta^6}R,\qquad r_\Omega=\frac{\pi}{\beta^3}R_\Omega,\qquad h=\varpi=\frac{4\pi^2}{\beta^2}.}
$$

The squared rotation parameter is $q=r_\Omega^2\ge0$. The printed $R_\Omega$ is proportional to rotation rate, so it is a square-root-type rotation parameter rather than the more usual [Taylor number](../../../../../../taylor-number.md) proportional to squared rotation rate; the algebra uses the coefficient as printed. At zero rotation the physical transverse velocity modes vanish; the normalized $d,e$ equations can still be understood through their continuous zero-rotation limit.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
