<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Equality $(\alpha)=(\beta)$ gives $\alpha=u\beta$ and $\beta=v\alpha$ for some $u,v\in\mathcal O_K$. Substitution and cancellation of the nonzero $\alpha$ yield $uv=1$. Thus $u$ is a unit and $\alpha=u\beta$.

For the [ideal](../../../../ideal.md)-power assertion, suppose first that all ideals are nonzero. A [prime ideal](../../../../prime-ideal.md) divides at most one $Q_i$ because the $Q_i$ are pairwise coprime. Taking its valuation in the given equality gives

$$
n_i v_P(Q_i)=k v_P(A).
$$

Since $\gcd(n_i,k)=1$, every exponent $v_P(Q_i)$ is divisible by $k$. Dividing all its prime-factorization exponents by $k$ constructs an [integral ideal](../../../../integral-ideal.md) $I_i$ with $Q_i=I_i^k$. If a $Q_i$ is zero, pairwise coprimality forces all other $Q_j$ to be the unit [ideal](../../../../ideal.md); taking $I_i=0$ and the other $I_j=\mathcal O_K$ covers that degenerate case too.

For the first Diophantine equation, $x$ cannot be odd: then $x^2+17\equiv2\pmod8$, while a cube modulo eight is $0$ or odd. Hence $x$ is even and $y$ is odd. Also $17\nmid x$, since otherwise $v_{17}(x^2+17)=1$, impossible for a cube.

In $\mathcal O=\mathbb Z[s]$, $s=\sqrt{-17}$, factor

$$
(x+s)(x-s)=y^3.
$$

The two principal ideals are coprime. A common [prime ideal](../../../../prime-ideal.md) would divide their sum $2x$ and difference $2s$, and hence lie above $2$ or $17$; odd [norm](../../../../norm.md) excludes $2$, while $17\nmid x$ excludes $17$. Their coprime product is the cube $(y)^3$, so the [ideal](../../../../ideal.md)-power assertion makes $(x+s)=I^3$. The class [group](../../../../group-split.md) has order $4$, while $[I]^3=1$, so $[I]=1$. Write $I=(a+bs)$ for integers $a,b$.

The only units are $\pm1$, since their [norm](../../../../norm.md) equation is $a^2+17b^2=1$. Equality of principal ideals therefore gives $x+s=\pm(a+bs)^3$. Absorb the sign into $a+bs$. Comparing the coefficient of $s$ yields

$$
b(3a^2-17b^2)=1.
$$

Thus $b=1$ or $-1$. The first gives $a^2=6$ and the second gives $3a^2=16$, both impossible for an [integer](../../../../integer-split.md) $a$. Consequently **the first equation has no integral solutions**.

For the product equation, odd $x$ gives $(x^2+17)(9x^2+17)\equiv4\pmod8$, again not a cube. If $17\mid x$, each factor has $17$-adic valuation one, so the product has valuation two, also impossible. Thus any hypothetical solution has $x$ even and $17\nmid x$. The two positive factors are odd, and their greatest common divisor divides

$$
(9x^2+17)-9(x^2+17)=-136=-8\cdot17.
$$

It must therefore be one. A product of coprime positive integers is a cube only if each factor is a cube. This would make $x^2+17$ a cube, contradicting the result already proved. Hence **the product equation also has no integral solutions**.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
