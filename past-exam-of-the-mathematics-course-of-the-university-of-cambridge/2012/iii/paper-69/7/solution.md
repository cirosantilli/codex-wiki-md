<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

[Fourier stability analysis](../../../../../fourier-stability-analysis.md) applies most directly to linear, constant-coefficient evolution schemes on uniform infinite or periodic grids. Translation invariance makes spatial shifts diagonal in [discrete Fourier modes](../../../../../discrete-fourier-mode.md). If a one-step scheme has $U^{n+1}=\sum_j A_jU^n_{m+j}$, substituting $U_m^n=\widehat U^n(\theta)e^{im\theta}$ gives the [Fourier amplification symbol](../../../../../fourier-amplification-symbol.md)

$$
\widehat U^{n+1}(\theta)=G(\theta)\widehat U^n(\theta),
\qquad G(\theta)=\sum_jA_je^{ij\theta}.
$$

The [discrete Parseval identity](../../../../../discrete-parseval-identity.md) identifies the discrete [L2 norm](../../../../../l2-norm.md) with the squared norm of Fourier coefficients. Uniform stability on a fixed time interval means a mesh-independent bound on $\|G(\theta)^n\|$ for all frequencies and $n\Delta t\leq T$. In the scalar case $|G|\leq1$ yields contraction. More generally $|G|\leq1+C\Delta t$ gives the bound $e^{CT}$ and is consistent with a continuously growing well-posed equation. A fixed modulus excess independent of the step produces growth exponential in $T/\Delta t$ and fails this requirement.

For systems, eigenvalue moduli alone are insufficient. The [uniform power bound for matrix Fourier symbols](../../../../../uniform-power-bound-for-matrix-fourier-symbols.md) also controls eigenvector conditioning and Jordan growth. For example $G=\begin{pmatrix}1&1\\0&1\end{pmatrix}$ has only unit eigenvalues but $G^n=\begin{pmatrix}1&n\\0&1\end{pmatrix}$, unbounded as $\Delta t\to0$ at fixed $T$. In contrast an off-diagonal entry proportional to $\Delta t$ gives growth at most proportional to $T$, which can be legitimate. A uniformly conditioned diagonalization is a sufficient reduction to scalar modal bounds; [nonnormal matrices](../../../../../non-normal-matrix.md) require direct power or energy estimates. Multilevel schemes similarly require the root condition for their frequency-dependent amplification polynomial and a uniform bound on the associated companion evolution, including limiting repeated-root cases.

The simplest parabolic example is the [Forward Euler method](../../../../../euler-method.md) with centered spatial diffusion. For $\mu=\Delta t/h^2$,

$$
G(\theta)=1-4\mu\sin^2(\theta/2),
\qquad \boxed{0\leq\mu\leq\tfrac12}
$$

is the sharp mesh-uniform contraction range. For the [theta method](../../../../../theta-method.md), $G=[1-4(1-a)\mu\sin^2(\theta/2)]/[1+4a\mu\sin^2(\theta/2)]$, giving unconditional contraction at $a\geq1/2$. Implicit stability permits larger steps, but accuracy still constrains them, and the [Crank-Nicolson method](../../../../../crank-nicolson-method.md) does not strongly damp high-frequency rough data.

For advection $u_t+cu_x=0$ with $c>0$, the [upwind finite difference scheme](../../../../../upwind-finite-difference-scheme.md) gives

$$
G=1-\nu(1-e^{-i\theta}),\qquad
|G|^2=1-4\nu(1-\nu)\sin^2(\theta/2),
\quad \nu=c\Delta t/h.
$$

Thus $0\leq\nu\leq1$ is its contraction range. The [Lax-Friedrichs scheme](../../../../../lax-friedrichs-method.md) has $G=\cos\theta-i\nu\sin\theta$ and is contractive exactly when $|\nu|\leq1$. These express a [Courant–Friedrichs–Lewy condition](../../../../../courant-friedrichs-lewy-condition.md): the numerical domain of dependence must encompass the physical one for convergence. That necessary condition is not sufficient by itself. Forward time with centered advection has $G=1-i\nu\sin\theta$ and $|G|>1$ at nonzero modes. At a fixed nonzero Courant number it is unstable even if $|\nu|\leq1$. Under the much stronger refinement $\Delta t=O(h^2)$, however, its powers remain bounded on fixed time intervals; the [centered-advection refinement-dependent stability](../../../../../centered-advection-refinement-dependent-stability.md) must not be confused with the usual hyperbolic-step instability.

Symbols also quantify dispersion and dissipation. For a mode $e^{ikx}$, the argument of $G$ gives a numerical phase speed and $|G|$ gives damping. Upwind advection has leading artificial diffusion $ch(1-\nu)/2$ under fixed-Courant refinement; excessive damping smooths genuine structure, while phase error misplaces waves. Stability controls boundedness, not either error by itself. Smooth low-frequency [Taylor expansions](../../../../../taylor-expansion.md) establish consistency; high-frequency modal bounds establish stability, so analyzing only fixed physical wavenumbers can miss grid-scale instabilities.

For a well-posed linear initial-value problem, the [Lax equivalence theorem](../../../../../lax-equivalence-theorem.md) makes consistency plus a uniform stability estimate equivalent to convergence in the chosen norm. Boundaries and variable coefficients need extra care: Fourier diagonalization no longer handles the full update, and an interior or frozen-coefficient symbol does not prove boundary or global stability. Boundary energy estimates, a suitable matrix analysis or a separate boundary-stability argument must supplement it. Nonlinear schemes also require controls beyond this linear symbol test. These limitations delimit what the method proves rather than reducing its usefulness: in its proper setting, it turns an arbitrarily large grid evolution into exact and interpretable modal algebra.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [Section II](../section-ii.md)
3. [Paper 69](../../paper-69-split.md)
4. [Iii](../../split.md)
5. [2012](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
