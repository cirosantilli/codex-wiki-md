<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a scalar, the [Lie derivative of a function](../../../../../lie-derivative-of-a-function.md) is its [directional derivative](../../../../../directional-derivative.md):

$$
\mathcal L_\xi f=\xi^a\partial_af.
$$

The [Lie derivative of a vector field](../../../../../lie-derivative-of-a-vector-field.md) is their [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md):

$$
(\mathcal L_\xi X)^a=\xi^b\partial_bX^a-X^b\partial_b\xi^a.
$$

For a [torsion-free connection](../../../../../torsion-free-connection.md),

$$
(\nabla_\xi X-\nabla_X\xi)^a=\xi^b\partial_bX^a-X^b\partial_b\xi^a+\Gamma^a{}_{bc}(\xi^bX^c-X^b\xi^c).
$$

The last term vanishes because the [connection coefficients](../../../../../connection-components.md) are symmetric in $b,c$. This proves **$\mathcal L_\xi X=\nabla_\xi X-\nabla_X\xi$**.

For the [metric tensor](../../../../../metric-tensor.md) statements use the [Levi-Civita connection](../../../../../levi-civita-connection.md), which also has [metric compatibility](../../../../../metric-compatibility.md). The [tensor derivation](../../../../../tensor-derivation.md) property of the [Lie derivative of a tensor field](../../../../../lie-derivative-of-a-tensor-field.md) gives

$$
(\mathcal L_\xi g)(X,Y)=\xi[g(X,Y)]-g(\mathcal L_\xi X,Y)-g(X,\mathcal L_\xi Y).
$$

Expanding the first term using $\nabla g=0$ and using the vector identity cancels the derivatives of $X$ and $Y$. What remains is

$$
(\mathcal L_\xi g)(X,Y)=g(\nabla_X\xi,Y)+g(X,\nabla_Y\xi)=2\xi_{(a;b)}X^aY^b.
$$

Since $X,Y$ are arbitrary, the [Killing equation](../../../../../killing-equation.md) is

$$
\boxed{\mathcal L_\xi g=0\quad\Longleftrightarrow\quad\xi_{(a;b)}=0.}
$$

[Metric compatibility](../../../../../metric-compatibility.md) is needed here, even though symmetry alone sufficed for the vector identity. In general the [Lie derivative of a metric with nonmetricity](../../../../../lie-derivative-of-a-metric-with-nonmetricity.md) contains a term $\xi^c\nabla_cg_{ab}$. For example, with the [metric tensor](../../../../../metric-tensor.md) $g=e^{2x}dx^2$, zero [connection coefficients](../../../../../connection-components.md) and $\xi=\partial_x$, the [Lie derivative of a tensor field](../../../../../lie-derivative-of-a-tensor-field.md) is $2e^{2x}$, whereas $2\nabla_x\xi_x=4e^{2x}$. The usual [metric connection](../../../../../metric-connection.md) interpretation of the question supplies the required compatibility.

For the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) calculation, keep the original PDF's convention. With $R_{abcd}=g_{ae}R^e{}_{bcd}$ and $R_{abc}{}^d=g^{de}R_{abce}$, it means

$$
[\nabla_c,\nabla_d]X^a=-R^a{}_{bcd}X^b.
$$

Thus the [commutator](../../../../../commutator.md) on a [covector](../../../../../covector.md) has the opposite sign. Write $K_{abc}=\xi_{a;bc}=\nabla_c\nabla_b\xi_a$. Taking a [covariant derivative](../../../../../covariant-derivative.md) of the [Killing equation](../../../../../killing-equation.md) makes $K$ antisymmetric in its first two indices, while the [Ricci identity](../../../../../curvature-commutator-on-a-covariant-tensor.md) gives

$$
K_{abc}-K_{acb}=R_{adbc}\xi^d.
$$

Combining this with the first-two-index antisymmetry gives the three relations

$$
K_{abc}+K_{cab}=R_{adbc}\xi^d,\quad K_{cab}+K_{bca}=R_{cdab}\xi^d,\quad K_{bca}+K_{abc}=R_{bdca}\xi^d.
$$

Add the first and third and subtract the second. Pair symmetry and the [first Bianchi identity](../../../../../first-bianchi-identity.md) imply $R_{adbc}+R_{bdca}-R_{cdab}=-2R_{abcd}$. Consequently

$$
K_{abc}=-R_{abcd}\xi^d,\qquad\boxed{\xi_{b;ca}=-R_{bca}{}^d\xi_d.}
$$

This is the [second covariant derivative of a Killing vector](../../../../../second-covariant-derivative-of-a-killing-vector.md) in the paper's convention; its sign is tied to the declared [curvature-sign convention in Killing derivative identities](../../../../../curvature-sign-convention-in-killing-derivative-identities.md), not to raising a particular index.

Set $L_{ab}=\xi_{a;b}$. Along any [smooth curve](../../../../../smooth-curve.md) with [tangent vector](../../../../../tangent-vector.md) $V$, the [chain rule](../../../../../chain-rule.md) and the just-proved identity give the [Killing transport equations](../../../../../killing-transport.md)

$$
\boxed{\nabla_V\xi_a=L_{ab}V^b,\qquad\nabla_VL_{ab}=-R_{abc}{}^dV^c\xi_d.}
$$

Choose a [parallel-propagated orthonormal frame](../../../../../parallel-propagated-orthonormal-frame.md) along the curve. These become a homogeneous [linear system of ordinary differential equations](../../../../../linear-system-of-differential-equations.md) for the components of $(\xi,L)$. Uniqueness of its [initial value problem](../../../../../initial-value-problem.md) implies that zero initial data remain zero. Any point in the same [connected component](../../../../../connected-component.md) as $P$ can be joined to $P$ by a piecewise smooth curve. Therefore **zero value and zero first derivative at $P$ force the [Killing field](../../../../../killing-vector-field.md) and its derivative to vanish throughout that component**, with no completeness assumption. On a [manifold](../../../../../topological-manifold.md) with one [connected component](../../../../../connected-component.md) this is the requested global result. [Connectedness](../../../../../connected-space.md) cannot be dropped: on two disjoint flat spacetimes, take the zero field on one and a nonzero translation on the other.

On a [pseudo-Riemannian manifold](../../../../../pseudo-riemannian-manifold.md) of dimension $n$ with one [connected component](../../../../../connected-component.md), the map $\xi\mapsto(\xi_a(P),L_{ab}(P))$ is therefore injective. There are $n$ independent components of the value and $n(n-1)/2$ of its antisymmetric derivative. The [dimension bound for Killing vector fields](../../../../../dimension-bound-for-killing-vector-fields.md) is

$$
\boxed{\dim\mathfrak{kill}(M,g)\leq\frac{n(n+1)}2.}
$$

It is attained in flat space by $\xi_a=A_a+B_{ab}x^b$ with constant antisymmetric $B$, giving translations and infinitesimal rotations or [Lorentz transformations](../../../../../lorentz-transformation.md). The four-dimensional maximum is **10**. For a disconnected manifold the bound applies componentwise; there is no uniform global bound depending only on $n$ if the number of components is unrestricted.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
