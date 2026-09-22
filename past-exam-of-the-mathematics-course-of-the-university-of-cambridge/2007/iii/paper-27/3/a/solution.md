<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [isogeny of elliptic curves](../../../../../../isogeny-of-elliptic-curves.md) $\phi:E_1\to E_2$ over a [field](../../../../../../field.md) $K$ is a nonconstant morphism preserving the identity and addition. It is [surjective](../../../../../../surjective-function.md) and finite: its image is a closed connected subgroup, and a nonconstant morphism of [smooth projective curves](../../../../../../smooth-projective-curve.md) is finite. The [degree of an isogeny](../../../../../../degree-of-an-isogeny.md) is the degree of its induced extension of [function fields](../../../../../../function-field-of-an-algebraic-variety.md). A [separable isogeny](../../../../../../separable-isogeny.md) has degree equal to the number of geometric kernel points; in general the degree is the length of the finite kernel scheme, incorporating inseparability. The [degree of an isogeny](../../../../../../degree-of-an-isogeny.md) multiplies under composition, and degree one means an [isomorphism](../../../../../../isomorphism.md). In characteristic zero all [elliptic isogenies](../../../../../../isogeny-of-elliptic-curves.md) are separable. In positive characteristic the [Frobenius isogeny](../../../../../../frobenius-isogeny-of-an-elliptic-curve.md) illustrates inseparability, while an [elliptic isogeny](../../../../../../isogeny-of-elliptic-curves.md) of degree [prime](../../../../../../prime-number.md) to the characteristic is separable.

The [homomorphism group of elliptic curves](../../../../../../homomorphism-group-of-elliptic-curves.md) includes the zero homomorphism, the constant identity map, and every nonzero member is an [elliptic isogeny](../../../../../../isogeny-of-elliptic-curves.md). The operations are pointwise addition and negation; for endomorphisms, composition also gives the [endomorphism ring of an elliptic curve](../../../../../../endomorphism-ring-of-an-elliptic-curve.md). We put $q(0)=0$ and $q(\phi)=\deg\phi$ otherwise. We now prove the [positive definiteness of degree on elliptic-curve homomorphisms](../../../../../../positive-definiteness-of-degree-on-elliptic-curve-homomorphisms.md) in full.

Let $E=E_2$, and choose a [Weierstrass model](../../../../../../weierstrass-equation-of-an-elliptic-curve.md). Its coordinate $x$ has a double pole at $O$, and the generic fibre of $x$ consists of $P$ and $-P$. On $E\times E$ the rational function $x(P)-x(Q)$ therefore has [Weil divisor](../../../../../../weil-divisor.md)

$$
\Delta+\Delta_- -2V-2H,
$$

where $\Delta=\{P=Q\}$, $\Delta_-=\{P=-Q\}$, $V=\{O\}\times E$, and $H=E\times\{O\}$. The generic zeros on the two diagonals have multiplicity one, and the generic poles on $V,H$ have multiplicity two; their intersections have codimension two and add no [Weil divisor](../../../../../../weil-divisor.md) components. This argument also uses the general Weierstrass involution in characteristic $2$, where $-P$ need not mean changing just the sign of $y$.

For the sum and difference maps $a(P,Q)=P+Q$ and $s(P,Q)=P-Q$, the divisors $a^*(O)$ and $s^*(O)$ are $\Delta_-$ and $\Delta$. Consequently, for the degree-one [line bundle](../../../../../../line-bundle.md) $L=\mathcal O_E(O)$,

$$
a^*L\otimes s^*L\cong\operatorname{pr}_1^*(L^{\otimes2})\otimes\operatorname{pr}_2^*(L^{\otimes2}).
$$

Pull back along $P\mapsto(\phi(P),\psi(P))$ and take degrees of [line bundles](../../../../../../line-bundle.md) on $E_1$. A nonconstant map pulls back $L$ to degree equal to its degree, while a constant map pulls it back to a trivial bundle of degree zero. We obtain the [degree parallelogram law](../../../../../../divisor-proof-of-the-degree-parallelogram-law.md)

$$
\boxed{q(\phi+\psi)+q(\phi-\psi)=2q(\phi)+2q(\psi).}
$$

Using the line-bundle identity is important: it still restricts correctly when $\phi=\psi$ or $\phi=-\psi$, when restriction of the displayed rational function would be identically zero.

Since $q(-\phi)=q(\phi)$, applying the identity to $n\phi$ and $\phi$ gives the second-difference recursion

