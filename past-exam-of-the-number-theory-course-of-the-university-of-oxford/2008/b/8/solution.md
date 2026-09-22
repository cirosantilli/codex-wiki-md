<h1 id="b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

For [integral solutions of x squared minus two equals y cubed](../../../../integral-solutions-of-x-squared-minus-two-equals-y-cubed.md), the equation implies $y\ge-1$, so $y+2>0$. If $y$ were even, then $x$ would be even and $x^2-2$ would be two or six modulo eight, whereas $y^3$ would be zero modulo eight. Thus $y$ and $x$ are odd. Also $3\nmid x$: otherwise $x^2-2\equiv7\pmod9$, which is not a cubic residue modulo nine. Reducing modulo three then gives $y\equiv2\pmod3$. Consequently

$$
\boxed{\gcd(y+2,6)=1.}
$$

Put $\eta=\sqrt{-6}$ and $\alpha=x+(y+1)\eta$. Its [field norm](../../../../field-norm.md) is $(y+2)^3$. The [principal ideals](../../../../principal-ideal.md) $(\alpha)$ and $(\bar\alpha)$ are coprime. Indeed a common [prime ideal](../../../../prime-ideal.md) has underlying rational prime $p$ dividing $y+2$. The displayed gcd excludes two and three, so both two and $\eta$ are invertible modulo that [prime ideal](../../../../prime-ideal.md). The difference $\alpha-\bar\alpha=2(y+1)\eta$ therefore implies $p\mid y+1$, contradicting $p\mid y+2$.

Their product is $(y+2)^3$, so [unique factorization of ideals in a number field](../../../../unique-factorization-of-ideals-in-a-number-field.md) and coprimality imply $(\alpha)=A^3$ for an [integral ideal](../../../../integral-ideal.md) $A$. In the given [ideal class group](../../../../ideal-class-group.md) of order two, $[A]^3=1$ implies $[A]=1$. Hence $A=(u+v\eta)$ with [integers](../../../../integer-split.md) $u,v$. Equality of [principal ideals](../../../../principal-ideal.md) gives $\alpha=\varepsilon(u+v\eta)^3$. The only [units](../../../../unit-in-a-ring.md) are $\pm1$, and both are cubes, so the sign can be absorbed into $u,v$. Taking [norms](../../../../norm.md), and using $y+2>0$, gives

$$
\boxed{x+(y+1)\eta=(u+v\eta)^3,\qquad u^2+6v^2=y+2.}
$$

The coefficient of $\eta$ gives $y+1=3u^2v-6v^3$. Eliminating $y$ with the [field norm](../../../../field-norm.md) identity yields

$$
(3v-1)u^2=6v^3+6v^2-1,\qquad u^2=\frac{6v^3+6v^2-1}{3v-1}.
$$

The denominator is nonzero for integral $v$. [Polynomial](../../../../polynomial-split.md) division makes the integrality obstruction especially clear:

$$
\boxed{9u^2=18v^2+24v+8-\frac1{3v-1}.}
$$

If $u$ is integral, the reciprocal must be an [integer](../../../../integer-split.md), forcing $3v-1=\pm1$. The only integral possibility is $v=0$. Then $u^2=1$, the [field norm](../../../../field-norm.md) gives $y=-1$, and the real coefficient in the cube gives $x=u^3=\pm1$. Both pairs directly satisfy the original equation. Therefore all integral solutions are

$$
\boxed{(x,y)=(1,-1),\ (-1,-1).}
$$

## ↑ Ancestors (12)

1. [8](../8.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
