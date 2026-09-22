# Time-reversal invariance of a path Jacobian

↑ **Parent:** [Onsager--Machlup path probability](onsager-machlup-path-probability.md)

For additive [Gaussian white noise](gaussian-white-noise.md) and a time-even [order parameter](order-parameter.md), a midpoint discretization of the [Onsager–Machlup functional](onsager-machlup-functional.md) evaluates drift derivatives at the midpoint configurations. Reversing a trajectory visits the same midpoints in reverse order, so the noise-to-path [Jacobian determinant](jacobian-determinant.md) is invariant under reversal. It may depend on the trajectory, and must be distinguished from the constant normalization of the noise measure.

For [nonconserved order-parameter dynamics](nonconserved-order-parameter-dynamics.md) with $\dot p=-\Gamma\mu[p]+f$, the factor at one time step, apart from a path-independent power of the step size, is

$$
\mathcal J_n=\left|\det\left[I+\frac{\Gamma\Delta t}{2}\mathcal H_n\right]\right|,
\qquad \mathcal H_n=\frac{\partial\mu}{\partial p}\bigg|_{(p_n+p_{n+1})/2}.
$$

Here the fields have first been restricted to a finite spatial grid, and $\mathcal H_n$ is the [Hessian matrix](hessian-matrix.md) of the [free energy](thermodynamic-free-energy.md).

For [mixed conserved and nonconserved order-parameter dynamics](mixed-conserved-and-nonconserved-order-parameter-dynamics.md), the required noises for a joint configuration and flux trajectory are

$$
f_n=\frac{p_{n+1}-p_n}{\Delta t}+\mathsf D W_n+\Gamma\mu_n,
\qquad N_n=W_n+M\mathsf G\mu_n,
$$

where $\mathsf D,\mathsf G$ represent the [divergence](divergence.md) and [gradient](gradient.md), and $\Delta=\mathsf D\mathsf G$ represents the [Laplacian](laplacian.md). The [Jacobian matrix](jacobian-matrix.md) is

$$
\frac{\partial(f_n,N_n)}{\partial(p_{n+1},W_n)}=
\begin{pmatrix}
\frac{I}{\Delta t}+\Gamma\mathcal H_n/2&\mathsf D\\
M\mathsf G\mathcal H_n/2&I
\end{pmatrix}.
$$

Taking its [Schur complement](schur-complement.md) gives the joint factor

$$
\boxed{\mathcal J_n=\left|\det\left[I+\frac{\Delta t}{2}(\Gamma I-M\Delta)\mathcal H_n\right]\right|.}
$$

For [periodic boundary conditions](periodic-boundary-conditions.md), discretizing the two spatial operators compatibly gives $\mathsf D=-\mathsf G^{\mathsf T}$, so $\Gamma I-M\Delta$ is the positive relaxation operator when $\Gamma,M>0$. Reversal leaves $\mathcal H_n$ unchanged and reverses the sign of the flux. The product of the joint factors is consequently the same for both histories, justifying its cancellation from the [joint path probability of an order parameter and its flux](joint-path-probability-of-an-order-parameter-and-its-flux.md). The [functional chain rule](functional-chain-rule.md) used in the action ratio holds in the continuum limit of this midpoint convention.

## ↑ Ancestors (8)

1. [Onsager--Machlup path probability](onsager-machlup-path-probability.md)
2. [Nonconserved order-parameter dynamics](nonconserved-order-parameter-dynamics.md)
3. [Order parameter](order-parameter.md)
4. [Critical phenomenon](critical-phenomenon-split.md)
5. [Statistical physics](statistical-physics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Joint path probability of an order parameter and its flux](joint-path-probability-of-an-order-parameter-and-its-flux.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-344/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-344/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344/2/d/solution.md)
