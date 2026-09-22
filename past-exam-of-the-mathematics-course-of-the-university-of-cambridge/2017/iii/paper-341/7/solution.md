<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For a fully discrete linear [partial differential equation](../../../../../partial-differential-equation-split.md) evolution, write $U^{n+1}=C_{h,k}U^n$ in a specified discrete [norm](../../../../../norm.md). Finite-time [stability of a numerical method](../../../../../stability-of-a-numerical-method.md) means

$$
\boxed{\|C_{h,k}^{\,n}\|\leq C_T\quad\text{whenever }nk\leq T},
$$

with $C_T$ independent of the allowed meshes. For a [multistep method](../../../../../linear-multistep-method.md), augment the state with its time-history values and include a stable starter. Bounds may grow as $e^{\omega T}$ when the continuous problem has growth; demanding decay for all time would be a stronger assertion. The treatment of initial data, forcing, [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), and the [norm](../../../../../norm.md) is part of the hypothesis, not a detail supplied by an interior calculation.

For constant coefficients on an infinite or periodic uniform grid, [von Neumann stability analysis](../../../../../von-neumann-stability-analysis.md) substitutes the [Fourier mode](../../../../../fourier-mode.md) $U_j^n=G(\theta)^ne^{ij\theta}$. The [discrete Fourier transform](../../../../../discrete-fourier-transform.md) and the [Parseval identity](../../../../../parseval-identity.md) turn a uniform multiplier estimate into a discrete [L2 norm](../../../../../l2-norm.md) estimate. In a one-step scalar scheme, $|G(\theta)|\leq1$ proves contractivity, while $|G(\theta)|\leq1+\omega k$ gives finite-time [stability](../../../../../stability-of-a-numerical-method.md). In a multilevel scheme, every [root of a polynomial](../../../../../root-of-a-polynomial.md) in its [amplification polynomial of a multilevel finite difference scheme](../../../../../amplification-polynomial-of-a-multilevel-finite-difference-scheme.md) matters, as does uniform control of the associated companion [matrix](../../../../../matrix.md).

For the [Forward Euler diffusion scheme](../../../../../forward-euler-diffusion-scheme.md) with $\mu=k/h^2$,

$$
G(\theta)=1-4\mu\sin^2(\theta/2).
$$

Thus $|G|\leq1$ for all frequencies exactly when

$$
\boxed{0\leq\mu\leq\frac12}.
$$

Sufficiency follows since $G\in[-1,1]$; necessity follows from the highest-frequency mode $\theta=\pi$ on even periodic grids. This gives the usual parabolic mesh restriction $k\leq h^2/2$. For the [Backward Euler diffusion scheme](../../../../../backward-euler-diffusion-scheme.md),

$$
G(\theta)=\frac1{1+4\mu\sin^2(\theta/2)},
$$

so every $\mu\geq0$ is stable. The [Crank-Nicolson method](../../../../../crank-nicolson-method.md) has

$$
G(\theta)=\frac{1-2\mu\sin^2(\theta/2)}{1+2\mu\sin^2(\theta/2)},
$$

again of [modulus](../../../../../modulus.md) at most one for all $\mu\geq0$, but stiff modes approach $-1$ rather than zero. These are PDE manifestations of the [A-stability](../../../../../a-stability.md) and [L-stability](../../../../../l-stability.md) distinctions for time integration.

For advection $u_t+a u_x=0$, assume $a>0$ and set $\nu=ak/h$. The [upwind finite difference scheme](../../../../../upwind-finite-difference-scheme.md) is $U_j^{n+1}=(1-\nu)U_j^n+\nu U_{j-1}^n$, with

$$
|G(\theta)|^2=1-2\nu(1-\nu)(1-\cos\theta).
$$

