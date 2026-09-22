<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $D=\sum_pr_pp\in X^{(d)}$. The [derivative of the Abelian sum map](../../../../../derivative-of-the-abelian-sum-map.md) is most naturally stated using [principal parts](../../../../../principal-part-of-a-meromorphic-function.md). The [tangent space](../../../../../tangent-space.md) of the [symmetric product of a curve](../../../../../symmetric-product-of-a-curve.md) at $D$ is $H^0(\mathcal O_D(D))$, and the [tangent space](../../../../../tangent-space.md) of the [Jacobian variety](../../../../../jacobian-variety.md) is $H^0(K_X)^*$. With these identifications,

$$
\boxed{(d u_d)_D(v)(\omega)=\sum_p\operatorname{res}_p(v_p\omega),\qquad \omega\in H^0(K_X).}
$$

Its dual is restriction of [holomorphic one-forms](../../../../../holomorphic-one-form.md) to the length-$d$ [divisor](../../../../../divisor.md) scheme. In particular,

$$
\boxed{\ker(d u_d)_D^*=H^0(K_X(-D)),\qquad
\operatorname{rank}(d u_d)_D=g-h^0(K_X(-D))=d+1-h^0(\mathcal O_X(D)).}
$$

The last equality is the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md). These formulas apply to repeated points as well as distinct ones.

Here is a direct proof of the [repeated-point Abel differential formula](../../../../../repeated-point-abel-differential-formula.md). At a multiplicity-$r$ point, choose a [local coordinate](../../../../../local-coordinate.md) $t$ with $t(p)=0$. A nearby local [divisor](../../../../../divisor.md) is described by the roots $t_1,\ldots,t_r$, or, without making an ordering choice, by their elementary symmetric functions $e_1,\ldots,e_r$:

$$
\prod_{i=1}^r(t-t_i)=t^r-e_1t^{r-1}+e_2t^{r-2}-\cdots+(-1)^re_r.
$$

These $e_k$ are smooth [local coordinates](../../../../../local-coordinate.md) on the [symmetric product of a curve](../../../../../symmetric-product-of-a-curve.md), including at the repeated [divisor](../../../../../divisor.md). Under a first-order deformation, minus the logarithmic variation of this defining polynomial is the [principal part](../../../../../principal-part-of-a-meromorphic-function.md)

$$
v_p=\sum_{k=1}^r(-1)^{k-1}\delta e_k\,t^{-k}\pmod{\mathcal O_{X,p}}.
$$

The sign can be checked at $r=1$: moving the point from $0$ to $\epsilon a$ gives $v=a/t$, and the Abel integral changes by $a\omega(p)$.

Write $\omega=(\sum_{j\ge0}c_jt^j)dt$ and its local primitive as $F(t)=\sum_{j\ge0}c_jt^{j+1}/(j+1)$. The local contribution to the [Abelian sum map](../../../../../abel-map-of-an-algebraic-curve.md) is $\sum_i F(t_i)$. [Newton's identities](../../../../../newton-s-identities.md), linearized at $e_1=\cdots=e_r=0$, give

$$
d\!\left(\sum_i t_i^k\right)=(-1)^{k-1}k\,de_k\quad(1\le k\le r),
\qquad d\!\left(\sum_i t_i^k\right)=0\quad(k>r).
$$

Substituting in the primitive therefore gives

$$
d\!\left(\sum_iF(t_i)\right)=\sum_{k=1}^r(-1)^{k-1}c_{k-1}\,de_k
=\operatorname{res}_p(v_p\omega).
$$

Summing over the support proves the theorem. In particular, a multiplicity-$r$ point tests the first $r$ coefficients of a [holomorphic one-form](../../../../../holomorphic-one-form.md), not just its value. The [residue](../../../../../residue.md) pairing between [principal parts](../../../../../principal-part-of-a-meromorphic-function.md) of order at most $r$ and differential jets through order $r-1$ is perfect. Thus the annihilator of the derivative is precisely the [holomorphic one-forms](../../../../../holomorphic-one-form.md) vanishing to order at least $r_p$ at every $p$, namely $H^0(K_X(-D))$.

There is also a [sheaf cohomology](../../../../../sheaf-cohomology.md) description that explains its [kernel](../../../../../kernel-of-a-linear-map.md) geometrically. The sequence

$$
0\longrightarrow\mathcal O_X\longrightarrow\mathcal O_X(D)\longrightarrow\mathcal O_D(D)\longrightarrow0
$$

gives a [connecting homomorphism](../../../../../connecting-homomorphism.md) $\delta:H^0(\mathcal O_D(D))\to H^1(\mathcal O_X)$. Represent a [principal part](../../../../../principal-part-of-a-meromorphic-function.md) by [meromorphic](../../../../../meromorphic-function.md) lifts on coordinate disks; their differences on overlaps give its [Čech cohomology](../../../../../cech-cohomology.md) class. Under [Serre duality](../../../../../serre-duality.md), pairing this class with $\omega$ is the sum of the [residues](../../../../../residue.md) of $v_p\omega$, so $\delta$ is the displayed derivative. Exactness shows that its [kernel](../../../../../kernel-of-a-linear-map.md) is $H^0(\mathcal O_X(D))/\mathbb C$, of dimension $h^0(\mathcal O_X(D))-1$, in agreement with the tangent directions to the [complete linear system of a divisor](../../../../../complete-linear-system-of-a-divisor.md) in Solution 2.

Two consequences will be useful below. If $d\ge2g-1$, then $K_X(-D)$ has negative degree and no nonzero sections, so $u_d$ is a [submersion](../../../../../submersion.md) everywhere. Its image is open, and it is also closed because $X^{(d)}$ is [compact](../../../../../compact-space.md). Since the [Jacobian variety](../../../../../jacobian-variety.md) is connected, $u_d$ is surjective. Thus the points $u(p)$ generate the [Jacobian variety](../../../../../jacobian-variety.md) as a group. Together with [Abel's theorem](../../../../../abel-theorem-for-divisors.md), this identifies the degree-zero [Picard group](../../../../../picard-group.md) with the [Jacobian variety](../../../../../jacobian-variety.md): every [line bundle](../../../../../line-bundle.md) has a [meromorphic](../../../../../meromorphic-function.md) section and thus a [divisor](../../../../../divisor.md) representation, injectivity is [Abel's theorem](../../../../../abel-theorem-for-divisors.md), and surjectivity follows from $u_d(D)-d u(p_0)$.

For $g\ge1$, one can choose $g-1$ distinct points imposing independent conditions on $H^0(K_X)$: at each step a surviving nonzero [holomorphic one-form](../../../../../holomorphic-one-form.md) has only finitely many zeros, so choose a point where it does not vanish. Their sum $D$ has $h^0(K_X(-D))=1$ and hence $h^0(\mathcal O_X(D))=1$. The derivative has [rank](../../../../../rank-one-quadratic-form.md) $g-1$ there. Consequently $W_{g-1}=u_{g-1}(X^{(g-1)})$ is an [irreducible](../../../../../irreducible-representation.md) subvariety of dimension $g-1$. This also covers $g=1$, when $X^{(0)}$ and $W_0$ are points.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
