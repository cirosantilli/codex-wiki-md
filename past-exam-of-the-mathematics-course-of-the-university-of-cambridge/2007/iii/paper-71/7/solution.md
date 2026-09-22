<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

[Fourier stability analysis](../../../../../fourier-stability-analysis.md) exploits translation invariance of a linear constant-coefficient [finite difference method](../../../../../finite-difference-method.md). On an infinite uniform grid of spacing $h$, a spatial shift acts on $e^{ij\theta}$ by multiplication by $e^{i\theta}$. Hence a scalar two-level scheme with new- and old-time symbols $L(\theta),N(\theta)$ propagates each [Fourier mode](../../../../../fourier-mode.md) by $G(\theta)=N(\theta)/L(\theta)$, provided the new-time operator is invertible. An explicit stencil $U_j^{n+1}=\sum_\ell a_\ell U_{j+\ell}^n$ simply has $G(\theta)=\sum_\ell a_\ell e^{i\ell\theta}$. This converts a spatial evolution into scalar algebra at each frequency.

The [Plancherel theorem](../../../../../plancherel-theorem.md) gives the full norm estimate, rather than just a heuristic about waves. For the discrete Fourier transform $\widehat U(\theta)=\sum_j U_j e^{-ij\theta}$, interpreted in the $L^2$ sense if necessary,

$$
\|U\|_h^2=h\sum_j|U_j|^2=\frac h{2\pi}\int_{-\pi}^{\pi}|\widehat U(\theta)|^2d\theta,\qquad\widehat U^{\,n}=G(\theta)^n\widehat U^{\,0}.
$$

Thus a scalar mode bound gives an exact [discrete L2 norm](../../../../../discrete-l2-norm.md) bound. Stability on a fixed physical interval requires constants independent of the refining spatial and time meshes:

$$
\boxed{\sup_{nk\leq T}\sup_\theta|G_{h,k}(\theta)|^n\leq C_T.}
$$

The contraction condition $|G|\leq1$ is sufficient and customary for equations whose exact solutions do not grow. More generally $|G|\leq1+Ck$ suffices, since $(1+Ck)^n\leq e^{CT}$. At a fixed [Courant number](../../../../../courant-number.md), when $G$ is independent of $k$, a mode with modulus strictly greater than one violates the estimate as $n\sim T/k\to\infty$. One must keep this scaling: physical growth such as $e^{\kappa t}$ does not by itself mean finite-time numerical instability. This is [finite-time stability versus power boundedness](../../../../../finite-time-stability-versus-power-boundedness.md).

For systems, the symbol is an amplification matrix. The requirement is a uniform bound on all its powers, not merely its [eigenvalues](../../../../../eigenvalue.md). A unit-modulus [Jordan block](../../../../../jordan-block.md) $\begin{pmatrix}1&1\\0&1\end{pmatrix}$ has powers $\begin{pmatrix}1&n\\0&1\end{pmatrix}$ and is unstable under refinement. A uniformly conditioned eigenbasis or an energy estimate can justify a modal conclusion; eigenvalues alone cannot control a general [nonnormal matrix](../../../../../non-normal-matrix.md). Multilevel schemes likewise produce an [amplification polynomial of a multilevel finite difference scheme](../../../../../amplification-polynomial-of-a-multilevel-finite-difference-scheme.md), with a uniform root condition and control of starting errors. Repeated unit-modulus roots can give polynomial growth, and roots approaching each other require attention to mesh-uniform constants.

Several elementary examples show how the calculation works. For $u_t+c u_x=0$ with $c>0$, forward Euler with centered spatial differences gives $G=1-i\mu\sin\theta$, where $\mu=ck/h$. Since $|G|^2=1+\mu^2\sin^2\theta$, it is unstable at every fixed nonzero Courant number. The [upwind finite difference scheme](../../../../../upwind-finite-difference-scheme.md) instead gives $G=1-\mu+\mu e^{-i\theta}$ and

$$
|G|^2=1-4\mu(1-\mu)\sin^2(\theta/2),
$$

so its exact contraction range is $0\leq\mu\leq1$. The [Lax-Wendroff advection scheme](../../../../../lax-wendroff-advection-scheme.md) has $G=1-i\mu\sin\theta+\mu^2(\cos\theta-1)$; expansion gives $|G|^2=1-4\mu^2(1-\mu^2)\sin^4(\theta/2)$, hence $|\mu|\leq1$. The [Courant–Friedrichs–Lewy condition](../../../../../courant-friedrichs-lewy-condition.md) relates these restrictions to the numerical domain of dependence, but is a necessary geometric check rather than a complete stability proof. Implicit schemes can have a global spatial dependence and different Courant ranges, as Question 3 illustrates.

For the [heat equation](../../../../../heat-equation.md) $u_t=\nu u_{xx}$, put $r=\nu k/h^2$. Central spatial differences with forward Euler give $G=1-4r\sin^2(\theta/2)$, so $0\leq r\leq1/2$. With backward Euler the factor is $[1+4r\sin^2(\theta/2)]^{-1}$, a contraction for every $r\geq0$. For the [Crank-Nicolson diffusion scheme](../../../../../crank-nicolson-diffusion-scheme.md) it is $[1-2r\sin^2(\theta/2)]/[1+2r\sin^2(\theta/2)]$, again a contraction for all $r\geq0$. At large $r$, however, high-frequency factors approach minus one rather than zero: unconditional stability does not imply strong damping or accurate resolution of every mode.

