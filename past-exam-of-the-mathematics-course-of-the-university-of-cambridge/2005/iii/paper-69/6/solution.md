<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For constant-coefficient evolution on an infinite or periodic grid, spatial [Fourier stability analysis](../../../../../fourier-stability-analysis.md) reduces a multidimensional recurrence to independent modal problems. This gives exact L2 [stability](../../../../../stability-of-a-numerical-method.md) results when the coefficients and geometry admit that reduction; it also exposes high-frequency restrictions which a truncation-error calculation alone misses.

Consider a scalar one-step update $(S_{h,k}U)_j=\sum_\ell a_\ell U_{j+\ell}$ on $\mathbb Z^d$. With $\widehat U(\theta)=\sum_jU_je^{-ij\cdot\theta}$, its symbol is $G(\theta)=\sum_\ell a_\ell e^{i\ell\cdot\theta}$ and $\widehat U^{,n}=G^n\widehat U^0$. [Parseval identity](../../../../../parseval-identity.md) gives

$$
\|U\|_h^2=\frac{h^d}{(2\pi)^d}\int_{[-\pi,\pi]^d}|\widehat U(\theta)|^2d\theta,
\qquad \boxed{\|S_{h,k}^n\|=\mathop{\mathrm{ess\,sup}}_\theta|G(\theta)|^n.}
$$

The upper bound is immediate by integration. For the reverse inequality choose Fourier data supported in a positive-measure neighborhood where $|G|$ approaches its essential supremum, then normalize them. This uses actual square-summable data, unlike an isolated infinite plane wave. On a periodic finite grid the [discrete Fourier transform](../../../../../discrete-fourier-transform.md) gives the same equality with a maximum over its resolved frequencies.

This proves the [scalar Fourier power criterion](../../../../../scalar-fourier-power-criterion.md). Contractivity is equivalent to $|G|\leq1$ at every frequency. For mesh-uniform [stability](../../../../../stability-of-a-numerical-method.md) on $nk\leq T$, a sufficient condition is instead $\sup|G|\leq1+Ck$, because $(1+Ck)^n\leq e^{CT}$. Conversely, if the powers at $n=\lfloor T/k\rfloor$ are bounded by a common $M_T\geq1$, then $\sup|G|\leq M_T^{1/n}=1+O(k)$ as $k\to0$. Thus finite-time [stability](../../../../../stability-of-a-numerical-method.md) may allow mild modal growth; demanding strict contraction is stronger than necessary.

[Stability](../../../../../stability-of-a-numerical-method.md) connects [numerical consistency](../../../../../consistency-of-a-numerical-method.md) to [numerical convergence](../../../../../convergence-of-a-numerical-method.md). Let $R_hu(t_n)$ be the exact solution restricted by a suitable projection and let its one-step defect be $\tau_n=R_hu(t_{n+1})-S_{h,k}R_hu(t_n)$. If $\|\tau_n\|\leq Ck(h^p+k^q)$ and $\|S^n\|\leq M_T$, the error recurrence gives

$$
e_n=S^ne_0-\sum_{j=0}^{n-1}S^{n-1-j}\tau_j,
\qquad
\boxed{\|e_n\|\leq M_T\|e_0\|+CM_TT(h^p+k^q).}
$$

This proves [numerical convergence](../../../../../convergence-of-a-numerical-method.md) for smooth solutions and convergent initial approximations. Density plus [stability](../../../../../stability-of-a-numerical-method.md) extends [numerical convergence](../../../../../convergence-of-a-numerical-method.md) to the natural data space when stable projections and well-posed continuous evolution are available.

For completeness, the converse in the [Lax equivalence theorem](../../../../../lax-equivalence-theorem.md) can be understood with faithful grid transfers. Let $J_h$ be a bounded reconstruction into the continuous data space and $R_h$ a bounded projection with $R_hJ_h=I$, and suppose the grid and reconstructed norms are uniformly equivalent. [numerical convergence](../../../../../convergence-of-a-numerical-method.md) for every datum, uniformly on the fixed time interval, makes the operators $J_hS_{h,k}^nR_h$ pointwise bounded. The [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md) makes their [operator norms](../../../../../operator-norm.md) uniformly bounded. Apply this bound to $J_hV$, use $R_hJ_hV=V$ and the norm equivalence, and obtain the uniform grid-power bound. With the [numerical consistency](../../../../../consistency-of-a-numerical-method.md) estimate above, this proves the [stability](../../../../../stability-of-a-numerical-method.md)/[numerical convergence](../../../../../convergence-of-a-numerical-method.md) equivalence under these standard linear assumptions.

