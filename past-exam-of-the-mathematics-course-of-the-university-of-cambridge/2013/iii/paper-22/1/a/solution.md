<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the cubic in the [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) as $f(x)=x^3+a_2x^2+a_4x+a_6$. A suitable [invariant differential on an elliptic curve](../../../../../../invariant-differential-on-an-elliptic-curve.md) is

$$
\boxed{\omega=\frac{dx}{2y}.}
$$

It is regular and nonzero wherever $y\ne0$. At a point with $y=0$, nonsingularity gives $f'(x)\ne0$, and differentiating the equation shows $\omega=dy/f'(x)$, again regular and nonzero. At the identity $O$, use the parameter $t=-x/y$: the expansions start $x=t^{-2}+\cdots$, $y=-t^{-3}+\cdots$, so $\omega=(1+\cdots)dt$. Thus it is a nowhere-vanishing regular differential on the whole [smooth projective curve](../../../../../../smooth-projective-curve.md).

Here is a direct proof of [translation invariance of a Weierstrass differential](../../../../../../translation-invariance-of-a-weierstrass-differential.md). Fix $Q=(u,v)$, let $P=(x,y)$ vary, and write $P+Q=(X,Y)$. On the open set where the [chord-and-tangent group law](../../../../../../chord-and-tangent-group-law.md) uses an ordinary chord, put $h=(y-v)/(x-u)$. The addition formulas are $X=h^2-a_2-x-u$ and $Y=h(x-X)-y$. The line-intersection identity is

$$
f(T)-(v+h(T-u))^2=(T-u)(T-x)(T-X).
$$

Differentiate this polynomial in $T$ at $T=x$ to obtain $f'(x)-2yh=(x-u)(x-X)$. Differentiating $h$ along the curve now gives $dh/dx=(x-X)/(2y)$, and hence

$$
\frac{dX}{dx}=2h\frac{dh}{dx}-1=\frac{Y}{y},\qquad\frac{dX}{2Y}=\frac{dx}{2y}.
$$

This proves translation invariance on a dense open set. Since the [translation on an elliptic curve](../../../../../../translation-on-an-elliptic-curve.md) is an automorphism and both sides are regular differentials, it proves invariance everywhere, including the exceptional addition cases. Translation by $O$ is the identity.

Translation invariance also gives $\mu^*\omega=\operatorname{pr}_1^*\omega+\operatorname{pr}_2^*\omega$ for the addition map: its differential on a tangent pair is the sum of the two translated tangent vectors. Therefore **$[j]^*\omega=j\omega$** for every integer $j$.

Let $d_j=\deg[j]$, with the zero endomorphism assigned degree zero. The assumed degree identity, applied to $[j]$ and $[1]$, gives

$$
d_{j+1}+d_{j-1}=2d_j+2,\qquad d_0=0,\quad d_1=1.
$$

Induction gives **$\deg[j]=j^2$** for positive $j$; negation is an automorphism, so the result holds for negative $j$ as well. This is [quadratic degree recursion for elliptic multiplication](../../../../../../quadratic-degree-recursion-for-elliptic-multiplication.md).

For a prime $\ell\ne p$, the [invariant differential on an elliptic curve](../../../../../../invariant-differential-on-an-elliptic-curve.md) has nonzero pullback under $[\ell]$, so that map is a [separable isogeny](../../../../../../separable-isogeny.md). Translation identifies all its fibres and their local multiplicities, so its geometric kernel has exactly its degree $\ell^2$ distinct points. It is killed by $\ell$, and therefore

$$
\boxed{E(\overline{\mathbb F}_p)[\ell]\cong(\mathbb Z/\ell\mathbb Z)^2.}
$$

The [algebraic closure](../../../../../../algebraic-closure.md) is essential here; the assertion is not generally true for the rational-point subgroup over $\mathbb F_p$ itself. This is [prime-to-characteristic geometric torsion](../../../../../../prime-to-characteristic-geometric-torsion.md).

For $[p]$, the pullback differential vanishes. Its total degree is $p^2$, and its inseparable degree is at least $p$, so its kernel has at most $p$ geometric points. Thus $E(\mathbb F_p)[p]$ has dimension at most one over $\mathbb F_p$, while every other prime-torsion subgroup has dimension at most two. The rational-point group is finite and abelian. The structure theorem for [finite abelian groups](../../../../../../finite-abelian-group.md) says that the number of cyclic factors of an $\ell$-primary component equals the dimension of its subgroup killed by $\ell$. Each component therefore has at most two factors. Combining the smaller primary factors into one [cyclic group](../../../../../../cyclic-group.md) and the larger ones into another yields

$$
\boxed{E(\mathbb F_p)\cong\mathbb Z/m\mathbb Z\times\mathbb Z/n\mathbb Z,\qquad m\mid n.}
$$

One may also choose $p\nmid m$, since the $p$-primary component is cyclic. This explains [two generators for elliptic curves over finite fields](../../../../../../two-generators-for-elliptic-curves-over-finite-fields.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