The connection with convergence is the [Lax equivalence theorem](../../../../../lax-equivalence-theorem.md) for a consistent approximation to a well-posed linear evolution problem. Its forward implication follows directly from the error recursion. If $e^{n+1}=G_h e^n+k\tau^n$ and $\|G_h^j\|\leq C_T$ for $jk\leq T$, then

$$
\|e^n\|\leq C_T\|e^0\|+C_Tk\sum_{j=0}^{n-1}\|\tau^j\|\leq C_T\|e^0\|+C_TT\max_j\|\tau^j\|.
$$

A convergent initialization and a vanishing normalized [local truncation error](../../../../../local-truncation-error.md) therefore give convergence. Smooth-data consistency can be extended by density when the approximation and initialization are uniformly bounded. For rough $L^2$ data, cell averages or another [L2-compatible initialization of grid data](../../../../../l2-compatible-initialization-of-grid-data.md) are preferable to undefined point samples. A high formal order does not rescue an unstable amplification operator.

Boundary conditions determine whether Fourier diagonalization is exact. On a periodic grid the update is a [circulant matrix](../../../../../circulant-matrix.md), and the finite [discrete Fourier transform](../../../../../discrete-fourier-transform.md) diagonalizes it at the frequencies $2\pi\ell/N$. Here an interior symbol controls the entire scheme, including the wrapping boundary. On the whole line, the continuous frequency transform serves the same purpose and there is no boundary closure to check.

For a finite interval with homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), centered diffusion is a symmetric tridiagonal problem diagonalized by discrete sine modes. One tests the same diffusion symbol at the admitted sine frequencies, not at arbitrary periodic modes. For homogeneous [Neumann boundary conditions](../../../../../neumann-boundary-condition.md), a suitable reflected closure uses discrete cosine modes; the constant mode is present and is neutral for pure diffusion. With the standard reflected endpoint stencil, the natural norm uses half endpoint weights, in which the matrix is self-adjoint. Consequently stable diffusion need not make every solution tend to zero under Neumann conditions. These special orthogonal bases supply an exact substitute for Fourier modes when the operator and closure have the required symmetry.

For transport, prescribe only the incoming physical boundary data. With $u_t+c u_x=0$, $c>0$, the inflow is the left endpoint; for $u_t=u_x$ it is the right endpoint. Imposing unrelated data at both ends generally overdetermines the first-order PDE. Outflow rows or ghost points must be chosen compatibly with the interior method. A general [boundary closure of a difference scheme](../../../../../boundary-closure-of-a-difference-scheme.md) destroys the circulant structure, so whole-line [von Neumann stability analysis](../../../../../von-neumann-stability-analysis.md) is necessary in many settings but not sufficient for the full initial-boundary problem. A defective boundary row that doubles one boundary unknown each step can create growth even beside a stable interior stencil.

A more refined boundary calculation seeks half-line modes $U_j^n=w^n\zeta^j$ with $|\zeta|<1$; these are localized near the boundary. Insert them into both the interior recurrence and boundary equations. A compatible mode with $|w|>1$ proves boundary instability. Absence of one isolated growing mode is not the whole theorem: weakly controlled limiting modes can still destroy a uniform estimate. The [Uniform Kreiss--Lopatinskii condition](../../../../../uniform-kreiss-lopatinskii-condition.md) requires a uniformly bounded inverse boundary system on the incoming/decaying mode space. Direct energy estimates are often a clearer alternative to solving that transformed boundary problem.

For example, suppose a first-derivative matrix obeys the [discrete summation by parts](../../../../../discrete-summation-by-parts.md) identity $HD+D^TH=e_Ne_N^T-e_0e_0^T$, with positive norm matrix $H$. The semidiscrete advection equation $U_t=-cDU$ then gives

$$
\frac d{dt}(U^THU)=-c(U_N^2-U_0^2).
$$

With homogeneous inflow $U_0=0$ and $c>0$, only a nonpositive outflow term remains; prescribed inflow contributes a controlled forcing term. This is the [inflow advection energy estimate from summation by parts](../../../../../inflow-advection-energy-estimate-from-summation-by-parts.md), and it tests the boundary as part of the operator. For a dissipative semidiscrete matrix $A$, backward Euler also preserves the estimate, because its update gives

$$
\|U^{n+1}\|_H^2-\|U^n\|_H^2=2k\langle U^{n+1},AU^{n+1}\rangle_H-\|U^{n+1}-U^n\|_H^2\leq0.
$$

This distinguishes spatial energy stability from stability of an arbitrary chosen time integrator.

Finally, nonhomogeneous boundaries can be homogenized by subtracting a suitable lifting, leaving a forced equation whose solution needs a bound in terms of both initial and boundary data. Variable coefficients and nonuniform grids remove translation invariance, so freezing coefficients gives only local diagnostic information. A full [energy method](../../../../../energy-method.md), a mesh-uniform operator estimate, or a dedicated boundary-symbol analysis is then needed. **Fourier symbols give complete stability tests when an orthogonal mode decomposition diagonalizes the full operator; otherwise the boundaries, matrix powers and norm estimates must be checked as well.**

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
