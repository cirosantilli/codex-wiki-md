<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An [isogeny of elliptic curves](../../../../../isogeny-of-elliptic-curves.md) over $k$ is a nonconstant morphism $\phi:E_1\to E_2$ defined over $k$ and preserving the identity. Such a morphism is a [group homomorphism](../../../../../group-homomorphism.md): apply the [Mumford rigidity lemma](../../../../../mumford-rigidity-lemma.md) to $\phi(P+Q)-\phi(P)-\phi(Q)$, whose restriction to either coordinate axis is zero. A nonconstant morphism of [smooth projective curves](../../../../../smooth-projective-curve.md) is finite and surjective, so its [degree of an isogeny](../../../../../degree-of-an-isogeny.md) is the positive integer

$$
\deg\phi=[k(E_1):\phi^*k(E_2)].
$$

Degrees multiply under composition. A [separable isogeny](../../../../../separable-isogeny.md) has degree equal to the number of geometric points in its [kernel of an isogeny](../../../../../kernel-of-an-isogeny.md). In positive [characteristic of a field](../../../../../characteristic-of-a-field.md), inseparable isogenies also occur, for example the [Frobenius isogeny](../../../../../frobenius-isogeny-of-an-elliptic-curve.md); their total degree includes inseparable multiplicity, so counting geometric kernel points alone is insufficient. Every isogeny of degree $d$ has a [dual isogeny](../../../../../dual-isogeny.md) $\widehat\phi$ satisfying $\widehat\phi\phi=[d]$ and $\phi\widehat\phi=[d]$.

Pointwise addition and negation make the [homomorphism group of elliptic curves](../../../../../homomorphism-group-of-elliptic-curves.md) $H=\operatorname{Hom}_k(E_1,E_2)$ an [abelian group](../../../../../abelian-group.md). Its zero is the constant identity map; every other element is an isogeny, because its nonconstant image is the whole target curve. Define $q(0)=0$ and $q(\phi)=\deg\phi$ otherwise. We prove the [positive definiteness of degree on elliptic-curve homomorphisms](../../../../../positive-definiteness-of-degree-on-elliptic-curve-homomorphisms.md), including arbitrary characteristic.

Let $L=\mathcal O_{E_2}(O)$, a [line bundle associated to a divisor](../../../../../line-bundle-associated-to-a-divisor.md) of degree one. On $E_2\times E_2$ write $m(P,Q)=P+Q$, $d(P,Q)=P-Q$ and let $\pi_i$ be the projections. The [divisor proof of the degree parallelogram law](../../../../../divisor-proof-of-the-degree-parallelogram-law.md) gives

$$
m^*L\otimes d^*L\cong\pi_1^*L^{\otimes2}\otimes\pi_2^*L^{\otimes2}.
$$

Here is a direct justification. The degree-two Weierstrass coordinate $x$ has a double pole at $O$, and $x(P)=x(Q)$ precisely when $Q=P$ or $Q=-P$. Consequently

$$
\operatorname{div}(x(P)-x(Q))=D_++D_--2(\{O\}\times E_2)-2(E_2\times\{O\}),
$$

where $D_+$ is the diagonal and $D_-$ the graph of negation. Since $D_+=d^{-1}(O)$ and $D_-=m^{-1}(O)$, this [principal divisor](../../../../../principal-divisor-on-an-algebraic-curve.md) gives the displayed [line bundle](../../../../../line-bundle.md) identity. This remains valid in characteristic two: the general [Weierstrass equation of an elliptic curve](../../../../../weierstrass-equation-of-an-elliptic-curve.md) of a [smooth algebraic curve](../../../../../smooth-algebraic-curve.md) has a nontrivial generic involution $(x,y)\mapsto(x,-y-a_1x-a_3)$, so the two graphs still occur. This identity is also the symmetric-line-bundle form of the [Theorem of the square](../../../../../theorem-of-the-square.md).

Pull back the bundle identity along $(\phi,\psi):E_1\to E_2\times E_2$ and take degrees of [line bundles](../../../../../line-bundle.md). For a nonzero map, $\deg(\phi^*L)=q(\phi)$; for a zero map its pullback is trivial and has degree zero. Thus the [degree parallelogram law](../../../../../divisor-proof-of-the-degree-parallelogram-law.md) is

$$
q(\phi+\psi)+q(\phi-\psi)=2q(\phi)+2q(\psi).
$$

Using bundles rather than pulling back the rational function itself is essential when $\phi=\pm\psi$, where that function can vanish identically. Negation preserves degree, so $q(-\phi)=q(\phi)$. Applying the parallelogram identity to $n\phi$ and $\phi$ gives the [quadratic degree recursion for elliptic multiplication](../../../../../quadratic-degree-recursion-for-elliptic-multiplication.md), and induction from $q(0)=0$ yields $q(n\phi)=n^2q(\phi)$ for every integer $n$.

Define the [bilinear degree pairing for elliptic-curve homomorphisms](../../../../../bilinear-degree-pairing-for-elliptic-curve-homomorphisms.md) by

$$
B(\phi,\psi)=\frac{q(\phi+\psi)-q(\phi-\psi)}4
=\frac{q(\phi+\psi)-q(\phi)-q(\psi)}2.
$$

It is symmetric and odd in each argument. Two applications of the [parallelogram law](../../../../../parallelogram-law.md) give

$$
\begin{aligned}
B(x+z,y)+B(x-z,y)&=2B(x,y),\\
B(x+z,y)-B(x-z,y)&=2B(z,y).
\end{aligned}
$$

Adding proves $B(x+z,y)=B(x,y)+B(z,y)$, and symmetry proves additivity in the other argument. Also $B(\phi,\phi)=q(\phi)$. Therefore $q$ is an integer-valued [quadratic form](../../../../../quadratic-form.md). The integral polarization is $2B(\phi,\psi)=q(\phi+\psi)-q(\phi)-q(\psi)$; $B$ itself may be half-integral.

Finally $q(\phi)>0$ for every nonzero $\phi$, since an isogeny has positive finite degree. If $n\phi=0$ with $n\ne0$, the identity $q(n\phi)=n^2q(\phi)$ forces $\phi=0$, so $H$ is a [torsion-free abelian group](../../../../../torsion-free-abelian-group.md). On any finite-dimensional rational span in $H\otimes\mathbb Q$, the pairing has a rational matrix and is positive on every nonzero rational vector. By density it is nonnegative on real vectors; if that rational matrix were singular, its [kernel](../../../../../kernel-of-a-linear-map.md) would contain a nonzero rational vector, contradicting strict positivity. Thus its real extension is a [positive-definite quadratic form](../../../../../positive-definite-quadratic-form.md). This establishes the required positivity as well as the quadratic identity. For example, on the subgroup of multiplication maps $[n]$, $q([n])=n^2$; on the [endomorphism ring of an elliptic curve](../../../../../endomorphism-ring-of-an-elliptic-curve.md) with [complex multiplication](../../../../../complex-multiplication.md) it is the imaginary-quadratic field norm, explaining the lattice geometry behind isogeny degrees.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
