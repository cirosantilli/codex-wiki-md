<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

**[Eigenvalue](../../../../../eigenvalue.md) analysis proves mesh-uniform stability when it is accompanied by control of [eigenvectors](../../../../../eigenvector.md) or an energy norm; the signs of [eigenvalues](../../../../../eigenvalue.md) alone are insufficient.** For an evolution equation, the [method of lines](../../../../../method-of-lines.md) first produces $u_h'=L_hu_h$. A time integrator then gives an amplification [matrix](../../../../../matrix.md) $S_{h,\delta}$, for example $S_{h,\delta}=R(\delta L_h)$ for a [Runge-Kutta method](../../../../../runge-kutta-method.md). The useful stability requirement on a fixed physical time interval is

$$
\sup_{n\delta\le T}\|S_{h,\delta}^n\|_h\le C_T,
$$

where $C_T$ is independent of the refining spatial and temporal meshes. The semidiscrete analogue is $\|e^{tL_h}\|_h\le C_T$ for $0\le t\le T$. These are bounds on propagation of initial errors and residuals, not merely statements that each finite [matrix](../../../../../matrix.md) has a bounded solution over its own finite time interval.

If $L_h$ is a [normal matrix](../../../../../normal-matrix.md) in the chosen discrete [inner product](../../../../../inner-product.md), it has a unitary eigenbasis. Then

$$
\|e^{tL_h}\|_h=\max_j e^{t\operatorname{Re}\lambda_j},\qquad
\|R(\delta L_h)^n\|_h=\max_j|R(\delta\lambda_j)|^n.
$$

For dissipative problems it is sufficient that every $\delta\lambda_j$ lie in the integrator's [linear stability domain](../../../../../linear-stability-domain.md). A diagonalizable family also suffices if its [eigenvector](../../../../../eigenvector.md) matrices have uniformly bounded [condition numbers](../../../../../condition-number.md): the same maximum is multiplied by $\|V_h\|\|V_h^{-1}\|$. Without that uniform bound the argument does not establish mesh stability. For finite-time estimates, an amplification modulus $1+O(\delta)$ can also be acceptable; strict contraction at every step is a stronger property.

For a constant-coefficient stencil on the full lattice or a periodic grid, [von Neumann stability analysis](../../../../../von-neumann-stability-analysis.md) provides the [eigenvectors](../../../../../eigenvector.md) explicitly. A [Fourier mode](../../../../../fourier-mode.md) diagonalizes each translation-invariant spatial difference, giving a scalar symbol $\lambda_h(\theta)$ or a small [matrix](../../../../../matrix.md) symbol for a system. The [discrete Fourier transform](../../../../../discrete-fourier-transform.md) and [Parseval identity](../../../../../parseval-identity.md) turn a uniform modal bound into an actual discrete [L2 norm](../../../../../l2-norm.md) bound. The two-dimensional stencil in question 3 has $\operatorname{Re}\lambda_h=-(1-\cos\eta)^2/h\le0$, so its continuous-time amplification is contractive; a later time integrator must still be checked. With boundaries one must analyze the boundary rows as well: a whole-line [Fourier symbol](../../../../../fourier-symbol-of-a-difference-operator.md) cannot detect an unstable boundary closure.

For the heat equation $u_t=\kappa u_{xx}$ on a unit interval with zero Dirichlet data, the centred second difference has a sine eigenbasis and [eigenvalues](../../../../../eigenvalue.md)

$$
\lambda_j=-\frac{4\kappa}{h^2}\sin^2\frac{j\pi}{2N},\qquad h=1/N,\quad 1\le j<N.
$$

[Explicit Euler method](../../../../../euler-method.md) multiplies mode $j$ by $1+\delta\lambda_j$. Requiring all factors to have modulus at most one yields $\kappa\delta/h^2\le1/[2\sin^2((N-1)\pi/(2N))]$ on a given grid, and the sharp grid-independent sufficient limit is

$$
\boxed{\kappa\delta/h^2\le\tfrac12\quad\text{in one dimension},
\qquad \kappa\delta/h^2\le\tfrac14\quad\text{on the standard equal-mesh two-dimensional grid}.}
$$

These parabolic time-step restrictions express the growth of the largest-magnitude diffusion [eigenvalue](../../../../../eigenvalue.md) like $h^{-2}$. [Backward Euler method](../../../../../backward-euler-method.md) instead has factor $(1-\delta\lambda_j)^{-1}$ and the [Crank-Nicolson method](../../../../../crank-nicolson-method.md) factor $(1+\delta\lambda_j/2)/(1-\delta\lambda_j/2)$, both bounded by one for every $\delta\ge0$. Their unconditional stability follows from [A-stability](../../../../../a-stability.md), with much stronger damping of the shortest scales for backward Euler.

For $u_t=-a u_x$, $a>0$, explicit time stepping with a backward spatial difference gives

$$
S(\theta)=1-\nu+\nu e^{-i\theta},\qquad \nu=a\delta/h,
\qquad |S(\theta)|^2=1-2\nu(1-\nu)(1-\cos\theta).
$$

