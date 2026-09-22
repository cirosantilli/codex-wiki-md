<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $X$ be a [smooth projective curve](../../../../../smooth-projective-curve.md) over $\mathbb C$, let $D=\sum_p m_pp$ be an effective [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) of degree $d$, and identify a translate of the [Jacobian variety](../../../../../jacobian-variety.md) with $\operatorname{Pic}^d(X)$. The precise derivative theorem is

$$
\boxed{T_DX^{(d)}=H^0(X,\mathcal O_D(D)),\qquad d u_d|_D=\delta_D,}
$$

where $\delta_D$ is the [connecting homomorphism](../../../../../connecting-homomorphism.md) of

$$
0\longrightarrow\mathcal O_X\longrightarrow\mathcal O_X(D)\longrightarrow\mathcal O_D(D)\longrightarrow0.
$$

The target is $T_{u_d(D)}\operatorname{Jac}(X)=H^1(X,\mathcal O_X)=H^0(X,K_X)^*$ under [Serre duality](../../../../../serre-duality.md). Its dual is restriction of [holomorphic differential forms](../../../../../holomorphic-differential-form.md) to the length-$d$ [closed subscheme](../../../../../closed-subscheme.md) $D$:

$$
(d u_d|_D)^*:H^0(K_X)\longrightarrow H^0(K_X|_D).
$$

In particular, this includes derivatives of the local coefficients at repeated points, rather than simply evaluating once for each point of the support.

Here is a local proof of all these identifications. Near a point of multiplicity $m$, take a coordinate $z$ vanishing at that point. Nearby effective [divisors](../../../../../divisor.md) are represented by monic polynomials of degree $m$. A first-order deformation has equation

$$
z^m-\varepsilon v(z)=0,\qquad v(z)=v_0+v_1z+\cdots+v_{m-1}z^{m-1},\qquad\varepsilon^2=0.
$$

These coefficients are the elementary symmetric coordinates on the [symmetric product of a curve](../../../../../symmetric-product-of-a-curve.md); they give $m$ independent tangent directions even at a repeated point. Dividing the variation of the equation by the original equation identifies the tangent direction with the [principal part](../../../../../principal-part-of-a-meromorphic-function.md) $v(z)/z^m$. Doing this at each point gives $H^0(\mathcal O_D(D))$, a space of dimension $d$.

To see the derivative of the [line bundle](../../../../../line-bundle.md) directly, use the local frame $1/(z^m-\varepsilon v)$ for $\mathcal O_X(D_\varepsilon)$ and the frame $1$ outside the small disks. Relative to the frame $1/z^m$ at $\varepsilon=0$, its transition multiplier changes by

$$
\frac{z^m}{z^m-\varepsilon v}=1+\varepsilon\frac{v}{z^m}.
$$

First-order changes of [line bundle](../../../../../line-bundle.md) transition functions have the form $1+\varepsilon c_{ij}$; changing frames adds a [Čech coboundary](../../../../../cech-coboundary.md). Thus the tangent space to the [Picard group](../../../../../picard-group.md) is $H^1(\mathcal O_X)$, and the derivative is exactly the [Čech cocycle](../../../../../cech-cocycle-condition.md) of these [principal parts](../../../../../principal-part-of-a-meromorphic-function.md), namely $\delta_D$.

This agrees with differentiating the Abel integrals, including the sign. If $\omega=f(z)\,dz$ and $F'=f$, the sum of $F$ at the roots of $z^m-\varepsilon v$ has derivative

$$
\operatorname{res}_{z=0}\left(\frac{v(z)}{z^m}\omega\right).
$$

For example, expand $F=\sum_{k\ge1}f_{k-1}z^k/k$. The first-order Newton identities give $\partial_\varepsilon\sum z_i^k=k v_{m-k}$ for $1\le k\le m$, and zero for $k>m$, yielding exactly the [residue](../../../../../residue.md) above. Equivalently the same formula follows by differentiating the contour integral for the sum over roots. [Serre duality](../../../../../serre-duality.md) pairs the [principal part](../../../../../principal-part-of-a-meromorphic-function.md) class with $\omega$ by the sum of these [residues](../../../../../residue.md). Locally this pairing is perfect between the [principal parts](../../../../../principal-part-of-a-meromorphic-function.md) $z^{-1},\ldots,z^{-m}$ and the jets $1,z,\ldots,z^{m-1}$ times $dz$. This proves the asserted dual restriction map.

The [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) now gives the kernel and rank without any reduced-support assumption:

$$
\ker(d u_d|_D)=H^0(\mathcal O_X(D))/\mathbb C,\qquad
\boxed{\operatorname{rank}(d u_d|_D)=d+1-h^0(\mathcal O_X(D)).}
$$

By duality,

$$
\boxed{\operatorname{im}(d u_d|_D)=H^0(K_X(-D))^\perp.}
$$

This is the geometric form of the [derivative of the Abelian sum map](../../../../../derivative-of-the-abelian-sum-map.md). For distinct points, the image is spanned by the evaluation vectors of the [canonical map](../../../../../canonical-map.md); at repeated points, the corresponding osculating directions must also be included. The [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) confirms the rank as $g-h^0(K_X(-D))$. When $h^0(D)=1$, the [Abelian sum map](../../../../../abel-map-of-an-algebraic-curve.md) is an immersion at $D$. For $d=g-1$ and $h^0(D)=1$, its image is a hyperplane annihilated by the unique nonzero [holomorphic differential form](../../../../../holomorphic-differential-form.md) vanishing along $D$, which will be the tangent hyperplane to the [theta divisor](../../../../../theta-divisor.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
