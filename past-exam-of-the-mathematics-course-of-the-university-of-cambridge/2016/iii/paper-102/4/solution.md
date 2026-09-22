<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Start with the [tensor product of Lie algebra representations](../../../../../tensor-product-of-lie-algebra-representations.md), whose action is

$$
x\cdot(v\otimes w)=(xv)\otimes w+v\otimes(xw).
$$

Writing $T_x=\rho(x)\otimes I+I\otimes\rho(x)$, the two tensor factors commute, so $[T_x,T_y]=T_{[x,y]}$. This verifies the [Lie algebra representation](../../../../../lie-algebra-representation.md) identity over every field.

The [exterior square](../../../../../exterior-square.md) and [symmetric square](../../../../../symmetric-square.md) are the [quotient vector spaces](../../../../../quotient-vector-space.md)

$$
\bigwedge^2V=(V\otimes V)/\langle v\otimes v:v\in V\rangle,
\qquad
S^2V=(V\otimes V)/\langle v\otimes w-w\otimes v:v,w\in V\rangle.
$$

In the [exterior square](../../../../../exterior-square.md), expanding $(v+w)\otimes(v+w)$ shows that $v\wedge w=-w\wedge v$, including in [characteristic two](../../../../../characteristic-two.md). Both defining relation spaces are invariant under the [tensor product](../../../../../tensor-product.md) action: $x(v\otimes v)=xv\otimes v+v\otimes xv$ is an exterior relation, and the image of a symmetric relation is a sum of symmetric relations. Thus the quotient actions are well-defined and satisfy

$$
x(v\wedge w)=xv\wedge w+v\wedge xw,\qquad x(vw)=(xv)w+v(xw).
$$

For the printed [basis](../../../../../basis.md) $v_1,\ldots,v_n$, [bases](../../../../../basis.md) are $v_i\wedge v_j$ with $i<j$ and $v_iv_j$ with $i\le j$. Their dimensions are $n(n-1)/2$ and $n(n+1)/2$ respectively.

**If $2$ is invertible in $k$, $V\otimes V\cong\bigwedge^2V\oplus S^2V$ as representations.** Define the flip $\tau(v\otimes w)=w\otimes v$. It commutes with the [Lie algebra](../../../../../lie-algebra-split.md) action and satisfies $\tau^2=I$. Therefore

$$
P_+=\frac{I+\tau}{2},\qquad P_-=\frac{I-\tau}{2}
$$

are complementary invariant [linear projections](../../../../../projection-linear-algebra.md). The maps

$$
vw\longmapsto\frac{v\otimes w+w\otimes v}{2},\qquad
v\wedge w\longmapsto\frac{v\otimes w-w\otimes v}{2}
$$

identify $S^2V$ with $\operatorname{im}P_+$ and $\bigwedge^2V$ with $\operatorname{im}P_-$. Their inverses are the corresponding quotient maps restricted to these subspaces. This proves the assertion for every field of odd [characteristic](../../../../../characteristic-of-a-field.md), and also for [characteristic zero](../../../../../characteristic-zero.md).

**Over every field, $S^2(V\oplus W)\cong S^2V\oplus S^2W\oplus(V\otimes W)$.** The [symmetric square of a direct sum](../../../../../symmetric-square-of-a-direct-sum.md) isomorphism sends the first two summands into products within $V$ and within $W$, and sends $v\otimes w$ to the mixed product $vw$. If $v_i$ and $w_j$ are [bases](../../../../../basis.md), the monomial [basis](../../../../../basis.md) of $S^2(V\oplus W)$ is the disjoint union

$$
\{v_iv_j:i\le j\},\qquad\{w_iw_j:i\le j\},\qquad\{v_iw_j:\text{all }i,j\}.
$$

Thus the map is bijective, with no division by $2$ needed. The [Leibniz rule](../../../../../leibniz-rule.md) for the action preserves each of these three summands and agrees with its usual [Lie algebra representation](../../../../../lie-algebra-representation.md) action, proving equivariance.

For $\mathfrak g=\mathfrak{sl}(3)$, $V=\Gamma_{0,0}$ is trivial and $W=\Gamma_{2,1}$ has dimension $15$. Hence

$$
S^2(V\oplus W)\cong\Gamma_{0,0}\oplus\Gamma_{2,1}\oplus S^2\Gamma_{2,1}.
$$

It remains to find the [irreducible representations](../../../../../irreducible-representation.md) in the [symmetric square of the sl3 representation of highest weight (2,1)](../../../../../symmetric-square-of-the-sl3-representation-of-highest-weight-2-1.md). We give the [formal character](../../../../../formal-character-of-a-weight-module.md) calculation explicitly.

Let $E=\mathbb C^3$ be the defining [special linear Lie algebra](../../../../../special-linear-lie-algebra.md) representation. In [Dynkin labels](../../../../../dynkin-label.md), its [weights](../../../../../weight-representation-theory.md) are $(1,0)$, $(-1,1)$, and $(0,-1)$; the [dual representation](../../../../../dual-representation.md) has their negatives. The equivariant contraction

$$
c:S^2E\otimes E^*\longrightarrow E,\qquad c(uv\otimes f)=f(u)v+f(v)u
$$