Thus the [upwind finite difference scheme](../../../../../upwind-finite-difference-scheme.md) is contractive exactly for $0\le\nu\le1$, a [Courant–Friedrichs–Lewy condition](../../../../../courant-friedrichs-lewy-condition.md) matching the direction and speed of information propagation. A centred spatial difference has purely imaginary [eigenvalues](../../../../../eigenvalue.md), and forward Euler gives $|S|^2=1+\nu^2\sin^2\theta>1$. Under a fixed positive hyperbolic Courant number, high-frequency data grow by a fixed factor in each of $O(1/h)$ steps, proving instability as the mesh is refined. This is not a claim that no exceptionally small coupled step can ever give a finite-time bound: if $\delta=O(h^2)$, the excess per step is only $O(\delta)$, but the usual hyperbolic scaling is unstable. Higher-order explicit integrators can possess nontrivial imaginary-axis stability intervals and are then suitable for skew-adjoint advection or the energy-form first-order wave equation.

Variable coefficients usually prevent Fourier diagonalization, but may preserve a [self-adjoint](../../../../../self-adjoint-operator.md) spatial operator. The positive-face diffusion discretization in question 5 is an example. Its discrete energy identity makes $A+B$ symmetric negative definite, so a unitary eigenbasis still exists even without a closed [eigenvalue](../../../../../eigenvalue.md) formula. More generally, a [dissipative operator](../../../../../dissipative-operator.md) $L_h$ in a discrete energy [inner product](../../../../../inner-product.md) obeys

$$
\frac d{dt}\|u_h\|_h^2=2\operatorname{Re}\langle L_hu_h,u_h\rangle_h\le0,
$$

which directly proves a uniform semigroup estimate. The [dissipative Cayley-transform contraction](../../../../../dissipative-cayley-transform-contraction.md) also follows without normality: for $\alpha\ge0$,

$$
\|(I+\alpha L_h)v\|_h^2-\|(I-\alpha L_h)v\|_h^2
=4\alpha\operatorname{Re}\langle L_hv,v\rangle_h\le0.
$$

Taking $v=(I-\alpha L_h)^{-1}u$ proves contraction of the Crank–Nicolson factor. The [contractivity of split Crank-Nicolson diffusion](../../../../../contractivity-of-split-crank-nicolson-diffusion.md) then follows from multiplying two contraction bounds; simultaneous [eigenvectors](../../../../../eigenvector.md) of the two directional matrices are unnecessary.

The [negative spectra do not imply uniform semidiscrete stability](../../../../../negative-spectra-do-not-imply-uniform-semidiscrete-stability.md) example shows what can go wrong. Let

$$
L_h=\begin{pmatrix}-1&h^{-1}\\0&-1\end{pmatrix},\qquad
 e^{tL_h}=e^{-t}\begin{pmatrix}1&t/h\\0&1\end{pmatrix}.
$$

Both [eigenvalues](../../../../../eigenvalue.md) are $-1$ for every mesh, but applying the propagator to the second unit vector at $t=1$ gives norm at least $1/(eh)$. The evolution is therefore not mesh-uniformly stable. For a discrete [matrix](../../../../../matrix.md), a unit-modulus [eigenvalue](../../../../../eigenvalue.md) with a nontrivial [Jordan block](../../../../../jordan-block.md) gives powers growing polynomially in the step number. Even strictly interior [eigenvalues](../../../../../eigenvalue.md) can allow large transient growth when [eigenvectors](../../../../../eigenvector.md) are badly conditioned. A [pseudospectrum](../../../../../pseudospectrum.md) or [numerical range of an operator](../../../../../numerical-range-of-an-operator.md), and especially a direct energy estimate, can reveal behavior missed by [eigenvalues](../../../../../eigenvalue.md).

A [resolvent](../../../../../resolvent-of-an-operator.md) estimate provides another way to see the needed uniformity. If $\|S_h^n\|\le C$ for every $n$, then for $|z|>1$,

$$
(zI-S_h)^{-1}=\sum_{n=0}^{\infty}\frac{S_h^n}{z^{n+1}},\qquad
\|(zI-S_h)^{-1}\|\le\frac{C}{|z|-1}.
$$

This shows directly that a uniform power estimate imposes more than the location of the spectrum. Conversely, resolvent-to-power estimates in varying dimension must themselves be uniform; a bound with constants depending on the number of grid points is not enough.

For a [linear multistep method](../../../../../linear-multistep-method.md), each spatial [eigenvalue](../../../../../eigenvalue.md) gives an amplification [polynomial](../../../../../polynomial-split.md), and all roots must satisfy the [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md), including simplicity of any unit-modulus root. Merely following the root approximating $e^{\delta\lambda}$ misses parasitic modes. The temporal and spatial analyses must therefore be combined with the appropriate [zero-stability](../../../../../zero-stability.md) and uniform modal bounds.

Finally stability connects to convergence. If the exact grid samples have normalized residual $\tau^n$ and the error obeys $e^{n+1}=S_he^n+\delta\tau^n$, iteration gives

$$
\|e^n\|_h\le C_T\left(\|e^0\|_h+\delta\sum_{j<n}\|\tau^j\|_h\right).
$$

A residual tending uniformly to zero then gives convergence on $[0,T]$. For a well-posed linear initial-value problem and a consistent linear finite-difference approximation, this is the forward implication of the [Lax equivalence theorem](../../../../../lax-equivalence-theorem.md). The practical conclusion is to analyze the full operator including boundaries, select a time method whose stability region contains the relevant scaled spectrum, and verify that [eigenvectors](../../../../../eigenvector.md) or an energy estimate make the resulting bounds uniform as the grid is refined.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
