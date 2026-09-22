<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For an evolutionary [partial differential equation](../../../../../partial-differential-equation-split.md), [stability of a numerical method](../../../../../stability-of-a-numerical-method.md) means that errors in the starting data and forcing stay controlled on each fixed interval $0\leq t\leq T$, with constants independent of the mesh. [Fourier stability analysis](../../../../../fourier-stability-analysis.md) is especially effective for a constant-coefficient [finite difference method](../../../../../finite-difference-method.md) on a uniform infinite or periodic grid: translation invariance makes different [Fourier modes](../../../../../fourier-mode.md) evolve independently.

For a scalar one-step scheme on the integer lattice, insert $U_m^n=\widehat U^n(\theta)e^{im\theta}$, with $-\pi\leq\theta\leq\pi$. The [Fourier symbol](../../../../../fourier-symbol-of-a-difference-operator.md) of each shift is $e^{ij\theta}$, and the update reduces to

$$
 \widehat U^{n+1}(\theta)=G(\theta)\widehat U^n(\theta).
$$

The [amplification factor](../../../../../amplification-factor.md) $G$ must be defined for every relevant frequency; for an implicit scheme this includes checking that its denominator is nonzero. The [Parseval identity](../../../../../parseval-identity.md) turns a bound $\sup_\theta|G(\theta)|^n\leq C_T$ into a discrete [L2 norm](../../../../../l2-norm.md) bound. Thus $|G|\leq1$ gives contractivity, while the more general bound $|G|\leq1+Ck$ gives $\|U^n\|_h\leq e^{CT}\|U^0\|_h$ for $nk\leq T$. Conversely, frequencies with amplification uniformly greater than one produce unstable wave packets or periodic [Fourier modes](../../../../../fourier-mode.md) under refinement.

For a system, $G(\theta)$ is an amplification [matrix](../../../../../matrix.md); for a multilevel scheme, a companion [matrix](../../../../../matrix.md) evolves the vector of time levels. The actual requirement is a uniform bound on matrix powers, not just their [spectral radius](../../../../../spectral-radius.md). A nontrivial [Jordan block](../../../../../jordan-block.md) at a unit-modulus [eigenvalue](../../../../../eigenvalue.md) creates polynomial growth in the time index. Even simple [eigenvalues](../../../../../eigenvalue.md) inside the unit disk can fail to give a uniform bound if the [eigenvector](../../../../../eigenvector.md) matrices become ill-conditioned as the mesh changes. Uniformly controlled [diagonalization of a matrix](../../../../../diagonalization-of-a-matrix.md), or a suitable quadratic energy estimate, resolves this issue. The [power boundedness of a two-level Fourier scheme](../../../../../power-boundedness-of-a-two-level-fourier-scheme.md) illustrates why root multiplicities and conditioning matter.

For the [heat equation](../../../../../heat-equation.md), put $\mu=k/h_x^2$. Centered space with the [Forward Euler method](../../../../../euler-method.md) has

$$
 G(\theta)=1-4\mu\sin^2(\theta/2).
$$

The [von Neumann stability analysis](../../../../../von-neumann-stability-analysis.md) condition $|G|\leq1$ holds exactly for $0\leq\mu\leq1/2$ on the full frequency interval. The [Backward Euler diffusion scheme](../../../../../backward-euler-diffusion-scheme.md) instead has $G=(1+4\mu\sin^2(\theta/2))^{-1}$ and is stable for every $\mu\geq0$. The [Crank-Nicolson diffusion scheme](../../../../../crank-nicolson-diffusion-scheme.md) has

$$
 G=\frac{1-2\mu\sin^2(\theta/2)}{1+2\mu\sin^2(\theta/2)}.
$$

It too is unconditionally stable, but poorly resolved high-frequency modes have $G\approx-1$ for large $\mu$, giving oscillatory numerical transients. [A-stability](../../../../../a-stability.md) therefore does not guarantee strong damping; [L-stability](../../../../../l-stability.md) distinguishes the damping of the [Backward Euler method](../../../../../backward-euler-method.md).

For the [advection equation](../../../../../transport-equation.md) $u_t+cu_x=0$, let $\nu=ck/h_x$. Forward time and centered space give

$$
 G=1-i\nu\sin\theta,\qquad |G|^2=1+\nu^2\sin^2\theta.
$$

For nonzero fixed $\nu$, repeated steps amplify some modes by a fixed factor greater than one, so the method is unstable under the usual refinement $k\propto h_x$. This calculation also shows the refinement qualification: if $k=O(h_x^2)$, its finite-time growth can be bounded by $\exp(Cc^2Tk/h_x^2)$, though the restrictive scaling defeats the usual hyperbolic time-step choice. For $c>0$, the [upwind finite difference scheme](../../../../../upwind-finite-difference-scheme.md) has

$$
 G=1-\nu+\nu e^{-i\theta},\qquad
 |G|^2=1-4\nu(1-\nu)\sin^2(\theta/2),
$$

