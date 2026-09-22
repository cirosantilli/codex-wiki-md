<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $G_0(k),G_l(k)$ denote the [Half-range Fourier transforms](../../../../../../half-range-fourier-transform.md) of $g_0,g_l$, and let $N_0(k),N_l(k)$ denote those of the upward [derivatives](../../../../../../derivative.md) $n_0,n_l$. Also set

$$
H(k)=\int_0^le^{ky}h(y)\,dy,\qquad
W(k)=\int_0^le^{ky}v(y)\,dy.
$$

Integrate the tangential [derivatives](../../../../../../derivative.md) in the three spectral [functions](../../../../../../function-split.md) by parts. For example, $\int_0^\infty e^{-ikx}g_0'=-h(0)+ikG_0$, and $\int_0^le^{ky}h'=e^{kl}h(l)-h(0)-kH$. All corner values cancel in $\rho_L+\rho_B+\rho_T=0$. The result is the [semistrip Laplace spectral global relation](../../../../../../semistrip-laplace-spectral-global-relation.md)

$$
e^{kl}N_l(k)-N_0(k)+k[G_0(k)-e^{kl}G_l(k)]-W(k)-ikH(k)=0.
$$

For $\kappa>0$, use the [sine transforms](../../../../../../fourier-sine-transform.md)

$$
G_j^s(\kappa)=\int_0^\infty\sin(\kappa x)g_j(x)\,dx,\qquad
S_j(\kappa)=\int_0^\infty\sin(\kappa x)n_j(x)\,dx.
$$

Reality of $q$ makes $W(\kappa)$ and $W(-\kappa)$ real, so taking imaginary parts removes the unknown left-side [normal derivative](../../../../../../normal-derivative.md). At $k=\kappa$ and $k=-\kappa$ the two consequences of the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) are

$$
\begin{aligned}
e^{\kappa l}S_l-S_0
&=\kappa[e^{\kappa l}G_l^s-G_0^s-H(\kappa)],\\
e^{-\kappa l}S_l-S_0
&=\kappa[G_0^s-e^{-\kappa l}G_l^s-H(-\kappa)].
\end{aligned}
$$

Subtracting these equations and then substituting back gives the [semistrip Dirichlet-to-Neumann sine transforms](../../../../../../semistrip-dirichlet-to-neumann-sine-transforms.md) entirely in terms of the prescribed [Dirichlet boundary data](../../../../../../dirichlet-boundary-data.md):

$$
\boxed{S_0(\kappa)=\frac{\kappa}{\sinh(\kappa l)}
\left[-\cosh(\kappa l)G_0^s(\kappa)+G_l^s(\kappa)
+\int_0^l\sinh(\kappa(l-y))h(y)\,dy\right],}
$$



$$
\boxed{S_l(\kappa)=\frac{\kappa}{\sinh(\kappa l)}
\left[-G_0^s(\kappa)+\cosh(\kappa l)G_l^s(\kappa)
-\int_0^l\sinh(\kappa y)h(y)\,dy\right].}
$$

These are the requested transforms of $q_y$ itself. The bottom outward [Neumann boundary data](../../../../../../neumann-boundary-data.md) have the opposite sign. The apparent division at $\kappa=0$ is handled by a continuous limit whenever the corresponding moments exist; there is no singularity for any $\kappa>0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 86](../../../paper-86-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
