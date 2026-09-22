<h1 id="section-b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Consider first a scalar constant-coefficient [Cauchy problem for a partial differential equation](../../../../../../cauchy-problem.md) on the whole line. A translation-invariant spatial discretization is a convolution operator, so the [discrete Fourier transform](../../../../../../discrete-fourier-transform.md) turns it into multiplication by its Fourier symbol. This reduction is exact because Fourier modes are the simultaneous generalized eigenfunctions of every translation-invariant stencil.

For a fully discrete one-step method

$$
u^{n+1}=Q_hu^n,
$$

write $H_h(\theta)$ for its [amplification factor](../../../../../../amplification-factor.md). The [Parseval identity](../../../../../../parseval-identity.md) gives

$$
\|Q_h^nu^0\|_2^2
=\int_{-\pi}^{\pi}|H_h(\theta)|^{2n}|\widehat u^0(\theta)|^2\,d\theta.
$$

Consequently the exact necessary and sufficient condition for stability on every bounded time interval $0\leq n\Delta t\leq T$ is

$$
\boxed{\operatorname*{ess\,sup}_\theta|H_h(\theta)|
\leq e^{C\Delta t}}
$$

with $C$ independent of the mesh. Sufficiency follows directly from Parseval; necessity follows by choosing transformed initial data concentrated where the multiplier is largest. For a contractive scheme one can take $C=0$, yielding the familiar [von Neumann stability analysis](../../../../../../von-neumann-stability-analysis.md) condition $|H_h(\theta)|\leq1$.

For a semidiscretization $u_t=A_hu$ with scalar symbol $a_h(\theta)$, the corresponding exact criterion is

$$
\boxed{\operatorname*{ess\,sup}_\theta\operatorname{Re}a_h(\theta)\leq C.}
$$

Indeed, the Fourier multiplier of the solution operator is $e^{ta_h(\theta)}$. For systems, eigenvalues alone cease to be sufficient when the matrix symbol is [non-normal](../../../../../../non-normal-matrix.md); the necessary and sufficient statement is the uniform bound $\|e^{tA_h(\theta)}\|\leq C_T$.

On the whole lattice, a finite stencil defines a [Laurent operator](../../../../../../laurent-operator.md), whose operator norm is the essential supremum of its symbol. Restricting the same stencil to a half-line gives a [Toeplitz operator](../../../../../../toeplitz-operator.md). The Cauchy symbol condition remains necessary for a stable initial-boundary scheme because data localized far from the boundary behave like the whole-line problem for a finite time. It is not sufficient: the boundary closure can support growing modes or amplify incoming modes even when every interior Fourier mode is stable.

Boundary stability therefore requires a uniform estimate for the forced half-line recurrence. After a Laplace transform in time and a Fourier transform in tangential variables, one solves a normal-direction recurrence. The [Uniform Kreiss--Lopatinskii condition](../../../../../../uniform-kreiss-lopatinskii-condition.md) requires the boundary equations to determine its decaying roots with a uniformly bounded inverse. In practical terms, one imposes one independent boundary condition for each incoming characteristic or numerical mode and none for outgoing modes. The [group velocity](../../../../../../group-velocity.md) $d\omega/dk$ identifies the direction in which a narrow [wave packet](../../../../../../wave-packet.md) carries energy, so its sign helps determine which boundary is inflow and explains why a numerically generated high-frequency branch can require a boundary condition different from that suggested by its phase velocity.

For a two-step method, the Fourier substitution produces an [amplification polynomial of a multilevel finite difference scheme](../../../../../../amplification-polynomial-of-a-multilevel-finite-difference-scheme.md). Every root must lie in the closed unit disk, and unit-modulus roots must be simple, uniformly in the wavenumber. For example, leapfrog differencing of $u_t+cu_x=0$ gives

$$
u_j^{n+1}=u_j^{n-1}-\nu(u_{j+1}^n-u_{j-1}^n),
\qquad \nu=\frac{c\Delta t}{\Delta x},
$$

and hence

$$
G^2+2i\nu\sin\theta\,G-1=0.
$$

The roots have unit modulus when $|\nu\sin\theta|\leq1$, giving the usual [Courant](../../../../../../courant-number.md) restriction $|\nu|\leq1$. At the endpoint, a wavenumber with $|\nu\sin\theta|=1$ produces a repeated unit root and violates the uniform root condition; strict $|\nu|<1$ avoids this marginal linear growth. The second root is the familiar oscillatory computational mode, illustrating why a multilevel scheme requires its full amplification polynomial rather than a single multiplier.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [Section B](../../section-b.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
