<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Translate the [rational point](../../../../../../rational-point.md) of order two to $(0,0)$ and complete the square. After clearing denominators by admissible scaling, write

$$
E:y^2=x(x^2+ax+b),\qquad a,b\in\mathbb Z,\qquad b(a^2-4b)\ne0.
$$

The companion curve is $E':Y^2=X(X^2-2aX+a^2-4b)$. The [two-isogeny formula](../../../../../../two-isogeny-formula.md) gives maps $\phi:E\to E'$ and $\psi:E'\to E$ satisfying $\psi\phi=[2]$.

For the [Weak Mordell-Weil theorem](../../../../../../weak-mordell-weil-theorem.md) in this setting, use the [two-torsion square-class homomorphism](../../../../../../two-torsion-square-class-homomorphism.md)

$$
\alpha(O)=1,\quad\alpha((0,0))=[b],\quad\alpha((x,y))=[x]\in\mathbb Q^*/\mathbb Q^{*2},
$$

and its counterpart $\alpha'$ on $E'$. These are homomorphisms: a nonvertical line intersecting the cubic in three points has the product of their $x$-coordinates a square, by comparison of the constant term of the intersection cubic. For a line through $(0,0)$, the product of the other two coordinates is $b$, explaining the special value there. The kernels are $\psi E'(\mathbb Q)$ and $\phi E(\mathbb Q)$, respectively, as follows by solving the [elliptic isogeny](../../../../../../isogeny-of-elliptic-curves.md) preimage quadratic and testing its discriminant for a square.

The [prime-support bound in two-isogeny descent](../../../../../../prime-support-bound-in-two-isogeny-descent.md) makes both images finite. Indeed at a [prime](../../../../../../prime-number.md) not dividing $b$, a negative [valuation](../../../../../../valuation.md) of $x$ makes the leading cubic term dominate, giving $2v(y)=3v(x)$; a positive [valuation](../../../../../../valuation.md) makes $x^2+ax+b$ a unit, giving $2v(y)=v(x)$. In either case $v(x)$ is even. Thus the [square class](../../../../../../square-class.md) of $x$ is supported only on primes dividing $b$, together with a possible sign. The same argument uses $b'=a^2-4b$ on $E'$. Since $2E=\psi\phi E$, the two finite [elliptic isogeny](../../../../../../isogeny-of-elliptic-curves.md) quotients imply that $E(\mathbb Q)/2E(\mathbb Q)$ is finite.

Finite generation still needs a descent on height. Let $h_x$ be the [logarithmic height](../../../../../../absolute-logarithmic-weil-height.md) of the $x$-coordinate. The duplication formula has a degree-four rational $x$-coordinate map with coprime numerator and denominator. Polynomial height estimates, with the resultant supplying the lower bound, give the [height growth under a morphism of the projective line](../../../../../../height-growth-under-a-morphism-of-the-projective-line.md) relation $h_x(2P)=4h_x(P)+O(1)$. Thus the convergent telescoping limit

$$
\widehat h(P)=\tfrac12\lim_{n\to\infty}4^{-n}h_x(2^nP)
$$

defines the [canonical height of an elliptic curve](../../../../../../canonical-height-of-an-elliptic-curve.md), without assuming finite generation. It is nonnegative, satisfies $\widehat h(2P)=4\widehat h(P)$ and the [height parallelogram identity](../../../../../../height-parallelogram-identity.md), and differs from $h_x/2$ by a bounded amount. Consequently its bounded subsets of [rational points](../../../../../../rational-point.md) are finite by the [Northcott theorem](../../../../../../northcott-theorem.md).

Choose the finite list $R_i$ of representatives modulo $2E(\mathbb Q)$ and let $H=\max_i\widehat h(R_i)$. For $P=2Q+R_i$, the [canonical height pairing](../../../../../../canonical-height-pairing.md) inequality gives

$$
\widehat h(Q)=\tfrac14\widehat h(P-R_i)\le\tfrac12\bigl(\widehat h(P)+H\bigr).
$$

Repeated halving brings the height below $H+1$. There are only finitely many such terminal points, and recovering $P$ expresses it as an integer combination of those points and the $R_i$. This proves the [canonical-height proof of Mordell-Weil finite generation](../../../../../../canonical-height-proof-of-mordell-weil-finite-generation.md), so

$$
\boxed{E(\mathbb Q)\cong\mathbb Z^{g_E}\oplus T,\qquad T\text{ finite}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
