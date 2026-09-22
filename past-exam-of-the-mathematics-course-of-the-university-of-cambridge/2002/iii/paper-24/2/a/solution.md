<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Move the nonidentity rational [2-torsion](../../../../../../2-torsion.md) point to $T=(0,0)$ and complete the square. After a rational change of coordinates, the [elliptic curve](../../../../../../elliptic-curve.md) has an integral model

$$
E:y^2=x(x^2+ax+b),\qquad b(a^2-4b)\ne0.
$$

The [two-isogeny formula](../../../../../../two-isogeny-formula.md) gives a partner

$$
E':Y^2=X\bigl(X^2-2aX+b'\bigr),\qquad b'=a^2-4b,
$$

and the [isogeny of elliptic curves](../../../../../../isogeny-of-elliptic-curves.md) and its [dual isogeny](../../../../../../dual-isogeny.md) are

$$
\phi(x,y)=\left(x+a+\frac bx,\ y\left(1-\frac b{x^2}\right)\right),\qquad
\widehat\phi(X,Y)=\left(\frac{X-2a+b'/X}{4},\ \frac{Y(1-b'/X^2)}8\right).
$$

Both extend at the exceptional points; their kernels are the identities and the distinguished [2-torsion](../../../../../../2-torsion.md) points, and $\widehat\phi\phi=[2]$.

The [two-torsion square-class homomorphism](../../../../../../two-torsion-square-class-homomorphism.md) is $\alpha(O)=1$, $\alpha(T)=[b]$, and $\alpha(x,y)=[x]$ otherwise, with values in $\mathbb Q^*/\mathbb Q^{*2}$. Its kernel is $\widehat\phi E'(\mathbb Q)$. Define $\alpha'$ on the partner in the same way. By the [prime-support bound in two-isogeny descent](../../../../../../prime-support-bound-in-two-isogeny-descent.md), representatives are signed squarefree divisors $d$ of $b$, or of $b'$ for the partner. A class is realized precisely when its [quartic covering in a two-isogeny descent](../../../../../../quartic-covering-in-a-two-isogeny-descent.md) has a rational solution:

$$
N^2=dU^4+aU^2V^2+\frac bd V^4,\qquad \gcd(U,V)=1.
$$

For $UV\ne0$, this comes from $x=d(U/V)^2$ and $y=dUN/V^3$; the cases $U=0$ or $V=0$ account for the distinguished point and the identity. Test this finite list using signs and local congruences, and exhibit rational solutions for the surviving classes. The [local-to-global gap in isogeny descent](../../../../../../local-to-global-gap-in-isogeny-descent.md) matters: local solubility gives an upper bound from the [isogeny Selmer group](../../../../../../isogeny-selmer-group.md), so a rank determination requires matching actual classes or further descent, not merely declaring every locally soluble cover to have a rational point.

Once the two actual images are determined, the [two-isogeny rank formula](../../../../../../square-class-index-formula-for-two-isogeny-descent.md) is

$$
\boxed{2^r=\frac{|\alpha E(\mathbb Q)|\,|\alpha'E'(\mathbb Q)|}{4}.}
$$

For completeness, put $A=E(\mathbb Q)$ and $B=E'(\mathbb Q)$. The [Mordell-Weil theorem](../../../../../../mordell-weil-group.md) gives $[A:2A]=2^r|A[2]|$. The [index of a subgroup](../../../../../../index-of-a-subgroup.md) formula through $\widehat\phi B$ gives

$$
[A:2A]=|\alpha A|\,|\alpha'B|\big/[\ker\widehat\phi:\ker\widehat\phi\cap\phi A].
$$

Here $\ker\widehat\phi\cap\phi A=\phi(A[2])$, since $\widehat\phi\phi=[2]$, and this image has size $|A[2]|/2$. The denominator is therefore $4/|A[2]|$, proving the displayed [rank of an elliptic curve](../../../../../../rank-of-an-elliptic-curve.md) formula.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
