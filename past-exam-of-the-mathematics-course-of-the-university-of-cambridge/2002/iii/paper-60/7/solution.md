<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

[Stability of a numerical method](../../../../../stability-of-a-numerical-method.md) controls how perturbations in initial data, roundoff and local residuals propagate. For a linear evolution scheme $U^{n+1}=S_hU^n+kF^n$, a suitable finite-time requirement is

$$
\sup_{nk\leq T}\|S_h^n\|\leq C_T,
$$

with $C_T$ independent of the refining mesh. The norm should approximate the norm of the continuous problem, such as an area-weighted [L2 norm](../../../../../l2-norm.md). The bound need not imply decay: $C_T=e^{CT}$ is appropriate when the equation itself permits finite-time growth. For a multilevel scheme the state includes all required time levels.

The error recurrence shows why [stability](../../../../../stability-of-a-numerical-method.md) matters. If $e^{n+1}=S_he^n+k\tau^n$, then

$$
e^n=S_h^ne^0+k\sum_{j=0}^{n-1}S_h^{n-1-j}\tau^j,qquad
\|e^n\|\leq C_T(\|e^0\|+T\max_j\|\tau^j\|).
$$

Thus a consistent residual tending to zero and a convergent start produce convergence when the [stability](../../../../../stability-of-a-numerical-method.md) constant is uniform. Tiny defects need not remain tiny without that bound. The [Lax equivalence theorem](../../../../../lax-equivalence-theorem.md) makes this precise: for a well-posed linear [initial value problem](../../../../../initial-value-problem.md) and a consistent linear approximation, [stability](../../../../../stability-of-a-numerical-method.md) is equivalent to convergence in the compatible solution norms. It is not a theorem for arbitrary nonlinear schemes, and a high formal order does not substitute for [stability](../../../../../stability-of-a-numerical-method.md).

For constant coefficients on a periodic or infinite grid, [von Neumann stability analysis](../../../../../von-neumann-stability-analysis.md) diagonalizes spatial translations using [Fourier modes](../../../../../fourier-mode.md). If $\widehat U^{n+1}=g(\theta)\widehat U^n$, the [Parseval identity](../../../../../parseval-identity.md) converts a uniform multiplier-power bound into an [L2 norm](../../../../../l2-norm.md) bound. The contraction condition $|g(\theta)|\leq1$ is sufficient; a more general $|g(\theta)|\leq1+Ck$ also yields a finite-time bound. For the centered-space explicit heat method,

$$
g(\theta)=1-4\mu\sin^2(\theta/2),\qquad \mu=k/h^2,
$$

so $|g|\leq1$ exactly for $0\leq\mu\leq1/2$. Larger fixed Courant numbers amplify high frequencies. The [Backward Euler method](../../../../../backward-euler-method.md) gives instead $g=[1+4\mu\sin^2(\theta/2)]^{-1}$ and is contractive for every $\mu\geq0$.

For $u_t=u_x$, forward time and centered space give $g=1+i\nu\sin\theta$, with $\nu=k/h$. Hence $|g|^2=1+\nu^2\sin^2\theta>1$ for nonzero frequencies, causing instability at a fixed nonzero [Courant number](../../../../../courant-number.md). The directionally correct [upwind finite difference scheme](../../../../../upwind-finite-difference-scheme.md) uses the neighbor at $m+1$ and has

$$
g=1-\nu+\nu e^{i\theta},\qquad
|g|^2=1-4\nu(1-\nu)\sin^2(\theta/2).
$$

It is contractive exactly for $0\leq\nu\leq1$. This also has a direct maximum-norm proof: the update is a convex combination of two old values. The continuum domain of dependence must fit inside the numerical one for a local explicit hyperbolic method to converge, giving the [Courant–Friedrichs–Lewy condition](../../../../../courant-friedrichs-lewy-condition.md). That necessary geometric restriction is not by itself a sufficient [stability](../../../../../stability-of-a-numerical-method.md) proof.

For systems and multilevel methods, each Fourier multiplier becomes a [matrix](../../../../../matrix.md). All [amplification roots](../../../../../amplification-root.md) must obey the appropriate root bound, but their moduli alone are insufficient. A repeated unit root in a companion [matrix](../../../../../matrix.md) gives a [Jordan block](../../../../../jordan-block.md); for instance $J=\begin{pmatrix}1&1\\0&1\end{pmatrix}$ has $J^n=\begin{pmatrix}1&n\\0&1\end{pmatrix}$. Even distinct roots require control of the diagonalizing [matrices](../../../../../matrix.md) uniformly in frequency and mesh. The [uniform power bound from separated amplification roots](../../../../../uniform-power-bound-from-separated-amplification-roots.md) supplies such control for a bounded two-root family with a positive gap. Question5 illustrates both sides: strict $0<\mu<1$ gives a uniform gap, whereas the endpoints have a double unit root and are unstable despite unit moduli.

[Energy estimates](../../../../../energy-estimate.md) are especially useful when coefficients vary or boundaries prevent Fourier diagonalization. As a simple example, for implicit heat evolution with homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), take the grid inner product of $(U^{n+1}-U^n)/k=D_{xx}U^{n+1}$ with $U^{n+1}$. Discrete integration by parts gives

$$
\frac12\left(\|U^{n+1}\|_h^2-\|U^n\|_h^2+\|U^{n+1}-U^n\|_h^2\right)
=-k\|D_+U^{n+1}\|_h^2\leq0.
$$

The boundary term vanishes because the boundary values are zero, proving contraction. For variable positive diffusion coefficients the corresponding flux-weighted squared differences remain nonnegative, so the argument extends without a constant-coefficient Fourier symbol. With forcing or lower-order terms, a discrete energy inequality and [Gronwall inequality](../../../../../gronwall-inequality.md) yield a mesh-independent finite-time bound.

A related technique is [eigenvalue stability analysis of a finite difference method](../../../../../eigenvalue-stability-analysis-of-a-finite-difference-method.md). If the spatial [matrix](../../../../../matrix.md) $L_h$ is symmetric with nonpositive [eigenvalues](../../../../../eigenvalue.md) and the time update is $R(kL_h)$, an orthonormal eigenbasis gives

$$
\|R(kL_h)^n\|_2=\max_j|R(k\lambda_j)|^n.
$$

This proves [stability](../../../../../stability-of-a-numerical-method.md) when all scaled spatial [eigenvalues](../../../../../eigenvalue.md) lie in the time method's [stability](../../../../../stability-of-a-numerical-method.md) domain. For a nonnormal spatial or amplification [matrix](../../../../../matrix.md), the [eigenvalues](../../../../../eigenvalue.md) alone do not control powers: ill-conditioned [eigenvectors](../../../../../eigenvector.md) or Jordan terms can cause transient growth. Direct operator-norm estimates, symmetrizers or energy estimates then provide the missing information. In particular an [A-stable](../../../../../a-stability.md) scalar time formula does not automatically give mesh-uniform bounds for every ill-conditioned family of spatial [matrices](../../../../../matrix.md).

Boundary conditions and starting procedures are part of the discretization. Interior Fourier analysis may fail to detect a growing boundary mode, and a multilevel method can excite a parasitic mode through a poor start. One must therefore analyze the actual finite-domain operator or include its boundary terms in an energy proof. **[Stability](../../../../../stability-of-a-numerical-method.md) is a uniform error-propagation bound; Fourier symbols, energy identities, [matrix](../../../../../matrix.md) norms and spectral analysis are complementary ways of establishing that bound.**

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
