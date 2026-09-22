<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work on a regular level surface, so $d\beta\ne0$. A nonzero normal [covector](../../../../../covector.md) has the local form $n_a=f\nabla_a\beta$. Extend it as a normal to neighbouring level surfaces. Since the [Levi-Civita connection](../../../../../levi-civita-connection.md) is torsion-free,

$$
n_{a;b}=f_{;b}\beta_{;a}+f\beta_{;ab},\qquad \beta_{;ab}=\beta_{;ba}.
$$

Antisymmetrizing the product with $n_c=f\beta_{;c}$ over three indices kills the symmetric second-derivative term and the term containing two copies of $d\beta$. Hence

$$
\boxed{n_{[a;b}n_{c]}=0.}
$$

Equivalently $n\wedge dn=0$, the [Frobenius theorem](../../../../../frobenius-theorem.md) condition for [hypersurface orthogonality](../../../../../hypersurface-orthogonality.md).

For the [second covariant derivative of a Killing vector](../../../../../second-covariant-derivative-of-a-killing-vector.md), the curvature sign needs explicit care. Denote the curvature defined on the cover by $C^a{}_{bcd}$, and obtain its other index positions by ordinary raising and lowering with the [metric tensor](../../../../../metric-tensor.md). With $D_{abc}=k_{a;bc}$, the [Killing equation](../../../../../killing-equation.md) gives $D_{abc}=-D_{bac}$, while the supplied [Ricci identity](../../../../../curvature-commutator-on-a-covariant-tensor.md) gives

$$
D_{abc}-D_{acb}=C_a{}^d{}_{bc}k_d.
$$

Successive use of these two facts gives

$$
\begin{aligned}
D_{abc}&=-D_{bac}=-D_{bca}-C_b{}^d{}_{ac}k_d\\
&=D_{cba}-C_b{}^d{}_{ac}k_d\\
&=D_{cab}+C_c{}^d{}_{ba}k_d-C_b{}^d{}_{ac}k_d\\
&=-D_{acb}+C_c{}^d{}_{ba}k_d-C_b{}^d{}_{ac}k_d.
\end{aligned}
$$

Substitute $D_{acb}=D_{abc}-C_a{}^d{}_{bc}k_d$. The curvature symmetries and [first Bianchi identity](../../../../../first-bianchi-identity.md) then imply

$$
2D_{abc}=(C_a{}^d{}_{bc}+C_c{}^d{}_{ba}-C_b{}^d{}_{ac})k_d=-2C_{abc}{}^dk_d.
$$

Thus the identity consistent with the cover convention is

$$
\boxed{k_{a;bc}=-C_{abc}{}^d k_d.}
$$

The plus-sign version is valid for the opposite curvature tensor $\widetilde R=-C$. With ordinary metric index raising, the printed plus sign and the cover's curvature convention cannot both be used. This is the [curvature-sign convention in Killing derivative identities](../../../../../curvature-sign-convention-in-killing-derivative-identities.md), not a failure of the [Killing equation](../../../../../killing-equation.md).

An explicit sign check uses $ds^2=e^{2x}dt^2-dx^2-dy^2-dz^2$ and the timelike [Killing vector](../../../../../killing-vector-field.md) $k=\partial_t$. Here $k_t=e^{2x}$, $\Gamma^t{}_{tx}=1$ and $\Gamma^x{}_{tt}=e^{2x}$. Direct differentiation gives $k_{t;xx}=e^{2x}$, whereas the cover definition gives $C^t{}_{xxt}=-1$ and $C_{txx}{}^dk_d=-e^{2x}$. This also verifies the corrected sign without relying on a remembered curvature convention.

To prove the [static Killing field is a Ricci eigenvector](../../../../../static-killing-field-is-a-ricci-eigenvector.md), use the permitted alternative of adapted coordinates. [Hypersurface orthogonality](../../../../../hypersurface-orthogonality.md) supplies hypersurfaces orthogonal to $k$. Choose spatial coordinates on one such hypersurface and carry them along the flow of the [Killing vector](../../../../../killing-vector-field.md), using its flow parameter as $t$. The flow preserves both the [metric tensor](../../../../../metric-tensor.md) and $k$, so it preserves orthogonality to $k$. Consequently the mixed metric components vanish, and the [Killing equation](../../../../../killing-equation.md) makes all coefficients independent of $t$:

$$
ds^2=N(\mathbf x)^2dt^2-h_{ij}(\mathbf x)dx^idx^j,\qquad k^a=(1,0,0,0),\qquad k_a=(N^2,0,0,0).
$$

The only nonzero [Christoffel symbols](../../../../../christoffel-symbol.md) involving time can be

$$
\Gamma^0{}_{0i}=\partial_i\log N,\qquad \Gamma^i{}_{00}=Nh^{ij}\partial_jN;
$$

in particular $\Gamma^0{}_{ij}=\Gamma^i{}_{0j}=\Gamma^0{}_{00}=0$. In $C_{0i}$, the derivative of the connection trace vanishes because $\Gamma^a{}_{0a}=0$; the other derivative is either a time derivative of a static coefficient or a derivative of $\Gamma^j{}_{0i}=0$. Every connection-product term contains a vanishing coefficient of these same types. Thus $C_{0i}=0$. The one-form $C_{ab}k^b=C_{a0}$ has only a time component, and is proportional to $k_a$. Therefore

$$
\boxed{k_d C^d{}_{[a}k_{b]}=0.}
$$

Changing the overall curvature sign leaves this zero identity unchanged.

Finally a [perfect fluid](../../../../../perfect-fluid.md) in signature $(+---)$ has $T_{ab}=(\rho+p)u_au_b-pg_{ab}$ and $u^au_a=1$. Contract the [Einstein field equations](../../../../../einstein-field-equations.md) with $k^b$, and antisymmetrize with $k_a$. Terms proportional to $g_{ab}$ disappear, as does the Ricci term just proved. This leaves

$$
(\rho+p)(k\cdot u)u_{[a}k_{b]}=0.
$$

Two nonzero timelike vectors cannot be orthogonal: in the fluid's rest [local inertial frame](../../../../../local-inertial-frame.md), $k\cdot u=k^0\ne0$. The hypothesis $\rho+p>0$ therefore forces $u_{[a}k_{b]}=0$. Choosing $k$ future-directed gives the normalized [perfect-fluid alignment in a static spacetime](../../../../../perfect-fluid-alignment-in-a-static-spacetime.md) result

$$
\boxed{u^a=\frac{k^a}{\sqrt{k^bk_b}}.}
$$

The enthalpy hypothesis matters: when $\rho+p=0$, the [stress-energy tensor](../../../../../stress-energy-tensor.md) is proportional to the [metric tensor](../../../../../metric-tensor.md) and does not select a velocity.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
