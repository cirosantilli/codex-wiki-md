<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $u_j=\dot p_j+\partial_iW_{ij}$. The noises required by a joint trajectory are $f_j=u_j+\Gamma\mu_j$ and $N_{ij}=W_{ij}+M\partial_i\mu_j$. Their independent [Gaussian white noise](../../../../../../gaussian-white-noise.md) weights give the [joint path probability of an order parameter and its flux](../../../../../../joint-path-probability-of-an-order-parameter-and-its-flux.md):

$$
\boxed{P_F[p,W]=\mathcal K[p,W]\exp\left[-\int\left\{\frac{|u+\Gamma\mu|^2}{2\sigma^2}+\frac{|W+M\nabla\mu|^2}{2\sigma_N^2}\right\}\right].}
$$

For the physically reversed path, $p$ is time-even and the transport flux $W$ is time-odd. Therefore $u\mapsto-u$, $W\mapsto-W$, and

$$
\boxed{P_B[p,W]=\mathcal K[p,W]\exp\left[-\int\left\{\frac{|-u+\Gamma\mu|^2}{2\sigma^2}+\frac{|-W+M\nabla\mu|^2}{2\sigma_N^2}\right\}\right].}
$$

The common factor includes the two noise normalizations and the midpoint [Jacobian determinant](../../../../../../jacobian-determinant.md). Its calculation must include both relaxation channels. On a finite spatial grid, let $\mathsf D$ and $\mathsf G$ represent the [divergence](../../../../../../divergence.md) and [gradient](../../../../../../gradient.md), with $\Delta=\mathsf D\mathsf G$ the discrete [Laplacian](../../../../../../laplacian.md), and let $\mathcal H_n=\partial\mu/\partial p$ be the [Hessian matrix](../../../../../../hessian-matrix.md) of $F$ at the midpoint of time step $n$. Differentiating the two required noises with respect to the next configuration and the interval flux gives the [Jacobian matrix](../../../../../../jacobian-matrix.md)

$$
\frac{\partial(f_n,N_n)}{\partial(p_{n+1},W_n)}=
\begin{pmatrix}
\frac{I}{\Delta t}+\Gamma\mathcal H_n/2&\mathsf D\\
M\mathsf G\mathcal H_n/2&I
\end{pmatrix}.
$$

Using the [Schur complement](../../../../../../schur-complement.md), its [Jacobian determinant](../../../../../../jacobian-determinant.md), apart from the path-independent power of $\Delta t$, is

$$
\det\left[I+\frac{\Delta t}{2}(\Gamma I-M\Delta)\mathcal H_n\right].
$$

Reversal visits the same midpoint configurations in reverse order, so the product of these factors is unchanged. The joint [time-reversal invariance of a path Jacobian](../../../../../../time-reversal-invariance-of-a-path-jacobian.md) therefore involves the complete relaxation operator $\Gamma I-M\Delta$.

Taking the action difference gives

$$
\boxed{\log\frac{P_F}{P_B}=-\frac{2\Gamma}{\sigma^2}\int\mu_j(\dot p_j+\partial_iW_{ij})-\frac{2M}{\sigma_N^2}\int W_{ij}\partial_i\mu_j.}
$$

Repeated component indices are summed. The second squared norm sums over both flux indices. This is [mixed conserved and nonconserved order-parameter dynamics](../../../../../../mixed-conserved-and-nonconserved-order-parameter-dynamics.md); reversing the order parameter history while leaving the flux unreversed would give the wrong probability ratio.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
