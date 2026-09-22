<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work first where all three coordinates are finite and the joining line is not vertical. By the [chord-and-tangent group law](../../../../../../chord-and-tangent-group-law.md), the third intersection of $y=\lambda x+\mu$ with the [elliptic curve](../../../../../../elliptic-curve.md) is $-(P_1+P_2)$, whose first coordinate is also $x_3$. Substitution gives the monic [polynomial](../../../../../../polynomial-split.md)

$$
x^3-\lambda^2x^2+(a-2\lambda\mu)x+(b-\mu^2).
$$

Its roots are $x_1,x_2,x_3$, counted with [intersection multiplicity](../../../../../../intersection-multiplicity.md). Comparing its coefficients with the [elementary symmetric polynomials](../../../../../../elementary-symmetric-polynomial.md) proves

$$
s_1=\lambda^2,\qquad s_2=a-2\lambda\mu,\qquad s_3=\mu^2-b,
\qquad \boxed{(s_2-a)^2=4s_1(s_3+b).}
$$

This [symmetric-coordinate identity for elliptic-curve addition](../../../../../../symmetric-coordinate-identity-for-elliptic-curve-addition.md) is an identity of [rational functions](../../../../../../rational-function.md). It includes tangent cases by specialization. Literally assigning finite $s_i$ when a point is $O$ would be meaningless; such cases must be interpreted on the projective curve. A nonsingular equation in the printed short form has characteristic different from two.

Here is how the identity yields the [quadratic form](../../../../../../quadratic-form.md) for the [degree of an isogeny](../../../../../../degree-of-an-isogeny.md). With $u=x(P)$, $v=x(Q)$, write $s=u+v$ and $q=uv$. As an equation for $t=x(P+Q)$, it becomes

$$
(u-v)^2t^2-\{2s(q+a)+4b\}t+(q-a)^2-4bs=0.
$$

Both $x(P+Q)$ and $x(P-Q)$ satisfy it, because replacing $Q$ by $-Q$ does not change $v$. Thus its two branches are the sum and difference maps. Their common denominator is the square of $u-v$. The following [divisor on an algebraic curve](../../../../../../divisor-on-an-algebraic-curve.md) calculation keeps track of cancellations and exceptional points rigorously, instead of assuming degrees of displayed numerators always add.

On $E_2\times E_2$, equality of the two first coordinates means $Q=P$ or $Q=-P$. Each coordinate has a double pole at $O$. Consequently the [principal divisor](../../../../../../principal-divisor-on-an-algebraic-curve.md) identity is

$$
\operatorname{div}(x(P)-x(Q))
=D_++D_- -2(\{O\}\times E_2)-2(E_2\times\{O\}),
$$

where $D_+$ is the diagonal and $D_-$ is the graph of negation. Equivalently, the two zero divisors are the inverse images of $O$ under difference and sum, exactly the two branches identified above. Their generic multiplicities are one; the divisor identity also accounts for their intersections at [2-torsion](../../../../../../2-torsion.md) points.

For nonzero [isogenies of elliptic curves](../../../../../../isogeny-of-elliptic-curves.md) $\phi,\psi:E_1\to E_2$ with $\phi\ne\pm\psi$, pull this identity back by $(\phi,\psi)$. Taking degrees of the resulting [principal divisor](../../../../../../principal-divisor-on-an-algebraic-curve.md) on $E_1$ gives the [divisor proof of the degree parallelogram law](../../../../../../divisor-proof-of-the-degree-parallelogram-law.md):

$$
\boxed{\deg(\phi+\psi)+\deg(\phi-\psi)=2\deg\phi+2\deg\psi.}
$$

If one map is zero, this is immediate. If $\phi=\pm\psi$, it follows from $\deg([2]\circ\phi)=4\deg\phi$. This also proves the [parallelogram law](../../../../../../parallelogram-law.md) for a general [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) in characteristic two: the same divisor identity uses the quotient by negation, even though the particular symmetric-coordinate formula above is unavailable.

Put $q(\phi)=\deg\phi$ and $q(0)=0$. Applying the [parallelogram law](../../../../../../parallelogram-law.md) to $n\phi,\phi$ gives the recurrence $q((n+1)\phi)+q((n-1)\phi)=2q(n\phi)+2q(\phi)$, and hence $q(n\phi)=n^2q(\phi)$ for every integer $n$. Its polarization $B(\phi,\psi)=q(\phi+\psi)-q(\phi)-q(\psi)$ is symmetric and integer-valued. For fixed $\psi$, the [parallelogram law](../../../../../../parallelogram-law.md) makes $B(\cdot,\psi)$ odd and gives $B(x+y,\psi)+B(x-y,\psi)=2B(x,\psi)$. Interchanging $x,y$ and adding proves additivity, since integers have no two-torsion. Thus $B$ has [bilinearity](../../../../../../bilinearity.md), and $q$ is a positive [quadratic form](../../../../../../quadratic-form.md) on $\operatorname{Hom}(E_1,E_2)$, with $q(\phi)>0$ whenever $\phi\ne0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