Several examples illustrate the test. For forward time and centered space on the one-dimensional [heat equation](../../../../../heat-equation.md),

$$
G(\theta)=1-4\mu\sin^2(\theta/2),\qquad \mu=k/h^2.
$$

Its minimum is $1-4\mu$, so **$0\leq\mu\leq1/2$** is the exact contraction range. In $d$ dimensions with mesh widths $h_a$, the symbol is $1-4\sum_a\mu_a\sin^2(\theta_a/2)$, where $\mu_a=k/h_a^2$. Therefore **$\sum_a\mu_a\leq1/2$**, or $\mu\leq1/(2d)$ on an equal mesh. This follows by independently maximizing every sine factor, not by applying a one-dimensional bound separately to each direction.

For advection $u_t+a u_x=0$, forward time and centered space give $G=1-i\nu\sin\theta$, $\nu=ak/h$. At fixed nonzero advective [Courant number](../../../../../courant-number.md) its modulus exceeds one, so its powers grow without a mesh-uniform bound. Under the much smaller choice $k=O(h^2)$, however, $\log|G|\leq a^2k^2/(2h^2)=O(k)$, allowing finite-time [stability](../../../../../stability-of-a-numerical-method.md). This illustrates why the specified refinement path matters. For $a>0$, the upwind update instead has

$$
G=1-\nu+\nu e^{-i\theta},\qquad
|G|^2=1-4\nu(1-\nu)\sin^2(\theta/2),
$$

and is contractive exactly for $0\leq\nu\leq1$. Its numerical diffusion explains the stable damping as well as its first-order spatial accuracy.

For the [heat equation](../../../../../heat-equation.md) with the [Crank-Nicolson method](../../../../../crank-nicolson-method.md), the symbol is $(1-2\mu\sin^2(\theta/2))/(1+2\mu\sin^2(\theta/2))$. It has modulus at most one for every nonnegative $\mu$, so there is no diffusion time-step restriction. Very stiff modes nevertheless have amplification near minus one, causing weakly damped oscillation; [stability](../../../../../stability-of-a-numerical-method.md) alone does not guarantee good stiff smoothing or small error.

For systems the symbol is a [matrix](../../../../../matrix.md), and the exact criterion is the [uniform power bound for matrix Fourier symbols](../../../../../uniform-power-bound-for-matrix-fourier-symbols.md), not just a bound on [eigenvalue](../../../../../eigenvalue.md) moduli. For example $G=\begin{pmatrix}1&1\\0&1\end{pmatrix}$ has both [eigenvalues](../../../../../eigenvalue.md) one but $G^n=\begin{pmatrix}1&n\\0&1\end{pmatrix}$ is unbounded as the number of steps increases. If $G=X\Lambda X^{-1}$ with uniformly bounded condition numbers, then $\|G^n\|\leq\|X\|\|X^{-1}\|\max|\lambda|^n$, so a scalar-type condition does suffice. Multilevel schemes are treated by stacking their time levels into a companion [matrix](../../../../../matrix.md) and checking its uniform powers. Simple unit-modulus roots and interior roots are the fixed-mode root condition, but uniformity near colliding roots still needs attention.

The technique is inexpensive, identifies the dangerous wavelengths, gives sharp constant-coefficient restrictions and generalizes directly to several space variables and Fourier-diagonalizable vector problems. Its limitations are equally concrete: boundaries can add unstable modes invisible to an infinite-grid calculation; variable coefficients couple frequencies; nonlinearities invalidate the fixed multiplier; nonuniform grids need another transform or energy estimate; and L2 [stability](../../../../../stability-of-a-numerical-method.md) does not by itself imply a maximum principle or positivity. Frozen-coefficient analysis is often useful evidence, while an energy or boundary estimate is needed to turn it into a global conclusion in those settings.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