$$
q((n+1)\phi)+q((n-1)\phi)=2q(n\phi)+2q(\phi).
$$

Starting from $q(0)=0$ and $q(\phi)$ yields $q(n\phi)=n^2q(\phi)$ for all [integers](../../../../../../integer.md) $n$. Define

$$
B(\phi,\psi)=\frac{q(\phi+\psi)-q(\phi-\psi)}4
=\frac{q(\phi+\psi)-q(\phi)-q(\psi)}2.
$$

It is symmetric and odd in each variable. Applying the parallelogram identity to the four terms in its first expression gives

$$
B(u+w,v)+B(u-w,v)=2B(u,v).
$$

Interchanging $u,w$ and using oddness also gives $B(u+w,v)-B(u-w,v)=2B(w,v)$. Adding proves $B(u+w,v)=B(u,v)+B(w,v)$; symmetry proves additivity in the other variable. Thus $q$ is a [quadratic form](../../../../../../quadratic-form.md) with associated rational [bilinear form](../../../../../../bilinear-form.md) $B$.

Every nonzero homomorphism has positive degree, so $q(\phi)>0$ for $\phi\ne0$. The scaling identity also shows that the homomorphism [group](../../../../../../group-split.md) is a [torsion-free group](../../../../../../torsion-free-group.md). Hence $q$ extends to its rational [vector space](../../../../../../vector-space-split.md). On the span of any finitely many rationally independent homomorphisms, the matrix of $B$ is rational. Positivity on nonzero rational vectors implies nonnegativity on real vectors by density. If the real matrix had a nontrivial kernel, its rational linear equations would have a nonzero rational solution, contradicting positivity. Thus its real extension is a [positive-definite quadratic form](../../../../../../positive-definite-quadratic-form.md). This establishes the requested positivity as well as the quadratic identities.

An important companion to degree is the [dual isogeny](../../../../../../dual-isogeny.md). Under $E\cong\operatorname{Pic}^0(E)$ via $P\mapsto[P-O]$, the pullback $\phi^*:\operatorname{Pic}^0(E_2)\to\operatorname{Pic}^0(E_1)$ defines $\widehat\phi:E_2\to E_1$. Divisor pushforward corresponds to $\phi$, and pushforward after pullback multiplies [divisor classes](../../../../../../divisor-class.md) by $n=\deg\phi$. Therefore $\phi\widehat\phi=[n]$. Composing shows that $\widehat\phi\phi-[n]$ takes values in the finite kernel of $\phi$; a morphism from a connected smooth curve into this finite scheme must be constant, and its identity value is zero. Thus

$$
\boxed{\widehat\phi\phi=[n],\qquad\phi\widehat\phi=[n],\qquad\deg\widehat\phi=n.}
$$

The last equality follows from $\deg[n]=n^2$, already proved by applying $q(m\phi)=m^2q(\phi)$ to the identity map. The [dual isogeny](../../../../../../dual-isogeny.md) is unique, since the difference of two choices composed with $\phi$ would vanish and $\phi$ is [surjective](../../../../../../surjective-function.md). It follows that being isogenous is an equivalence relation: duality supplies symmetry, and composition supplies transitivity. For a finite subgroup of geometric points of order [prime](../../../../../../prime-number.md) to the characteristic, the quotient curve and its quotient map give an [elliptic isogeny](../../../../../../isogeny-of-elliptic-curves.md) with that kernel; in general one uses finite subgroup schemes. This is the geometric source of explicit descent maps, including the [two-isogeny formula](../../../../../../two-isogeny-formula.md) in Question 4.

Finally [elliptic isogenies](../../../../../../isogeny-of-elliptic-curves.md) preserve the rational [rank of an abelian group](../../../../../../rank-of-an-abelian-group.md) over a [number field](../../../../../../number-field.md). Their dual compositions are multiplication by $n$, so after tensoring the [rational point](../../../../../../rational-point.md) [groups](../../../../../../group-split.md) with $\mathbb Q$ the [elliptic isogeny](../../../../../../isogeny-of-elliptic-curves.md) becomes invertible. For a single curve, its endomorphism algebra in characteristic zero is $\mathbb Q$ or an imaginary quadratic [field](../../../../../../field.md), giving ordinary [integer](../../../../../../integer.md) multiplication or [complex multiplication](../../../../../../complex-multiplication.md). In positive characteristic a supersingular curve can instead have a quaternionic endomorphism algebra. The positive degree form controls the sizes of these homomorphisms, while duality makes their arithmetic and geometric properties accessible.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
