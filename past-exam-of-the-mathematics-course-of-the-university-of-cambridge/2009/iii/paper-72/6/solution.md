<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [eigenvalue stability analysis of a finite difference method](../../../../../eigenvalue-stability-analysis-of-a-finite-difference-method.md) reduces a linear evolution discretization to its modal behavior, but it must retain the [norm](../../../../../norm.md) and the dependence on the mesh. For a homogeneous system obtained by the [method of lines](../../../../../method-of-lines.md), $U'=A_hU$, the solution is $e^{tA_h}U(0)$. A one-step time discretization gives $U^{n+1}=G_{h,k}U^n$; for a [Runge-Kutta method](../../../../../runge-kutta-method.md), where its stage [matrices](../../../../../matrix.md) are invertible, $G_{h,k}=R(kA_h)$. With a [multistep method](../../../../../linear-multistep-method.md) one instead uses an amplification [matrix](../../../../../matrix.md) on the augmented [vector](../../../../../vector.md) of several time levels.

The relevant finite-time stability estimate is

$$
\boxed{\|G_{h,k}^n\|_h\leq C_T\quad\text{whenever }0\leq nk\leq T,}
$$

with $C_T$ independent of the refining spatial mesh and allowed time steps. Similarly, semidiscrete stability requires $\|e^{tA_h}\|_h\leq C_T$ for $0\leq t\leq T$. The [norm](../../../../../norm.md) should represent the continuum problem, such as the [discrete L2 norm](../../../../../discrete-l2-norm.md) $\|U\|_{2,h}^2=h\sum_j|U_j|^2$ in one dimension. A fixed finite [matrix](../../../../../matrix.md) having decaying solutions as $t\to\infty$ is not by itself a mesh-uniform result for the [partial differential equation](../../../../../partial-differential-equation-split.md).

If $G=X\Lambda X^{-1}$, then

$$
\|G^n\|\leq\|X\|\|X^{-1}\|\max_j|\lambda_j|^n.
$$

Thus [eigenvalues](../../../../../eigenvalue.md) of modulus at most one give a uniform bound when the diagonalizing [bases](../../../../../basis.md) have uniformly bounded [condition numbers](../../../../../condition-number.md). For a [normal matrix](../../../../../normal-matrix.md) in the chosen [inner product](../../../../../inner-product.md), the [spectral theorem for normal operators](../../../../../spectral-theorem-for-normal-operators.md) supplies an [orthonormal basis](../../../../../orthonormal-basis.md), so the [condition number](../../../../../condition-number.md) is one and the [norm](../../../../../norm.md) of $G^n$ is exactly $\max_j|\lambda_j|^n$. For a [self-adjoint](../../../../../self-adjoint-operator.md) or [skew-adjoint](../../../../../skew-adjoint-generator.md) spatial [matrix](../../../../../matrix.md), applying a scalar [stability function](../../../../../stability-function.md) preserves this favorable modal structure. This is the setting where [eigenvalue](../../../../../eigenvalue.md) calculations provide especially clean, reliable step restrictions.

A precise fixed-matrix statement is also useful: a [matrix](../../../../../matrix.md) is power bounded for all nonnegative integers $n$ if and only if all its [eigenvalues](../../../../../eigenvalue.md) lie in the closed [unit disk](../../../../../unit-disk.md) and every [Jordan block](../../../../../jordan-block.md) at a unit-modulus [eigenvalue](../../../../../eigenvalue.md) has size one. Indeed, powers of an interior [Jordan block](../../../../../jordan-block.md) contain a [polynomial](../../../../../polynomial-split.md) in $n$ times a decaying geometric factor and are bounded; a larger block on the unit circle produces unbounded [polynomial](../../../../../polynomial-split.md) growth. For a family of [matrices](../../../../../matrix.md), the resulting bounds must still be uniform. Moreover, [finite-time stability versus power boundedness](../../../../../finite-time-stability-versus-power-boundedness.md) distinguishes this all-time condition from the physical-time estimate above. For example $G_k=I+kN$, $N^2=0$, has $G_k^n=I+nkN$, bounded for $nk\leq T$ despite a nontrivial [Jordan block](../../../../../jordan-block.md) at one. Even the scalar update $1+k$ is stable on fixed intervals, since $(1+k)^n\leq e^T$, although it represents a growing equation rather than a contraction.

