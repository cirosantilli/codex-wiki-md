<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

A spatial [finite difference method](../../../../../finite-difference-method.md) and time discretization for a linear evolution problem give a recurrence $U^{n+1}=B_{h,k}U^n$. To obtain [numerical stability](../../../../../stability-of-a-numerical-method.md) on $0\le nk\le T$, one needs a bound $\|B_{h,k}^n\|\le C_T$ uniform in the permitted grid sizes and time steps. More generally a growth estimate $\|B_{h,k}^n\|\le C e^{c nk}$ is sufficient. The [finite-time stability versus power boundedness](../../../../../finite-time-stability-versus-power-boundedness.md) distinction matters: growth per step of $1+O(k)$ can be compatible with the latter finite-time estimate, whereas unrestricted geometric growth at a fixed [Courant number](../../../../../courant-number.md) is not.

The eigenvalue method diagonalizes $B_{h,k}$ into modes. If $B_{h,k}$ is a [normal matrix](../../../../../normal-matrix.md), the [spectral theorem](../../../../../spectral-theorem.md) gives $\|B_{h,k}^n\|_2=\max_j|\mu_j|^n$. Thus $|\mu_j|\le1$ gives contraction, and $|\mu_j|\le e^{ck}$ gives the preceding growth estimate. A [diagonalizable matrix](../../../../../diagonalizable-matrix.md) $B=V\Lambda V^{-1}$ has $\|B^n\|_2\le\|V\|_2\|V^{-1}\|_2\max_j|\mu_j|^n$, so its [condition number](../../../../../condition-number.md) must remain bounded uniformly as the mesh changes. A stable-looking list of [eigenvalues](../../../../../eigenvalue.md) alone is insufficient.

Indeed,

$$
B=\begin{pmatrix}1&1\\0&1\end{pmatrix},\qquad B^n=\begin{pmatrix}1&n\\0&1\end{pmatrix}.
$$

Both [eigenvalues](../../../../../eigenvalue.md) are one, but the [Jordan block](../../../../../jordan-block.md) gives growth proportional to $n\sim T/k$, violating uniform finite-time [numerical stability](../../../../../stability-of-a-numerical-method.md). A [nonnormal Fourier amplification matrix](../../../../../nonnormal-fourier-amplification-matrix.md) can similarly exhibit large amplification even with its [eigenvalues](../../../../../eigenvalue.md) inside the [unit disk](../../../../../unit-disk.md). [Eigenvector](../../../../../eigenvector.md) conditioning and the full powers of the amplification operator are essential.

For constant-coefficient schemes on a periodic or infinite grid, a [Fourier transform](../../../../../fourier-transform.md) diagonalizes scalar translation-invariant stencils. This yields [von Neumann stability analysis](../../../../../von-neumann-stability-analysis.md) using the [Fourier amplification symbol](../../../../../fourier-amplification-symbol.md) $G(\theta)$. The [discrete Parseval identity](../../../../../discrete-parseval-identity.md) turns a bound on $G(\theta)^n$ into a discrete [L2 norm](../../../../../l2-norm.md) estimate. For systems, the symbol is a [matrix](../../../../../matrix.md); a [uniform power bound for matrix Fourier symbols](../../../../../uniform-power-bound-for-matrix-fourier-symbols.md) is required, rather than a bound on its [spectral radius](../../../../../spectral-radius.md) alone.

For the [heat equation](../../../../../heat-equation.md), a [central finite difference](../../../../../central-finite-difference.md) in space and the [explicit Euler method](../../../../../euler-method.md) in time give

$$
G(\theta)=1-4r\sin^2(\theta/2),\qquad r=k/h^2.
$$

The scalar condition $|G|\le1$ for every frequency is exactly **$0\le r\le1/2$**. With zero [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), the spatial [matrix](../../../../../matrix.md) is [symmetric](../../../../../symmetric-relation.md) and diagonalized by sine modes, leading to the same uniform sufficient restriction. By contrast, the [Backward Euler diffusion scheme](../../../../../backward-euler-diffusion-scheme.md) has $G(\theta)=[1+4r\sin^2(\theta/2)]^{-1}$ and is stable for every $r\ge0$.

For the [advection equation](../../../../../transport-equation.md) $u_t+a u_x=0$, $a>0$, centered space with the [explicit Euler method](../../../../../euler-method.md) gives $G=1-i\nu\sin\theta$, $\nu=ak/h$, and $|G|^2=1+\nu^2\sin^2\theta$. At fixed positive [Courant number](../../../../../courant-number.md), repeated powers are unbounded as the mesh is refined. The [upwind finite difference scheme](../../../../../upwind-finite-difference-scheme.md) instead has

$$
G=1-\nu+\nu e^{-i\theta},\qquad |G|^2=1-2\nu(1-\nu)(1-\cos\theta),
$$

which gives contraction precisely for **$0\le\nu\le1$**. This comparison shows why the spatial stencil and time method must be analyzed together.

Boundary treatment can destroy the normality or mode decomposition available on a periodic grid, so a finite-interval scheme needs its own uniform operator estimate. Multilevel time schemes likewise require the [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md) and uniform bounds for the associated amplification matrices; simple scalar root tests do not establish these bounds for arbitrary systems. Once [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md), a well-posed linear evolution problem and the required [numerical stability](../../../../../stability-of-a-numerical-method.md) estimate hold, the [Lax equivalence theorem](../../../../../lax-equivalence-theorem.md) gives [numerical convergence](../../../../../convergence-of-a-numerical-method.md). Eigenvalues provide a powerful route to that estimate when the accompanying eigenvector and boundary analysis is justified.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
