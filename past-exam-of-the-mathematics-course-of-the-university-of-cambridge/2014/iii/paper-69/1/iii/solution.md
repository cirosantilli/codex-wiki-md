<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [dispersion symmetry elimination of a boundary trace](../../../../../../dispersion-symmetry-elimination-of-a-boundary-trace.md) uses the symmetry of the [dispersion relation](../../../../../../dispersion-relation.md)

$$
\nu(k)=i\alpha-k,\qquad \omega(\nu(k))=\omega(k).
$$

For $k\in\overline{D^+}$, $\operatorname{Im}\nu(k)\leq0$, so the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) is valid at $\nu(k)$. Since $i\nu+\alpha=-ik$, it gives

$$
G_1(k,t)=\widehat u_0(\nu)-e^{\omega t}\widehat u(\nu,t)+ikG_0(k,t).
$$

Substitution into the [contour integral](../../../../../../contour-integral.md) representation produces an unwanted integral $\int_{\partial D^+}e^{ikx}\widehat u(\nu(k),t)\,dk$. Its integrand is analytic in $D^+$ and decays on closing the contour upwards; [Jordan lemma](../../../../../../jordan-s-lemma.md) makes this integral zero for $x>0$. Hence the [Fokas method](../../../../../../fokas-method.md) eliminates the unknown [normal derivative](../../../../../../normal-derivative.md):

$$
\boxed{\begin{aligned}
u(x,t)&=\frac1{2\pi}\int_{\mathbb R}e^{ikx-\omega(k)t}\widehat u_0(k)\,dk\\
&\quad-\frac1{2\pi}\int_{\partial D^+}e^{ikx-\omega(k)t}
\left[\widehat u_0(i\alpha-k)+(2ik+\alpha)G_0(k,t)\right]\,dk.
\end{aligned}}
$$

All quantities here are determined by the prescribed initial and [Dirichlet boundary data](../../../../../../dirichlet-boundary-data.md) up to time $t$.

For verification and for numerical evaluation it is useful to evaluate the spectral [contour integrals](../../../../../../contour-integral.md), giving a [half-line drift reflection kernel](../../../../../../half-line-drift-reflection-kernel.md). Put

$$
H(r,t)=\frac{e^{-r^2/(4t)}}{\sqrt{4\pi t}},\qquad
K_\alpha(x,y,t)=H(x-y+\alpha t,t)-e^{\alpha y}H(x+y+\alpha t,t),
$$

and define the [half-line drift boundary kernel](../../../../../../half-line-drift-boundary-kernel.md)

$$
P_\alpha(x,t)=\frac{x}{2\sqrt\pi\,t^{3/2}}
\exp\left[-\frac{(x+\alpha t)^2}{4t}\right].
$$

[Fubini's theorem](../../../../../../fubini-s-theorem.md), the [Gaussian Fourier transform](../../../../../../fourier-transform-of-a-gaussian.md) and [contour deformation](../../../../../../contour-deformation.md) give the equivalent causal formula

$$
\boxed{u(x,t)=\int_0^\infty K_\alpha(x,y,t)u_0(y)\,dy
+\int_0^t P_\alpha(x,t-s)g_0(s)\,ds.}
$$

For the reflected initial term, $\widehat u_0(i\alpha-k)=\int_0^\infty e^{\alpha y+iky}u_0(y)\,dy$ on the contour; the evaluated Gaussian supplies the necessary large-$y$ decay. If $e^{\alpha y}u_0(y)$ is not integrable, truncate the [initial conditions](../../../../../../initial-condition.md) first, evaluate, and pass to the limit using Gaussian bounds. No extra exponential-decay assumption on the original data is needed for this kernel formula.

The boundary kernel follows particularly simply from

$$
-\frac1{2\pi}\int_{\partial D^+}(2ik+\alpha)e^{ikx-\omega(k)t}\,dk
=-(2\partial_x+\alpha)H(x+\alpha t,t)
=\frac{x}{t}H(x+\alpha t,t).
$$

This calculation independently checks both the sign and the coefficient of the boundary forcing.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
