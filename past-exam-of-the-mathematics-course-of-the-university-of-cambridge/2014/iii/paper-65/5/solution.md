<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [kernel support vector machine](../../../../../kernel-support-vector-machine.md) constructs a large-margin classifier in a feature [Hilbert space](../../../../../hilbert-space-split.md). Given training points $x_i$ and labels $y_i\in\{-1,1\}$, choose a feature map $\Phi:X\to\mathcal H$ and an affine score $f(x)=\langle w,\Phi(x)\rangle+b$. Prediction is the sign of the score. Normalizing the functional margin to one makes the closest separating geometric margin $1/\|w\|$, and the full margin between the two supporting hyperplanes is $2/\|w\|$. Maximizing that margin therefore minimizes $\frac12\|w\|^2$.

For separable data, the hard-margin [support vector machine](../../../../../support-vector-machine.md) primal is

$$
\boxed{\min_{w,b}\frac12\|w\|_{\mathcal H}^2\quad
\text{subject to }y_i(\langle w,\Phi(x_i)\rangle+b)\geq1.}
$$

Noisy or nonseparable data use slack variables and the [soft-margin support vector machine](../../../../../soft-margin-support-vector-machine.md):

$$
\boxed{\min_{w,b,\xi}\frac12\|w\|_{\mathcal H}^2+C\sum_i\xi_i,\quad
 y_i(\langle w,\Phi(x_i)\rangle+b)\geq1-\xi_i,\quad\xi_i\geq0,\quad C>0.}
$$

Eliminating $\xi$ gives the equivalent [hinge loss](../../../../../hinge-loss.md) objective $\frac12\|w\|^2+C\sum_i(1-y_if(x_i))_+$. The parameter balances margin size against violations; it is not a hard bound on their number. The bias is unpenalized here, which determines the equality constraint in the dual.

Attach multipliers $\alpha_i\geq0$ to $1-\xi_i-y_if(x_i)\leq0$ and $\eta_i\geq0$ to $-\xi_i\leq0$. The [Lagrangian](../../../../../lagrangian.md) is

$$
\mathcal L=\frac12\|w\|^2+C\sum_i\xi_i+
\sum_i\alpha_i[1-\xi_i-y_i(\langle w,\Phi(x_i)\rangle+b)]-\sum_i\eta_i\xi_i.
$$

Stationarity gives $w=\sum_i\alpha_i y_i\Phi(x_i)$, $\sum_i\alpha_i y_i=0$ and $C-\alpha_i-\eta_i=0$. Eliminating $w,b,\xi$ yields

$$
\boxed{\max_\alpha\sum_i\alpha_i-\frac12\sum_{i,j}\alpha_i\alpha_jy_iy_jk(x_i,x_j),\quad
\sum_i\alpha_i y_i=0,\quad0\leq\alpha_i\leq C,}
$$

where $k(x,x')=\langle\Phi(x),\Phi(x')\rangle$ is a [positive-definite kernel](../../../../../positive-semidefinite-kernel.md), meaning positive semidefinite Gram matrices. The hard-margin dual is the same objective with only $\alpha_i\geq0$, without the upper bound. Soft-margin strict feasibility follows by taking $w=b=0$ and all $\xi_i>1$, so [strong duality](../../../../../strong-duality.md) and the [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) apply. For separable hard-margin data a separator can be rescaled to give strict margins, supplying the analogous qualification. Although the feature space may be infinite dimensional, projecting $w$ onto the finite span of the training feature vectors preserves scores and cannot increase its norm, so this optimization reduces to a finite span.

The [complementary slackness](../../../../../complementary-slackness.md) relations are

$$
\alpha_i[y_if(x_i)-1+\xi_i]=0,\qquad(C-\alpha_i)\xi_i=0.
$$

Points with $\alpha_i>0$ are [support vectors](../../../../../support-vector.md). If $0<\alpha_i<C$, then $\xi_i=0$ and $y_if(x_i)=1$; such a point gives $b=y_i-\sum_j\alpha_jy_jk(x_j,x_i)$. A point with $\alpha_i=C$ can lie inside the margin or be misclassified, while $\alpha_i=0$ contributes no term to $w$. If no coefficient lies strictly between the bounds, an admissible bias must be obtained from the KKT inequalities, rather than dividing by a nonexistent margin vector. Bias and dual coefficients can be nonunique even when the optimal feature-space weight is unique.

The [kernel trick](../../../../../kernel-trick.md) operates both during training and prediction. The dual optimization uses only the [Gram matrix](../../../../../gram-matrix.md) $K_{ij}=k(x_i,x_j)$, so the feature vectors need not be formed. Prediction likewise uses

$$
\boxed{f(x)=\sum_{i:\alpha_i>0}\alpha_i y_i k(x_i,x)+b.}
$$

A nonlinear kernel therefore makes a linear separator in feature space represent a nonlinear boundary in input space. For example, on $\mathbb R^2$ the degree-two polynomial kernel $(x\cdot x')^2$ corresponds to $\Phi(x)=(x_1^2,\sqrt2x_1x_2,x_2^2)$. Gaussian kernels yield infinite-dimensional feature spaces. An arbitrary similarity is not automatically a valid kernel: for every finite collection and real coefficients $a_i$, one needs $\sum_{i,j}a_ia_jk(x_i,x_j)\geq0$. This makes the dual quadratic form positive semidefinite and the maximization concave.

[Mercer's theorem](../../../../../mercer-s-theorem.md) gives a spectral realization under its additional analytic hypotheses. For a continuous symmetric positive-semidefinite kernel on a compact domain with a finite full-support measure, the integral operator $(T_kf)(x)=\int k(x,x')f(x')\,d\mu(x')$ is compact, self-adjoint and positive. The Mercer expansion is

$$
k(x,x')=\sum_j\lambda_j e_j(x)e_j(x'),\qquad\lambda_j\geq0,
$$

with the standard uniform convergence conclusions under these hypotheses. Since $\sum_j\lambda_j e_j(x)^2=k(x,x)<\infty$, the nonlinear feature map

$$
\boxed{\Phi(x)=(\sqrt{\lambda_j}e_j(x))_j\in\ell^2,\qquad
k(x,x')=\langle\Phi(x),\Phi(x')\rangle_{\ell^2}}
$$

is well defined. This explains the connection of [Mercer kernels](../../../../../mercer-kernel.md) to [Hilbert space](../../../../../hilbert-space-split.md) features, rather than treating the [kernel trick](../../../../../kernel-trick.md) as a purely formal substitution.

The finite-Gram positivity condition is more general than this compact-domain spectral theorem. Every such kernel generates a [Reproducing kernel Hilbert space](../../../../../reproducing-kernel-hilbert-space.md): on finite sums of kernel sections define

$$
\left\langle\sum_i a_i k(x_i,\cdot),\sum_j b_j k(z_j,\cdot)\right\rangle
=\sum_{i,j}a_ib_j k(x_i,z_j),
$$

quotient out zero-norm elements, and complete. The resulting space satisfies the [reproducing property](../../../../../reproducing-property.md) $h(x)=\langle h,k(x,\cdot)\rangle$. Its canonical feature map is $\Phi(x)=k(x,\cdot)$, whose inner product is exactly $k(x,x')$. A feature map need not be injective; calling it an embedding does not by itself prove distinct inputs remain distinct. The [kernel support vector machine](../../../../../kernel-support-vector-machine.md) uses this geometry together with convex duality to fit and evaluate a maximum-margin classifier while accessing the geometry only through kernel evaluations.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
