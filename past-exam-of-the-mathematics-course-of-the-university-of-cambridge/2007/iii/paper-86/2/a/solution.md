<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Wirtinger derivatives](../../../../../../wirtinger-derivatives.md) $\partial_z=(\partial_x-i\partial_y)/2$ and $\partial_{\bar z}=(\partial_x+i\partial_y)/2$. In particular $q_{z\bar z}=\Delta q/4$. Let $E=e^{-ikz-\lambda\bar z/(ik)}$, $A=E(q_z+ikq)$ and $B=E(q_{\bar z}+\lambda q/(ik))$, so the printed [differential form](../../../../../../differential-form-split.md) is $W=A\,dz-B\,d\bar z$. Since $E_z=-ikE$ and $E_{\bar z}=-\lambda E/(ik)$,

$$
\begin{aligned}
A_{\bar z}&=E\left[q_{z\bar z}+ikq_{\bar z}-\frac\lambda{ik}q_z-\lambda q\right],\\
B_z&=E\left[q_{z\bar z}+\frac\lambda{ik}q_z-ikq_{\bar z}-\lambda q\right].
\end{aligned}
$$

Thus the [exterior derivative](../../../../../../exterior-derivative.md) is

$$
\boxed{dW=-2E(q_{z\bar z}-\lambda q)\,dz\wedge d\bar z.}
$$

Because $E$ never vanishes and $k\ne0$, this proves both directions: $W$ is a [closed differential form](../../../../../../closed-differential-form.md) if and only if $q_{z\bar z}=\lambda q$. The latter is the [modified Helmholtz equation](../../../../../../modified-helmholtz-equation.md) $\Delta q-4\lambda q=0$ for positive $\lambda$. The associated [global relations](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) on a bounded region $\Omega$ are, for every nonzero spectral parameter,

$$
\boxed{\int_{\partial\Omega}e^{-ikz-\lambda\bar z/(ik)}\left[(q_z+ikq)dz-(q_{\bar z}+\lambda q/(ik))d\bar z\right]=0.}
$$

The boundary orientation is positive, by [Stokes theorem](../../../../../../stokes-theorem.md). Each admissible spectral parameter gives a separate identity between the traces. Interchanging $z$ and $\bar z$ gives the dual family, equivalently the same family at $k\mapsto-\lambda/k$ with an overall minus sign. No assumption that $q$ is real is needed.

For later use with $\lambda>0$, as in the remaining parts, make the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) explicit in the first quadrant. Put

$$
a(k)=k-\frac\lambda k,\qquad b(k)=k+\frac\lambda k,\qquad E=e^{-iax+by}.
$$

Let $h_2(x)=q(x,0)$, $n_2(x)=q_y(x,0)$ and $h_1(y)=q(0,y)$, $n_1(y)=q_x(0,y)$. These normals are inward-coordinate derivatives. The bottom is traversed from zero to infinity and the left side from infinity to zero. Their oriented spectral integrals are

$$
\begin{aligned}
\rho_x(k)&=i\int_0^\infty e^{-ia(k)x}\left[b(k)h_2(x)-n_2(x)\right]dx,\\
\rho_y(k)&=\int_0^\infty e^{b(k)y}\left[a(k)h_1(y)-i n_1(y)\right]dy.
\end{aligned}
$$

Here $\rho_x$ is analytic for $\operatorname{Im}k<0$ and $\rho_y$ for $\operatorname{Re}k<0$, with suitable boundary limits. Indeed $\operatorname{Im}a=(r+\lambda/r)\sin\theta$ and $\operatorname{Re}b=(r+\lambda/r)\cos\theta$ for $k=re^{i\theta}$. On their common third quadrant, both exponential weights decay. Apply the finite-domain relation to expanding rectangles; sufficient decay of the solution and traces eliminates the distant edges. This derives

$$
\boxed{\rho_x(k)+\rho_y(k)=0,\qquad\pi<\arg k<3\pi/2.}
$$

The limiting relations on the negative real and negative imaginary axes will remove the unknown derivative traces.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 86](../../../paper-86-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
