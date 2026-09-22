<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Hessian criterion for flexes of a plane cubic](../../../../../../hessian-criterion-for-flexes-of-a-plane-cubic.md) applied to the defining [polynomial](../../../../../../polynomial-split.md) gives

$$
\det\begin{pmatrix}6X&0&0\\0&6Y&0\\0&0&6dZ\end{pmatrix}=216dXYZ.
$$

Consequently the [inflection points of a plane cubic](../../../../../../inflection-point-of-a-plane-cubic.md) on this curve are exactly its intersections with the three coordinate lines. Choose $r\in\overline{\mathbb Q}$ with $r^3=d$, and a primitive cube [root of unity](../../../../../../root-of-unity.md) $\zeta$. The nine distinct [flexes of a diagonal cubic](../../../../../../flexes-of-a-diagonal-cubic.md) are

$$
\boxed{(1:-\zeta^j:0),\quad(0:-r\zeta^j:1),\quad(-r\zeta^j:0:1),\qquad j=0,1,2.}
$$

With the chosen flex as identity, these points are precisely $E_d[3]$. A tangent cutting the [Weil divisor](../../../../../../weil-divisor.md) $3P$ gives $3(P-O)=0$; conversely $3(P-O)=0$ makes the hyperplane [Weil divisor](../../../../../../weil-divisor.md) equivalent to $3P$, which supplies a tangent with triple contact. This is the [three-torsion points are flexes of a plane cubic](../../../../../../three-torsion-points-are-flexes-of-a-plane-cubic.md) correspondence.

On $Z=0$ only $O$ is rational, since the other cube [roots of unity](../../../../../../root-of-unity.md) are not rational. On each other coordinate line a [rational point](../../../../../../rational-point.md) exists exactly when $d$ is a rational cube, and then exactly one does. Therefore

$$
\boxed{E_d(\mathbb Q)[3]\cong\begin{cases}\mathbb Z/3\mathbb Z,&d\in(\mathbb Q^\times)^3,\\0,&\text{otherwise}.\end{cases}}
$$

In particular the rational [torsion subgroup](../../../../../../torsion-subgroup.md) cannot contain two independent points of order $3$.

One can also determine the whole [rational torsion of a diagonal cubic](../../../../../../rational-torsion-of-a-diagonal-cubic.md). First it is killed by $6$. To see this, use the [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) from (iii). At [primes](../../../../../../prime-number.md) $\ell\equiv2\pmod3$ outside the finite set containing $2,3$ and the prime divisors of the numerator and denominator of $d$, the cube map permutes $\mathbb F_\ell$, so

$$
\#E_d(\mathbb F_\ell)=1+\sum_{x\in\mathbb F_\ell}\bigl(1+\chi(x^3-432d^2)\bigr)=\ell+1,
$$

where the quadratic character is extended by $\chi(0)=0$, and the character sum vanishes after substituting $t=x^3-432d^2$. [Reduction of torsion points on an elliptic curve](../../../../../../reduction-of-torsion-points-on-an-elliptic-curve.md) injects the prime-to-$\ell$ part of rational torsion into this [finite group](../../../../../../finite-group.md). This injection follows because multiplication by an [integer](../../../../../../integer.md) [prime](../../../../../../prime-number.md) to $\ell$ is invertible on the [formal group of an elliptic curve](../../../../../../formal-group-of-an-elliptic-curve.md), and hence its reduction kernel has no such torsion.

For any [prime](../../../../../../prime-number.md) $q>3$, choose a good $\ell\equiv2\pmod3$ with $\ell\equiv1\pmod q$; the [Dirichlet theorem on primes in arithmetic progressions](../../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md) and the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) supply such [primes](../../../../../../prime-number.md) outside the finite bad [set](../../../../../../set-split.md). Then $q\nmid\ell+1$, excluding $q$-torsion. Similarly good $\ell\equiv5\pmod{12}$ exclude order $4$, and good $\ell\equiv11\pmod{18}$ exclude order $9$. Thus every rational torsion point has order dividing $6$.

The inversion formula in (i) shows that the only possible nonidentity [rational point](../../../../../../rational-point.md) of order $2$ has $X=Y$ and $Z\ne0$. It exists precisely when $(X/Z)^3=-d/2$, that is, when $d/2$ is a rational cube. There is at most one such point. This condition and $d$ being a cube cannot hold together, since $2$ is not a rational cube. Combining it with the three-torsion calculation gives the full answer:

$$
\boxed{E_d(\mathbb Q)_{\mathrm{tors}}\cong\begin{cases}
\mathbb Z/3\mathbb Z,&d\in(\mathbb Q^\times)^3,\\
\mathbb Z/2\mathbb Z,&d/2\in(\mathbb Q^\times)^3,\\
0,&\text{otherwise}.
\end{cases}}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