It is contractive when $0\leq\nu\leq1$. This also has a direct maximum-norm proof: each newest value is a [convex combination](../../../../../convex-combination.md) of two old values. The resulting [Courant–Friedrichs–Lewy condition](../../../../../courant-friedrichs-lewy-condition.md) expresses that the numerical [domain of dependence](../../../../../domain-of-dependence.md) covers the physical one. For negative $a$, the upwind direction must be reversed. By contrast, [Forward Euler method](../../../../../euler-method.md) time stepping with the centered first [finite difference](../../../../../finite-difference-split.md) has $G=1-i\nu\sin\theta$ and $|G|>1$ for nonzero $\nu\sin\theta$. Under fixed nonzero $\nu$ refinement it is unstable, since a fixed nontrivial mode grows geometrically over $T/k$ steps. This is not a claim of instability under every imaginable mesh coupling: $k=O(h^2)$ instead bounds its spurious finite-time growth, since $\log|G|\leq a^2k^2/(2h^2)$.

The [leapfrog advection scheme](../../../../../leapfrog-advection-scheme.md) illustrates a multilevel subtlety. Its [amplification polynomial of a multilevel finite difference scheme](../../../../../amplification-polynomial-of-a-multilevel-finite-difference-scheme.md) is

$$
\xi^2+2i\nu\sin\theta\,\xi-1=0.
$$

For $|\nu|<1$, both [roots of a polynomial](../../../../../root-of-a-polynomial.md) have unit [modulus](../../../../../modulus.md) and separation at least $2\sqrt{1-\nu^2}$. A uniformly conditioned eigenbasis of the companion [matrix](../../../../../matrix.md) then proves [power boundedness of a two-level Fourier scheme](../../../../../power-boundedness-of-a-two-level-fourier-scheme.md) for arbitrary history data. At $|\nu|=1$ and a grid admitting $\theta=\pi/2$, the roots coincide on the [unit circle](../../../../../complex-unit-circle.md), and a [Jordan block](../../../../../jordan-block.md) produces $n\xi^n$ growth. Thus the endpoint fails the ordinary arbitrary-history [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md); checking only that both moduli equal one misses the instability. Restricting the starter or filtering the parasitic mode is an additional hypothesis.

The [energy method](../../../../../energy-method.md) handles variable coefficients and finite boundaries for which [Fourier stability analysis](../../../../../fourier-stability-analysis.md) may be unavailable. For the [Backward Euler diffusion scheme](../../../../../backward-euler-diffusion-scheme.md) with homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), define $\|U\|_h^2=h\sum_j|U_j|^2$. The discrete [summation by parts](../../../../../abel-s-summation-formula.md) identity is

$$
\langle U,L_hU\rangle_h=-\|D_+U\|_h^2.
$$

Take the [inner product](../../../../../inner-product.md) of $U^{n+1}-U^n=kL_hU^{n+1}$ with $2U^{n+1}$. The elementary identity $2\operatorname{Re}\langle x-y,x\rangle=\|x\|^2-\|y\|^2+\|x-y\|^2$ gives

$$
\|U^{n+1}\|_h^2-\|U^n\|_h^2
+\|U^{n+1}-U^n\|_h^2+2k\|D_+U^{n+1}\|_h^2=0.
$$

This proves unconditional contractivity including the actual boundary treatment. More generally, a [dissipative operator](../../../../../dissipative-operator.md) $L_h$ gives $(I-kL_h)^{-1}$ of [operator norm](../../../../../operator-norm.md) at most one: with $V=(I-kL_h)U$, dissipativity implies $\operatorname{Re}\langle V,U\rangle\geq\|U\|^2$, and the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $\|U\|\leq\|V\|$. In finite dimensions this also proves invertibility. For the second-order [backward differentiation formula](../../../../../backward-differentiation-formula.md), the [BDF2 discrete energy identity](../../../../../bdf2-discrete-energy-identity.md) used in question 4 controls both time levels and proves unconditional diffusion stability. A repeated root strictly inside the disk is harmless here; the energy argument supplies the uniform bound without a singular [eigenvector](../../../../../eigenvector.md) formula.

