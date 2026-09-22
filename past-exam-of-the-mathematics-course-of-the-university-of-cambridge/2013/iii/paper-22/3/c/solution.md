<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Lutz–Nagell theorem](../../../../../../nagell-lutz-theorem.md) says that for a nonsingular short equation $y^2=x^3+ax+b$ with $a,b\in\mathbb Z$, every nonidentity rational [torsion point of an elliptic curve](../../../../../../torsion-point-of-an-elliptic-curve.md) $(x,y)$ has $x,y\in\mathbb Z$, and either $y=0$ or

$$
\boxed{y^2\mid 4a^3+27b^2.}
$$

This is a necessary condition for torsion, not a converse.

To prove integrality, fix a prime $q$. If $v_q(x)<0$, the $x^3$ term dominates the right side of the equation. Hence $2v_q(y)=3v_q(x)$, so $v_q(x)=-2s$, $v_q(y)=-3s$ for some $s\ge1$. The parameter $t=-x/y$ has valuation $s$ and identifies the point with the formal neighbourhood of the identity, namely the [formal group of an elliptic curve](../../../../../../formal-group-of-an-elliptic-curve.md) evaluated on $q\mathbb Z_q$.

For odd $q$, this group is a [torsion-free group](../../../../../../torsion-free-group.md) by the logarithm argument of Question 2. For $q=2$, use the special short-model structure. Negation sends $t$ exactly to $-t$, so the formal multiplication series $[2](t)$ is odd and has integral coefficients:

$$
[2](t)=2t+t^3g(t),\qquad g(t)\in\mathbb Z_2[[t]].
$$

If $s=v_2(t)\ge1$, the first term has valuation $s+1$ and all the others have valuation at least $3s>s+1$. Thus $v_2([2](t))=s+1$, and no iteration of doubling kills a nonzero point. Multiplication by an odd integer has unit linear coefficient and also cannot kill it. This proves the [torsion-free formal subgroup for a short Weierstrass equation](../../../../../../torsion-free-formal-subgroup-for-a-short-weierstrass-equation.md), including at two. Consequently a rational [torsion point of an elliptic curve](../../../../../../torsion-point-of-an-elliptic-curve.md) cannot have $v_q(x)<0$ at any prime. Its $x$ is integral, and the equation then makes its rational $y$ integral too.

For the divisibility conclusion suppose $y\ne0$. Then $2P\ne O$ and is also a rational [torsion point of an elliptic curve](../../../../../../torsion-point-of-an-elliptic-curve.md), so $x(2P)$ is integral. Its tangent slope $\lambda=f'(x)/(2y)$ satisfies $x(2P)=\lambda^2-2x$. Thus $\lambda^2\in\mathbb Z$; a rational number with integral square is itself integral. In particular $y^2\mid f'(x)^2$. Reduce the supplied polynomial identity modulo $y^2=f(x)$: both terms on the left are divisible by $y^2$, so the right side $4a^3+27b^2$ is too. This is the [divisibility proof in the Nagell–Lutz theorem](../../../../../../divisibility-proof-in-the-nagell-lutz-theorem.md).

For the specific curve, $4a^3+27b^2=3^7 5^4$. The computed equality $2P_1=-P_1$ makes $P_1$ a point of exact order three. The coordinate $y(P_3)=17$ has square not dividing $3^7 5^4$, so $P_3$ has infinite order. To decide $P_2$, use the already computed point $P_1+P_2=(15,-60)$. Its $y$-coordinate has even square, which cannot divide the odd number $3^7 5^4$, so that sum has infinite order. Since $P_1$ is torsion, $P_2$ must have infinite order as well. **$P_1$ has order three; $P_2$ and $P_3$ both have infinite order.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
