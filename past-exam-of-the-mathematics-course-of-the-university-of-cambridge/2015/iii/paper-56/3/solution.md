<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The product of the magnetic field with the velocity in this question is the three-dimensional [cross product](../../../../../cross-product.md). Fix $\epsilon_{123}=1$ and write $K^i{}_j=\epsilon^i{}_{kj}B^k$, so $K\mathbf v=\mathbf B\times\mathbf v$. In coordinates $y^0=t$, $y^i=x^i$ on $\mathbb R^3\times\mathbb R$, prescribe an [affine connection](../../../../../affine-connection.md) by the following [Christoffel symbols](../../../../../christoffel-symbol.md):

$$
\boxed{\Gamma^i{}_{00}=-E^i,\qquad\Gamma^i{}_{0j}=\Gamma^i{}_{j0}=-K^i{}_j=\epsilon^i{}_{jk}B^k,}
$$

with all other [Christoffel symbols](../../../../../christoffel-symbol.md) zero. These are smooth globally in the given Cartesian coordinates. The lower-index symmetry makes this a [torsion-free connection](../../../../../torsion-free-connection.md). It is the [geometrization of the Lorentz force by an affine connection](../../../../../geometrization-of-the-lorentz-force-by-an-affine-connection.md); no condition on the [curl](../../../../../curl.md) of $\mathbf E$ or the [divergence](../../../../../divergence.md) of $\mathbf B$ is required for this construction.

An affinely parametrized [geodesic](../../../../../geodesic.md), with primes denoting differentiation with respect to $\lambda$, satisfies

$$
t''=0,\qquad \mathbf x''-\mathbf E(t')^2-2t'\mathbf B\times\mathbf x'=0.
$$

On the branch $t'=c\ne0$, use $t$ itself as an [affine parameter](../../../../../affine-parameter.md). Dividing the spatial equation by $c^2$ gives

$$
\boxed{\frac{d^2\mathbf x}{dt^2}=\mathbf E+2\mathbf B\times\frac{d\mathbf x}{dt}.}
$$

Conversely, each solution of this equation makes $\lambda=t$, $y(t)=(t,\mathbf x(t))$ an affinely parametrized [geodesic](../../../../../geodesic.md) of the constructed [affine connection](../../../../../affine-connection.md). Therefore its image is also an unparametrized [geodesic](../../../../../geodesic.md). A general change of parameter adds a term proportional to the tangent in the [geodesic equation](../../../../../geodesic-equation.md), leaving the curve unchanged. The branch $t'=0$ is not a trajectory with time as parameter.

For the metric realization, assume $\mathbf E=-\nabla U$ and $\nabla\cdot\mathbf B=0$. Introduce the [differential form](../../../../../differential-form-split.md)

$$
F=\iota_{\mathbf B}(dx^1\wedge dx^2\wedge dx^3)=\frac12F_{ij}\,dx^i\wedge dx^j,\qquad F_{ij}=\epsilon_{ijk}B^k.
$$

Then $dF=(\nabla\cdot\mathbf B)\,dx^1\wedge dx^2\wedge dx^3=0$. The global [Poincaré lemma](../../../../../poincare-lemma.md) on the contractible space $\mathbb R^3$ supplies a one-form $A=A_i dx^i$ with $dA=F$, equivalently a [magnetic vector potential](../../../../../magnetic-vector-potential.md) with $\nabla\times\mathbf A=\mathbf B$. An explicit [radial-gauge potential for a divergence-free magnetic field](../../../../../radial-gauge-potential-for-a-divergence-free-magnetic-field.md) is

$$
\boxed{A_i(\mathbf x)=\int_0^1 s x^jF_{ji}(s\mathbf x)\,ds,\qquad\mathbf A(\mathbf x)=\int_0^1s\,\mathbf B(s\mathbf x)\times\mathbf x\,ds.}
$$

This is the radial homotopy formula for a closed two-form and is smooth even at the origin. For a constant magnetic field it gives $\mathbf A=\tfrac12\mathbf B\times\mathbf x$.

Consider the [Eisenhart-Duval lift](../../../../../eisenhart-duval-lift.md) with the [Lorentzian metric](../../../../../lorentzian-metric.md)

$$
g=d\mathbf x^2+2dt\bigl(du-2A_i dx^i-Udt\bigr).
$$

The independent one-forms $dx^1,dx^2,dx^3,dt,du-2A_i dx^i-Udt$ exhibit three positive directions and a two-dimensional block with one positive and one negative direction. Thus the metric is nondegenerate, of signature $(4,1)$. Its coefficients do not depend on $u$, and $g_{uu}=0$, so $\xi=\partial_u$ is a null [Killing vector field](../../../../../killing-vector-field.md). Indeed $g_{Au}$ are constant, so $\Gamma^A{}_{Bu}=0$ for the [Levi-Civita connection](../../../../../levi-civita-connection.md) and $\xi$ is parallel.

The [geodesic](../../../../../geodesic.md) Lagrangian for an [affine parameter](../../../../../affine-parameter.md) $\lambda$ is

$$
L=\frac12|\mathbf x'|^2-U(t')^2-2A_i x'^i t'+t'u'.
$$