A second technique is [eigenvalue stability analysis of a finite difference method](../../../../../eigenvalue-stability-analysis-of-a-finite-difference-method.md). Under the [method of lines](../../../../../method-of-lines.md), a time integrator advances $U'=L_hU$ by $R(kL_h)$. If $L_h$ is a [normal matrix](../../../../../normal-matrix.md), the scalar [linear stability domain](../../../../../linear-stability-domain.md) criterion on all $k\lambda_j(L_h)$ controls its powers exactly in the corresponding [L2 norm](../../../../../l2-norm.md). For the centered [Dirichlet discrete Laplacian](../../../../../dirichlet-discrete-laplacian.md), its [eigenvalues](../../../../../eigenvalue.md) lie between $-4/h^2$ and zero; intersecting this interval with a time integrator's stability interval determines its mesh restriction. A uniform bound on the [diagonalization of a matrix](../../../../../diagonalization-of-a-matrix.md) is needed for nonnormal diagonalizable systems. Eigenvalues alone can be misleading. For example,

$$
C_{h,k}=\begin{pmatrix}1-k&k/h\\0&1-k\end{pmatrix}
$$

has both [eigenvalues](../../../../../eigenvalue.md) inside the disk for $0<k<1$, but the upper-right entry of $C_{h,k}^n$ is $nk(1-k)^{n-1}/h$. Taking $k=h$, $nk\to T>0$, this grows like $Te^{-T}/h$. Hence stable scalar [eigenvalues](../../../../../eigenvalue.md) do not give mesh-uniform [stability](../../../../../stability-of-a-numerical-method.md). Boundary closures can introduce precisely the extra growth that an interior [Fourier symbol](../../../../../fourier-symbol-of-a-difference-operator.md) overlooks, so [boundary stability of a finite-difference method](../../../../../boundary-stability-of-a-finite-difference-method.md) must be checked separately.

For nonlinear spatial discretizations, a useful replacement for [Fourier stability analysis](../../../../../fourier-stability-analysis.md) is a convexity argument. If the [Forward Euler method](../../../../../euler-method.md) map $E_k(U)=U+kF(U)$ is nonexpansive in a chosen [norm](../../../../../norm.md) for $k\leq k_{\mathrm{FE}}$, the second-order [strong stability preserving Runge-Kutta method](../../../../../strong-stability-preserving-runge-kutta-method.md)

$$
Y=E_k(U),\qquad
U_{\mathrm{new}}=\frac12U+\frac12E_k(Y)
$$

is also nonexpansive under the same restriction. Indeed, for two inputs, the [triangle inequality](../../../../../triangle-inequality.md) gives $\|U_{\mathrm{new}}-\widetilde U_{\mathrm{new}}\|\leq\frac12\|U-\widetilde U\|+\frac12\|E_k(Y)-E_k(\widetilde Y)\|\leq\|U-\widetilde U\|$. Its [Taylor expansion](../../../../../taylor-expansion.md) is $U+kF(U)+k^2F'(U)F(U)/2+O(k^3)$, proving order two. Such [strong stability preserving Runge-Kutta methods](../../../../../strong-stability-preserving-runge-kutta-method.md) transfer suitable forward-step bounds without relying on a linear spectral calculation.

Finally, [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) explains what stability buys. For a linear [Hadamard well-posed problem](../../../../../well-posed-problem.md), the [Lax equivalence theorem](../../../../../lax-equivalence-theorem.md) equates convergence of a consistent discretization with its [stability](../../../../../stability-of-a-numerical-method.md), under the stated approximation-space and norm hypotheses. Directly, if the error satisfies $e^{n+1}=C_{h,k}e^n+k\tau^n$, iteration gives the discrete [Duhamel principle](../../../../../duhamel-s-principle.md)

$$
e^n=C_{h,k}^ne^0+k\sum_{j=0}^{n-1}C_{h,k}^{n-1-j}\tau^j,
\qquad
\|e^n\|\leq C_T\bigl(\|e^0\|+T\max_j\|\tau^j\|\bigr).
$$

Thus vanishing normalized [local truncation error](../../../../../local-truncation-error.md) and initial error yield convergence. With a nonlinear Lipschitz step estimate, the [discrete Gronwall inequality](../../../../../discrete-gronwall-inequality.md) plays the same role. A stable but inconsistent stencil, such as the literal defective formulas in questions 3 and 4 under their usual refinement, is not rescued by any amplification bound. **The decisive checks are a mesh-uniform evolution bound, a valid boundary closure, and consistency with the actual PDE.**

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 341](../../paper-341-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
