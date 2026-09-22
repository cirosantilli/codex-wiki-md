<h1 id="b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Work in $\mathcal O_K=\mathbb Z[\sqrt{-d}]$, since $d\equiv2\pmod4$. First $x$ must be odd: if it were even, coprimality would make $a$ odd, so $x^2+a^2d\equiv2\pmod4$, which cannot be an odd power $y^p$ for $p\ge3$. Thus $y$ is odd too. Also no odd prime $\ell$ can divide both $x$ and $d$. Such a prime does not divide $a$, and square-freeness of $d$ gives $v_\ell(x^2+a^2d)=1$, whereas $v_\ell(y^p)$ is divisible by $p$. Hence $\gcd(x,d)=1$.

Put $\alpha=x+a\sqrt{-d}$. Suppose a [prime ideal](../../../../prime-ideal.md) $P$ divides both $(\alpha)$ and $(\overline\alpha)$, and let $\ell$ be the rational prime below it. It then contains $2x$ and $2a\sqrt{-d}$. The case $\ell=2$ is impossible because $N((\alpha))=y^p$ is odd. If $\ell$ is odd, the first inclusion gives $\ell\mid x$, and $\gcd(a,x)=1$ makes $a$ nonzero in the residue [field](../../../../field.md). The second inclusion therefore gives $\sqrt{-d}\in P$, so $\ell\mid d$, contradicting the previous paragraph. Thus $(\alpha)$ and $(\overline\alpha)$ are coprime [ideals](../../../../ideal.md). In particular they generate the [unit ideal](../../../../unit-ideal.md), the precise meaning of coprimality here; no unique factorization of elements is assumed.

Their product is $(y)^p$. Unique [prime ideal factorization](../../../../prime-ideal-factorization.md) and disjoint prime support imply $(\alpha)=A^p$ for an [integral ideal](../../../../integral-ideal.md) $A$. In the [ideal class group](../../../../ideal-class-group.md), $[A]^p=1$. Since $p$ does not divide the [class number](../../../../class-number.md), [Lagrange's theorem](../../../../lagrange-s-theorem.md) forces $[A]=1$. Write $A=(u+v\sqrt{-d})$. Equality of the principal [ideals](../../../../ideal.md) gives $\alpha=\varepsilon(u+v\sqrt{-d})^p$. The only units are $\pm1$, since a unit satisfies $u^2+dv^2=1$ and $d\ge2$. Both signs are $p$th powers for odd $p$, so they can be absorbed into the generator:

$$
\boxed{x+a\sqrt{-d}=(u+v\sqrt{-d})^p\quad(u,v\in\mathbb Z).}
$$

Apply the [class-number obstruction from a ramified odd exponent](../../../../class-number-obstruction-from-a-ramified-odd-exponent.md). For the equation with $a=1$ and $p\mid d$, compare the coefficients of $\sqrt{-d}$ in this identity. The coefficient on the right is

$$
v\sum_{\substack{1\le j\le p\\j\text{ odd}}}
\binom pj u^{p-j}v^{j-1}(-d)^{(j-1)/2}.
$$

Its $j=1$ term is divisible by $p$, and every $j\ge3$ term contains a factor $d$, so the whole coefficient is divisible by $p$. The coefficient on the left is one, a contradiction. Thus **there are no positive [integer](../../../../integer-split.md) solutions under the stated class-number and divisibility assumptions**.

Finally,

$$
\boxed{13^2+174=7^3.}
$$

The [integer](../../../../integer-split.md) $174=2\cdot3\cdot29$ is square-free, is two modulo four, and is divisible by three. If its imaginary quadratic [class number](../../../../class-number.md) were not divisible by three, the preceding result with $p=3$ would prohibit this solution. Consequently

$$
\boxed{3\mid h(\mathbb Q(\sqrt{-174})).}
$$

## ↑ Ancestors (12)

1. [8](../8.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