is surjective. Its [kernel](../../../../../kernel-of-a-linear-map.md) has dimension $18-3=15$. The tensor $e_1^2\otimes e_3^*$ is a [highest-weight vector](../../../../../highest-weight-vector.md) of [highest weight](../../../../../highest-weight-of-a-representation.md) $(2,1)$ in that [kernel](../../../../../kernel-of-a-linear-map.md). By the [Weyl complete reducibility theorem](../../../../../weyl-complete-reducibility-theorem.md), the [kernel](../../../../../kernel-of-a-linear-map.md) contains the [irreducible representation](../../../../../irreducible-representation.md) $\Gamma_{2,1}$, whose [Weyl dimension formula](../../../../../weyl-dimension-formula.md) gives dimension $15$; therefore the [kernel](../../../../../kernel-of-a-linear-map.md) equals $\Gamma_{2,1}$. This yields

$$
\chi_W=\chi_{S^2E}\chi_{E^*}-\chi_E.
$$

Multiplying the six [weights](../../../../../weight-representation-theory.md) of $S^2E$ by the three [weights](../../../../../weight-representation-theory.md) of $E^*$ and subtracting those of $E$ gives the following full [weight multiplicity](../../../../../weight-multiplicity.md) list:

$$
\begin{array}{c|l}
\text{multiplicity}&\text{weights in Dynkin labels}\\\hline
1&(2,1),(3,-1),(2,-2),(1,-3),(0,2),(-1,-2),(-2,3),(-2,0),(-3,2)\\
2&(1,0),(0,-1),(-1,1)
\end{array}
$$

The multiplicities sum to $9+2\cdot3=15$.

For any finite-dimensional [weight-space decomposition](../../../../../weight-space-decomposition.md), a [weight](../../../../../weight-representation-theory.md) $\mu$ of multiplicity $m_\mu$ contributes $m_\mu(m_\mu+1)/2$ to [weight](../../../../../weight-representation-theory.md) $2\mu$ in its [symmetric square](../../../../../symmetric-square.md). Distinct [weights](../../../../../weight-representation-theory.md) $\mu,\nu$ contribute $m_\mu m_\nu$ to $\mu+\nu$. Equivalently,

$$
\chi_{S^2W}(z)=\frac{\chi_W(z)^2+\chi_W(z^2)}{2}.
$$

Applying this to the displayed list gives all dominant [weight multiplicities](../../../../../weight-multiplicity.md) in the second column below. The remaining columns are the [weight multiplicities](../../../../../weight-multiplicity.md) of the candidate [irreducible representations](../../../../../irreducible-representation.md):

$$
\begin{array}{c|r|rrrrr}
\text{weight}&S^2W&\Gamma_{4,2}&\Gamma_{3,1}&\Gamma_{0,4}&\Gamma_{1,2}&\Gamma_{2,0}\\\hline
(4,2)&1&1&0&0&0&0\\
(5,0)&1&1&0&0&0&0\\
(2,3)&1&1&0&0&0&0\\
(3,1)&3&2&1&0&0&0\\
(0,4)&2&1&0&1&0&0\\
(1,2)&5&2&1&1&1&0\\
(2,0)&8&3&2&1&1&1\\
(0,1)&9&3&2&1&2&1
\end{array}
$$

For an explicit way to compute each irreducible column, set $z_1z_2z_3=1$ and use the [Weyl character formula](../../../../../weyl-character-formula.md) in the form

$$
\chi_{a,b}(z_1,z_2,z_3)=
\frac{\det\begin{pmatrix}z_1^{a+b+2}&z_1^{b+1}&1\\z_2^{a+b+2}&z_2^{b+1}&1\\z_3^{a+b+2}&z_3^{b+1}&1\end{pmatrix}}
{\det\begin{pmatrix}z_1^2&z_1&1\\z_2^2&z_2&1\\z_3^2&z_3&1\end{pmatrix}}.
$$

A monomial $z_1^{n_1}z_2^{n_2}z_3^{n_3}$ has [Dynkin labels](../../../../../dynkin-label.md) $(n_1-n_2,n_2-n_3)$. Equivalently, the quotient is enumerated by [Semistandard Young tableaux](../../../../../semistandard-young-tableau.md) of shape $(a+b,b)$ with entries $1,2,3$, weakly increasing across rows and strictly increasing down columns; the exponents count the three entries.

The five irreducible columns sum to the $S^2W$ column. These are all its dominant [weights](../../../../../weight-representation-theory.md), and all five candidate characters have no other dominant [weights](../../../../../weight-representation-theory.md). Every [Weyl group](../../../../../weyl-group.md) orbit meets the dominant chamber, and [weight multiplicities](../../../../../weight-multiplicity.md) are constant on [Weyl group](../../../../../weyl-group.md) orbits. Thus the table proves equality of the full [formal characters](../../../../../formal-character-of-a-weight-module.md), and the [Weyl complete reducibility theorem](../../../../../weyl-complete-reducibility-theorem.md) gives

$$
\boxed{S^2\Gamma_{2,1}\cong\Gamma_{4,2}\oplus\Gamma_{3,1}\oplus\Gamma_{0,4}\oplus\Gamma_{1,2}\oplus\Gamma_{2,0}.}
$$

The [Weyl dimension formula](../../../../../weyl-dimension-formula.md) checks the result:

$$
60+24+15+15+6=120=\frac{15\cdot16}{2}.
$$

Consequently the requested decomposition is

$$
\boxed{S^2(\Gamma_{0,0}\oplus\Gamma_{2,1})\cong\Gamma_{0,0}\oplus\Gamma_{2,1}\oplus\Gamma_{4,2}\oplus\Gamma_{3,1}\oplus\Gamma_{0,4}\oplus\Gamma_{1,2}\oplus\Gamma_{2,0}.}
$$

Its total dimension is $1+15+120=136=16\cdot17/2$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 102](../../paper-102-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