For a constant-coefficient periodic difference operator, [Fourier modes](../../../../../fourier-mode.md) diagonalize the spatial [matrix](../../../../../matrix.md). The [discrete Fourier transform](../../../../../discrete-fourier-transform.md) is a [unitary operator](../../../../../unitary-operator.md), so [Parseval's identity](../../../../../parseval-identity.md) identifies its modal maximum with the [operator norm](../../../../../operator-norm.md). The [eigenvalue stability analysis of a finite difference method](../../../../../eigenvalue-stability-analysis-of-a-finite-difference-method.md) then becomes [von Neumann stability analysis](../../../../../von-neumann-stability-analysis.md). For the [Dirichlet discrete Laplacian](../../../../../dirichlet-discrete-laplacian.md), a [discrete sine transform](../../../../../discrete-sine-transform.md) plays the same role. These facts explain its advantages: a large [matrix](../../../../../matrix.md) calculation becomes a scalar symbol or a known spectral interval, and the extremal [eigenvalue](../../../../../eigenvalue.md) directly determines a safe time step.

As a first example, centered space discretization of the [heat equation](../../../../../heat-equation.md) $u_t=u_{xx}$ has [eigenvalues](../../../../../eigenvalue.md)

$$
\lambda(\theta)=-\frac4{h^2}\sin^2(\theta/2).
$$

[Forward Euler method](../../../../../euler-method.md) gives $R(k\lambda)=1-4r\sin^2(\theta/2)$ with $r=k/h^2$. Requiring all factors in $[-1,1]$ yields $0\leq r\leq1/2$ for all periodic meshes. In two dimensions the corresponding uniform bound is $r\leq1/4$. Because these are [normal matrices](../../../../../normal-matrix.md), these scalar bounds prove contraction rather than merely suggest it.

[Backward Euler method](../../../../../backward-euler-method.md) has $R(z)=1/(1-z)$, so the centered discretization of the [heat equation](../../../../../heat-equation.md) is contractive for every $k>0$. The [Crank-Nicolson method](../../../../../crank-nicolson-method.md) has $R(z)=(1+z/2)/(1-z/2)$ and is likewise contractive for these negative real modes. However, its factor tends to $-1$ for very stiff modes, leaving high-frequency oscillations weakly damped; [Backward Euler method](../../../../../backward-euler-method.md) tends to zero. The [eigenvalues](../../../../../eigenvalue.md) therefore expose the presence of [stiff differential equations](../../../../../stiff-equation.md) and damping as well as binary stability. Unconditional stability does not remove accuracy requirements.

For an [advection equation](../../../../../transport-equation.md) example, the [upwind finite difference scheme](../../../../../upwind-finite-difference-scheme.md) for $u_t+c u_x=0$, $c>0$, has factor $G=1-\nu+\nu e^{-i\theta}$, with $\nu=ck/h$. Since

$$
|G|^2=1-2\nu(1-\nu)(1-\cos\theta),
$$

it is a contraction in the periodic [discrete L2 norm](../../../../../discrete-l2-norm.md) exactly for $0\leq\nu\leq1$. In contrast, [Forward Euler method](../../../../../euler-method.md) with centered advection has factor $1-i\nu\sin\theta$. Its modulus exceeds one at nonzero active frequencies, and repeated amplification makes it unstable under fixed nonzero Courant refinement. A much smaller scaling $k=O(h^2)$ can bound its finite-time growth, demonstrating again that exact contraction and the most general stability estimate are different claims.

The major limitation is the possible presence of a [nonnormal matrix](../../../../../non-normal-matrix.md). For example,

$$
A_h=\begin{pmatrix}-1&h^{-1}\\0&-1\end{pmatrix},\qquad
e^{tA_h}=e^{-t}\begin{pmatrix}1&t/h\\0&1\end{pmatrix}.
$$

Both [eigenvalues](../../../../../eigenvalue.md) are negative, yet at $t=1$ the second unit [vector](../../../../../vector.md) is amplified by at least $1/(eh)$. This proves that [negative spectra do not imply uniform semidiscrete stability](../../../../../negative-spectra-do-not-imply-uniform-semidiscrete-stability.md). Ill-conditioned [eigenvectors](../../../../../eigenvector.md), [Jordan normal form](../../../../../jordan-normal-form.md) and transient amplification can invalidate a spectral-only argument. Direct [energy estimates](../../../../../energy-estimate.md) or estimates for the [resolvent](../../../../../resolvent-of-an-operator.md) can supply the missing [norm](../../../../../norm.md) control.

[Boundary conditions](../../../../../boundary-condition.md) are another limitation. A periodic symbol proves a periodic or whole-line result, not an arbitrary initial-boundary-value problem. [Boundary closure of a difference scheme](../../../../../boundary-closure-of-a-difference-scheme.md) can introduce growing modes or mesh-dependent amplification. A spatial operator with variable coefficients can still be studied through its assembled [matrix](../../../../../matrix.md), but then whether it is a [normal matrix](../../../../../normal-matrix.md), its [condition number](../../../../../condition-number.md) and the physical [inner product](../../../../../inner-product.md) must be checked rather than borrowed from a [Fourier stability analysis](../../../../../fourier-stability-analysis.md). For the [finite element method](../../../../../finite-element-method.md) the natural [mass matrix](../../../../../mass-matrix.md) [inner product](../../../../../inner-product.md) often turns a [generalized eigenvalue problem](../../../../../generalized-eigenvalue-problem.md) into a [self-adjoint](../../../../../self-adjoint-operator.md) one.

For time-dependent or split updates, separate spectra are insufficient to control products. For instance, $G_1=\begin{pmatrix}0&K\\0&0\end{pmatrix}$ and $G_2=\begin{pmatrix}0&0\\K&0\end{pmatrix}$ each have only zero [eigenvalues](../../../../../eigenvalue.md), while $G_2G_1$ has [eigenvalue](../../../../../eigenvalue.md) $K^2$. For $K>1$, alternating the two is unstable. A common contractive [norm](../../../../../norm.md) would control the products, but their individual [eigenvalues](../../../../../eigenvalue.md) do not.

Finally, stability and [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) have different roles. The [Lax equivalence theorem](../../../../../lax-equivalence-theorem.md) states that, for a well-posed linear initial-value problem and a consistent [finite difference method](../../../../../finite-difference-method.md) on compatible grid spaces, stability on every fixed time interval is equivalent to [convergence of a numerical method](../../../../../convergence-of-a-numerical-method.md) as the admissible meshes refine. Bounded grid representation and the correct initial and boundary setup are part of that framework. An [eigenvalue](../../../../../eigenvalue.md) estimate can establish its stability hypothesis in the favorable settings described above; it neither proves [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) nor bypasses its uniformity requirements. The method is therefore a powerful modal tool, provided its spectral calculation is connected to a genuine [norm](../../../../../norm.md) estimate.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 72](../../paper-72-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
