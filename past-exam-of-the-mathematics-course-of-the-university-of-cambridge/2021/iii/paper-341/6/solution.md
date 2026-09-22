<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Stability asks whether perturbations already present in data, arithmetic, or an earlier numerical step remain controlled under subsequent evolution. It complements [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md): consistency says that an exact smooth solution nearly satisfies one numerical step, while stability prevents the accumulated local defects from being amplified without bound. For a well-posed differential equation these two properties are what make convergence possible.

For a [linear multistep method](../../../../../linear-multistep-method.md), zero-stability concerns the limit $h\to0$. The roots of its first characteristic polynomial must lie in the closed unit disk, and every root on the unit circle must be simple. The [Dahlquist equivalence theorem](../../../../../dahlquist-equivalence-theorem.md) states that a consistent linear multistep method converges precisely when it is zero-stable. The parasitic root $5/11$ in Question 1 decays, whereas a repeated root at $1$ would turn small defects into secular growth.

Absolute stability instead fixes $z=h\lambda$ for the [Dahlquist test equation](../../../../../dahlquist-test-equation.md). A one-step method has amplification factor $R(z)$ and absolute-stability region

$$
\mathcal S=\{z:|R(z)|\leq1\}.
$$

A-stability means that $\mathcal S$ contains the entire closed left half-plane, matching every decaying scalar linear problem. [L-stability](../../../../../l-stability.md) additionally requires $R(z)\to0$ as $z\to-\infty$, which suppresses unresolved fast transients in a [stiff differential equation](../../../../../stiff-equation.md). Backward Euler is L-stable; the trapezoidal rule is A-stable but approaches $-1$ and can retain stiff oscillations; forward Euler is stable only in the disk $|1+z|\leq1$.

For nonlinear dissipative systems, scalar absolute stability can be insufficient. B-stability controls distances between numerical solutions of contractive differential equations. For Runge–Kutta methods, algebraic stability—nonnegative weights and positive semidefiniteness of $BA+A^TB-bb^T$—is a useful sufficient condition for B-stability. Question 2 shows how a single negative diagonal entry disproves it.

After spatial discretization of a partial differential equation, stability can be studied through the semidiscrete matrix. If its Hermitian part is nonpositive, the [energy method](../../../../../energy-method.md) proves contractivity without diagonalizing it. A skew-Hermitian generator instead conserves norm, as in the discrete Schrodinger problem of Question 3. Eigenvalues alone can be misleading for a [non-normal matrix](../../../../../non-normal-matrix.md): transient growth may be large even when every eigenvalue lies in the left half-plane, so matrix norms, logarithmic norms, resolvent bounds, or a [pseudospectrum](../../../../../pseudospectrum.md) may be needed.

For constant-coefficient Cauchy problems, [von Neumann stability analysis](../../../../../von-neumann-stability-analysis.md) inserts Fourier modes and bounds their amplification factors. Question 4 gives a typical result: centered diffusion contributes a negative real symbol and centered advection an imaginary symbol. Semidiscrete evolution is stable, yet forward Euler imposes both the parabolic restriction $\Delta t=O(\Delta x^2)$ and an advection-diffusion restriction. This illustrates a [Courant–Friedrichs–Lewy condition](../../../../../courant-friedrichs-lewy-condition.md): a stable spatial approximation need not remain stable under an arbitrary time stepper.

For a well-posed linear initial-value problem and a consistent finite-difference approximation, the [Lax equivalence theorem](../../../../../lax-equivalence-theorem.md) identifies stability with convergence. Its hypotheses matter: it does not by itself cover nonlinear equations, inconsistent boundary closures, changing norms, or non-smooth solutions. Boundaries also defeat a naive whole-line Fourier argument; an energy estimate, normal-mode boundary analysis, or a discrete semigroup bound must include the boundary treatment.

Practical stability analysis therefore starts from the structure of the differential equation. Conservation laws favor unitary or symplectic methods, diffusion favors A- or L-stable implicit methods, monotone transport may require strong-stability-preserving time stepping and upwind fluxes, and stiff splitting requires attention to both the factors and their commutators. Stability does not guarantee accuracy: a heavily damped method may be stable while erasing the solution, and a stable computation with $h\lambda$ near the edge of its stability region may have an unacceptable phase error.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 341](../../paper-341-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