so it is stable for $0\leq\nu\leq1$. The [Lax-Wendroff advection scheme](../../../../../lax-wendroff-advection-scheme.md) instead has

$$
 G=1-i\nu\sin\theta+\nu^2(\cos\theta-1),\qquad
 |G|^2=1-4\nu^2(1-\nu^2)\sin^4(\theta/2),
$$

giving $|\nu|\leq1$. These examples separate the effects of the spatial stencil, temporal approximation and [Courant number](../../../../../courant-number.md); a higher [order of a numerical method](../../../../../order-of-a-numerical-method.md) by itself does not establish [stability](../../../../../stability-of-a-numerical-method.md).

A [periodic boundary condition](../../../../../periodic-boundary-conditions.md) is ideal for this analysis. The [discrete Fourier transform](../../../../../discrete-fourier-transform.md) diagonalizes the circulant update, with only the discrete frequencies $2\pi j/J$ needed on a grid of $J$ points. A bound on all $\theta$ is a convenient guarantee over every such grid. On the whole line, the [Fourier transform](../../../../../fourier-transform.md) uses a continuous frequency interval and the [Parseval identity](../../../../../parseval-identity.md) proves the corresponding square-summable-data estimate.

Homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) do not admit arbitrary complex exponential [Fourier modes](../../../../../fourier-mode.md). For the standard centered second difference on $M$ interior points, a [discrete sine transform](../../../../../discrete-sine-transform.md) diagonalizes the actual boundary-value [matrix](../../../../../matrix.md):

$$
 v_j(m)=\sin\frac{jm\pi}{M+1},\qquad
 -D_hv_j=\frac4{h_x^2}\sin^2\frac{j\pi}{2(M+1)}v_j.
$$

The same heat amplification formulas then apply at these sine frequencies. For example, the exact forward-Euler contractivity limit on that fixed grid is $\mu\leq[2\cos^2(\pi/(2(M+1)))]^{-1}$; the mesh-independent sufficient limit $1/2$ follows by including all frequencies. Homogeneous [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) can similarly permit a [discrete cosine transform](../../../../../discrete-cosine-transform.md), provided the endpoint discretization and its weighted [inner product](../../../../../inner-product.md) are chosen consistently. The constant mode is then present, reflecting conservation of the heat equation's spatial mean. For inhomogeneous [boundary conditions](../../../../../boundary-condition.md), subtract a suitable lifting of the prescribed boundary data and estimate the induced source using the homogeneous evolution's bound and a [Duhamel principle](../../../../../duhamel-s-principle.md) estimate. Bounds for the lifting and source must themselves be uniform in the mesh.

General [boundary conditions](../../../../../boundary-condition.md) require separate [boundary stability of a finite-difference method](../../../../../boundary-stability-of-a-finite-difference-method.md). For an [advection equation](../../../../../transport-equation.md), incoming data are prescribed at the inflow boundary, while an outflow closure must respect the outgoing characteristics. An interior periodic [Fourier symbol](../../../../../fourier-symbol-of-a-difference-operator.md) cannot detect a growing mode confined near a boundary. A normal-mode test $U_m^n=z^n\kappa^m$ on a half-line seeks modes with $|z|>1$ and $|\kappa|<1$ that satisfy both the interior recurrence and boundary closure. Their existence proves instability, and uniform control requires more than merely excluding isolated growing roots; the [Uniform Kreiss--Lopatinskii condition](../../../../../uniform-kreiss-lopatinskii-condition.md) addresses boundary resolvent bounds. Alternatively, a direct [energy method](../../../../../energy-method.md) using [summation by parts](../../../../../abel-s-summation-formula.md) can include the boundary terms and establish the required estimate.

Variable coefficients and nonuniform meshes usually destroy exact [Fourier transform](../../../../../fourier-transform.md) diagonalization. Frozen-coefficient [Fourier stability analysis](../../../../../fourier-stability-analysis.md) is then a useful diagnostic, but it is not automatically a proof for the full variable-coefficient boundary problem. The mesh-uniform [energy method](../../../../../energy-method.md) in question 5 is an example of a direct proof. Also, an [L2 norm](../../../../../l2-norm.md) proof is not automatically a mesh-uniform maximum-[norm](../../../../../norm.md) proof: finite-dimensional norm-equivalence constants may grow with the number of grid points.

Finally, [stability](../../../../../stability-of-a-numerical-method.md) measures error propagation; [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) measures the defect of inserting the exact solution. For a well-posed linear initial-value problem in the chosen norm, the [Lax equivalence theorem](../../../../../lax-equivalence-theorem.md) says that a consistent approximation is convergent exactly when it is stable. Boundary discretization and starting data must be included in that assertion. **A Fourier calculation proves convergence only after consistency, well-posedness and the actual boundary treatment have also been checked.**

## ↑ Ancestors (11)

1. [6](../6.md)
2. [Section B](../section-b.md)
3. [Paper 68](../../paper-68-split.md)
4. [Iii](../../split.md)
5. [2015](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
