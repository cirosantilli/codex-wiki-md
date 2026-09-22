<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Work on a regular patch with a smooth nonzero conformal factor. Its sign is constant there, so replace it by $|\Omega|$ if necessary and assume $\Omega>0$. Put $u=\log\Omega$, and let all partial derivatives, index raising on $u_i,\Omega_i$, and the operators $\Delta,|\nabla\cdot|^2$ in the following formulas use the flat Cartesian metric $\delta$. The [orthonormal coframe](../../../../../orthonormal-coframe-in-spacetime.md) $E^i=\Omega dx^i$ has

$$
dE^i=\Omega^{-2}\Omega_k E^k\wedge E^i.
$$

The proposed [connection 1-forms](../../../../../connection-1-form-split.md) reduce to

$$
\boxed{\omega^i{}_j=\Omega^{-2}(\Omega_jE^i-\Omega_iE^j)=u_jdx^i-u_idx^j.}
$$

Lowering the first frame index with $\delta$ makes these antisymmetric, which establishes [metric compatibility](../../../../../metric-compatibility.md). Moreover,

$$
\omega^i{}_j\wedge E^j=\Omega^{-2}\Omega_jE^i\wedge E^j=-dE^i.
$$

Thus [Cartan's first structure equation](../../../../../cartan-s-first-structure-equation.md) has zero torsion. Uniqueness of the metric-compatible [torsion-free connection](../../../../../torsion-free-connection.md) identifies these forms as the [Levi-Civita connection](../../../../../levi-civita-connection.md); this also explains why merely guessing a skew connection would not have sufficed.

To calculate the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md), use [Cartan's second structure equation](../../../../../cartan-s-second-structure-equation.md). Direct differentiation and multiplication give

$$
\begin{aligned}
d\omega^i{}_j&=u_{jk}dx^k\wedge dx^i-u_{ik}dx^k\wedge dx^j,\\
\omega^i{}_k\wedge\omega^k{}_j
&=u_j u_kdx^i\wedge dx^k-|\nabla u|^2dx^i\wedge dx^j+u_i u_kdx^k\wedge dx^j.
\end{aligned}
$$

Introduce the [Schouten tensor](../../../../../schouten-tensor.md) in Cartesian coordinate components,

$$
S_{ij}=-u_{ij}+u_i u_j-\frac12|\nabla u|^2\delta_{ij}
=-\frac{\Omega_{ij}}\Omega+\frac{2\Omega_i\Omega_j}{\Omega^2}-\frac{|\nabla\Omega|^2}{2\Omega^2}\delta_{ij}.
$$

The preceding calculation groups into the [curvature 2-forms](../../../../../curvature-2-form.md)

$$
\mathcal R^i{}_j=S_{jl}\,dx^i\wedge dx^l+S_{ik}\,dx^k\wedge dx^j.
$$

Keep the convention $R_{ijkl}=g(\partial_i,R(\partial_k,\partial_l)\partial_j)$, with $R(X,Y)=[\nabla_X,\nabla_Y]-\nabla_{[X,Y]}$, as in the first solution. Converting frame indices to coordinate indices gives the [curvature of a conformally Euclidean metric](../../../../../curvature-of-a-conformally-euclidean-metric.md):

$$
\boxed{R_{ijkl}=\Omega^2(\delta_{ik}S_{jl}+\delta_{jl}S_{ik}-\delta_{il}S_{jk}-\delta_{jk}S_{il}).}
$$

These are coordinate components. Components in the dual [orthonormal frame](../../../../../orthonormal-frame-in-spacetime.md) are $\Omega^{-4}R_{ijkl}$, hence the same expression with the overall factor $\Omega^{-2}$. This distinction is important when contracting the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md).

Contract with $g^{ik}=\Omega^{-2}\delta^{ik}$. In four dimensions the [Ricci tensor](../../../../../ricci-tensor.md) becomes $R_{jl}=2S_{jl}+\delta_{jl}\sum_kS_{kk}$, and therefore

$$
\boxed{R_{ij}=-2u_{ij}+2u_i u_j-\delta_{ij}\bigl(\Delta u+2|\nabla u|^2\bigr)
=-\frac{2\Omega_{ij}}\Omega+\frac{4\Omega_i\Omega_j}{\Omega^2}-\delta_{ij}\left(\frac{\Delta\Omega}\Omega+\frac{|\nabla\Omega|^2}{\Omega^2}\right).}
$$

Taking the remaining metric trace yields the [Ricci scalar](../../../../../ricci-scalar.md)

$$
\boxed{R=-6\Omega^{-2}\bigl(\Delta u+|\nabla u|^2\bigr)=-6\Omega^{-3}\Delta\Omega.}
$$

The cancellation of the gradient-squared terms in the last expression is special to dimension four.

For the [Tolman wormhole](../../../../../tolman-wormhole.md), compute on $r>0$:

$$
\Omega_i=-\frac{2\lambda x_i}{r^4},\qquad
\Omega_{ij}=-\frac{2\lambda\delta_{ij}}{r^4}+\frac{8\lambda x_ix_j}{r^6},\qquad
\Delta\Omega=0,\qquad |\nabla\Omega|^2=\frac{4\lambda^2}{r^6}.
$$

Substitution into the [Ricci tensor](../../../../../ricci-tensor.md) and [Ricci scalar](../../../../../ricci-scalar.md) gives

$$
\boxed{R=0,\qquad R_{ij}=\frac{4\lambda}{(r^2+\lambda)^2}\left(\delta_{ij}-\frac{4x_ix_j}{r^2}\right).}
$$

For example, the coordinate radial eigenvalue is $-12\lambda/(r^2+\lambda)^2$, while each of the three tangential eigenvalues is $4\lambda/(r^2+\lambda)^2$. Their sum vanishes, but none vanishes when $\lambda\ne0$. The [Vacuum Einstein equations](../../../../../vacuum-einstein-equations.md) with zero [cosmological constant](../../../../../cosmological-constant.md) require $R_{ij}-\tfrac12Rg_{ij}=0$ and hence $R_{ij}=0$. **The metric is scalar-flat but not a vacuum solution for any nonzero $\lambda$; only $\lambda=0$ gives flat vacuum space.** A nonzero cosmological constant does not rescue it: its trace would force $R=4\Lambda$, so $R=0$ would first force $\Lambda=0$.

The smooth wormhole interpretation uses $\lambda>0$; $r=0$ is another asymptotically flat end, not an included origin, as inversion $\rho=\lambda/r$ shows. For $\lambda<0$, the conformal factor vanishes at $r=\sqrt{-\lambda}$, where the metric is degenerate. The local non-vacuum calculation remains valid on each regular region away from that sphere, but such a metric is not a smooth wormhole across it.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