The cyclic coordinate $u$ gives the [conserved quantity](../../../../../conserved-quantity.md) $p_u=\partial L/\partial u'=t'$. Work at a nonzero value of $p_u$ and rescale the [affine parameter](../../../../../affine-parameter.md) to set $t'=1$. This is the essential step in the [null Kaluza-Klein reduction of a stationary force](../../../../../null-kaluza-klein-reduction-of-a-stationary-force.md): one fixes the momentum along the null isometry and projects its [geodesics](../../../../../geodesic.md), rather than dividing by $g_{uu}$.

The spatial [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md), before setting $t'=1$, are

$$
x''_i+\partial_iU(t')^2+2(\partial_iA_j-\partial_jA_i)x'^j t'-2A_i t''=0.
$$

Since $t''=0$ and $F_{ij}v^j=-(\mathbf B\times\mathbf v)_i$, their reduction is

$$
\boxed{\ddot{\mathbf x}=-\nabla U+2\mathbf B\times\dot{\mathbf x}.}
$$

Equivalently, after taking $t$ as the [affine parameter](../../../../../affine-parameter.md), the term $\dot u$ is a total derivative and the reduced Lagrangian is $L_{\mathrm{red}}=\tfrac12|\dot{\mathbf x}|^2-2\mathbf A\cdot\dot{\mathbf x}-U$. Its [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) give the same sign and factor two.

There is also an explicit converse using null [geodesics](../../../../../geodesic.md). For any physical trajectory, set

$$
\boxed{\dot u=U+2\mathbf A\cdot\dot{\mathbf x}-\frac12|\dot{\mathbf x}|^2.}
$$

This makes its five-dimensional tangent null. The conserved momentum of the cyclic coordinate $t$ becomes

$$
p_t=-2U-2\mathbf A\cdot\dot{\mathbf x}+\dot u=-\left(U+\frac12|\dot{\mathbf x}|^2\right).
$$

The quantity in parentheses is conserved, because its derivative is $\dot{\mathbf x}\cdot(2\mathbf B\times\dot{\mathbf x})=0$. Hence the $t$ equation, as well as the spatial and $u$ [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md), is satisfied. **Every trajectory admits a null geodesic lift with $p_u=1$, and every such lift projects to the required trajectory.**

Finally, a time-independent [gauge transformation](../../../../../gauge-transformation.md) $\mathbf A\mapsto\mathbf A+\nabla\chi$ is absorbed by $u\mapsto u+2\chi$. The one-form $du-2A_i dx^i-Udt$ and the five-dimensional metric are unchanged. These [gauge transformations of an Eisenhart-Duval lift](../../../../../gauge-transformations-of-an-eisenhart-duval-lift.md) alter the reduced Lagrangian only by the total derivative $-2d\chi/dt$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
