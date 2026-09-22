<h1 id="b/6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The curve has [good reduction](../../../../../good-reduction-of-an-elliptic-curve.md) at five and seven: its [discriminant](../../../../../discriminant.md) is $-432D^2$, and the hypotheses make $D$ a [unit](../../../../../unit-in-a-ring.md) at those [primes](../../../../../prime-number-split.md). Over $\mathbb F_5$ the cubing map is a bijection, so

$$
\#E(\mathbb F_5)=1+\sum_{x\in\mathbb F_5}(1+\chi(x^3+D))=6.
$$

The character sum vanishes after replacing $x^3+D$ by a variable ranging over the whole [field](../../../../../field.md). Over $\mathbb F_7$, where $D=2$, the possible cubes are zero once, one three times, and minus one three times. The corresponding right sides are two, three and one. Two and one are nonzero squares while three is not, so the count is $1+2+0+6=9$.

[Rational torsion](../../../../../torsion-subgroup.md) injects into the reduction group at a good odd [prime](../../../../../prime-number-split.md), a standard reduction theorem. Thus its order divides $\gcd(6,9)=3$. If a point of order three existed, its coordinates would be integral by the [Nagell–Lutz theorem](../../../../../nagell-lutz-theorem.md). Since $2P=-P$, the [duplication formula](../../../../../elliptic-curve-group-law-from-riemann-roch.md) gives

$$
\frac{9x^4}{4y^2}-2x=x,\qquad3x(x^3+4D)=0.
$$

Thus either $x=0$ and $y^2=D$, or $x^3=-4D$ and $y^2=-3D$.

At the [prime](../../../../../prime-number-split.md) in the hypothesis, $D$ is a nonsquare [unit](../../../../../unit-in-a-ring.md). Since $p\equiv1\pmod3$, there is a nontrivial cube [root of unity](../../../../../root-of-unity.md) $\zeta\in\mathbb F_p$, and $(2\zeta+1)^2=-3$. Hence $-3$ is a nonzero square, so both $D$ and $-3D$ are nonsquares. Neither ordinate equation is possible even modulo $p$. There is no [rational point](../../../../../rational-point.md) of order three, proving

$$
\boxed{E(\mathbb Q)_{\mathrm{tors}}=\{\mathbf o\}.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
