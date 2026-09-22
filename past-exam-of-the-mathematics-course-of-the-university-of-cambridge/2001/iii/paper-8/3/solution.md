<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take a real modulus $0<k<1$ and complementary modulus $k'=\sqrt{1-k^2}$. The [Jacobi elliptic sine](../../../../../jacobi-elliptic-sine.md) is constructed by inverting a [Schwarz-Christoffel mapping](../../../../../schwarz-christoffel-mapping.md). The main reason for the Schwarz-Christoffel [derivative](../../../../../derivative.md) is local angle behavior: if a [prevertex](../../../../../prevertex-of-a-schwarz-christoffel-map.md) $a_j$ corresponds to a [polygon](../../../../../polygon.md) angle $\pi\alpha_j$, straightening that corner gives $U(w)-U(a_j)\sim C_j(w-a_j)^{\alpha_j}$. Hence $U'$ has exponent $\alpha_j-1$. Along each straight boundary side its argument is constant. Dividing $U'$ by $\prod_j(w-a_j)^{\alpha_j-1}$ removes those angle changes; [Schwarz reflection](../../../../../schwarz-reflection-principle.md) extends the quotient across the real boundary and the corner singularities. With all vertices finite, its behavior at infinity is also regular, because the sum of the [derivative](../../../../../derivative.md) exponents is $-2$. It is therefore a nonzero constant on the sphere. This yields

$$
U'(w)=C\prod_j(w-a_j)^{\alpha_j-1}.
$$

This argument explains the exponents, the branch choices and the role of boundary reflection, rather than just writing down the formula.

For a [rectangle](../../../../../rectangle.md), four angles are $\pi/2$, so choose prevertices $-1/k,-1,1,1/k$ and normalize the inverse map as

$$
U(w)=\int_0^w\frac{dt}{\sqrt{(1-t^2)(1-k^2t^2)}}.
$$

Use the branch positive on $(-1,1)$. Set

$$
K=\int_0^1\frac{dt}{\sqrt{(1-t^2)(1-k^2t^2)}},\qquad K'=K(k').
$$

The two middle corner values are $U(\pm1)=\pm K$. The right side length is

$$
\int_1^{1/k}\frac{dt}{\sqrt{(t^2-1)(1-k^2t^2)}}=K',
$$

as the substitution $t=(1-k'^2s^2)^{-1/2}$ shows. The selected branch makes the increment along that side $iK'$. Thus the other corner values are $K+iK'$ and $-K+iK'$. The two boundary intervals through infinity have combined horizontal length $2K$; the substitution $t=1/(ks)$ gives length $K$ from $1/k$ to infinity. In particular $U(\infty)=iK'$. As in the [square](../../../../../square.md) mapping, the boundary goes once around a [rectangle](../../../../../rectangle.md), and the [argument principle](../../../../../argument-principle.md) gives a [conformal](../../../../../conformal-map.md) [bijection](../../../../../bijection.md)

$$
U:\mathbb H\longrightarrow\{-K<\operatorname{Re}z<K,\quad0<\operatorname{Im}z<K'\}.
$$

Its inverse $s(z)=\operatorname{sn}(z,k)$ maps that [rectangle](../../../../../rectangle.md) onto the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md), and near zero has $s(0)=0$, $s'(0)=1$. Differentiating the inverse relation gives

$$
(s')^2=(1-s^2)(1-k^2s^2),\qquad s''=-(1+k^2)s+2k^2s^3.
$$

These identities continue meromorphically.

All four [rectangle](../../../../../rectangle.md) edges have real images, so [Schwarz reflection](../../../../../schwarz-reflection-principle.md) extends $s$ across them. Reflection in the bottom edge gives $s(\bar z)=\overline{s(z)}$. Reflection in the right edge, combined with the first reflection, gives $s(2K-z)=s(z)$. The even inverse-integral [derivative](../../../../../derivative.md) gives $s(-z)=-s(z)$, and hence

$$
s(z+2K)=-s(z),\qquad s(z+4K)=s(z).
$$

Reflection in the top edge and then the bottom gives $s(z+2iK')=s(z)$. The resulting [period lattice of the Jacobi elliptic sine](../../../../../period-lattice-of-the-jacobi-elliptic-sine.md) is

$$
\boxed{\Lambda=4K\mathbb Z+2iK'\mathbb Z}.
$$

To see the [poles](../../../../../pole.md), use $U'(w)\sim-1/(kw^2)$ near the boundary point infinity. Then $U(w)-iK'\sim1/(kw)$, so the inverse has a [simple pole](../../../../../simple-pole.md) at $iK'$ with [residue](../../../../../residue.md) $1/k$. The real half-period shift gives another [pole](../../../../../pole.md) at $2K+iK'$ with opposite [residue](../../../../../residue.md). Reflection tiles the plane with copies of the [rectangle](../../../../../rectangle.md), so these are exactly two [simple poles](../../../../../simple-pole.md) per displayed fundamental cell. They also show there is no additional period: a period must permute these two [pole](../../../../../pole.md) classes; exchanging them would shift by $2K$ modulo the displayed lattice, which reverses the function's sign and [residues](../../../../../residue.md) rather than preserving it.

For any finite $w$, integrate $s'(z)/(s(z)-w)$ around a [fundamental parallelogram](../../../../../fundamental-parallelogram-of-a-period-lattice.md) avoiding its zeros and [poles](../../../../../pole.md). The opposite edges cancel by periodicity, so the number of zeros of $s-w$ equals the number of [poles](../../../../../pole.md), namely two. Therefore **every value has two inverse images modulo periods, counted with multiplicity**. The value infinity likewise has the two [simple poles](../../../../../simple-pole.md) as preimages. Usually the finite-value preimages are distinct; the involution $z\mapsto2K-z$ interchanges them. At $w=\pm1,\pm1/k$, a critical point supplies one double inverse image instead. For example $s(K)=1$, $s'(K)=0$, $s''(K)=-(1-k^2)\ne0$. Thus the printed “exactly two” requires the standard multiplicity convention; it would be false if interpreted as two distinct solutions at these [branch values of a holomorphic map](../../../../../branch-value-of-a-holomorphic-map.md).

Now choose $z_0=K$ and put $f(z)=s(z+K)$. Since $s(2K-z)=s(z)$, $f$ is even, elliptic for $\Lambda$, and has degree two. The [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) for the same lattice is even and has one [double pole](../../../../../double-pole.md) per cell, hence also degree two. Its generic fibers are precisely $\{z,-z\}$. Consequently an even $f$ is constant on those fibers and descends to a [meromorphic function](../../../../../meromorphic-function.md) $R$ of $\wp$. At the four fixed classes of $z\mapsto-z$, the even local Laurent expansion makes this descent [meromorphic](../../../../../meromorphic-function.md) in the squared local coordinate. A [meromorphic function](../../../../../meromorphic-function.md) on the [Riemann sphere](../../../../../riemann-sphere.md) is rational, so $f=R(\wp)$. Generic map degrees multiply:

$$
2=\deg f=\deg R\,\deg\wp=2\deg R.
$$

Thus $R$ has degree one and the [degree-two even elliptic function](../../../../../degree-two-even-elliptic-function.md) conclusion is

$$
\boxed{\operatorname{sn}(z+K,k)=\frac{a\wp(z)+b}{c\wp(z)+d},\qquad ad-bc\ne0}.
$$

The [determinant](../../../../../determinant.md) condition follows because $f$ is nonconstant. This proves the existence requested, with the explicit allowable shift $z_0=K$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
