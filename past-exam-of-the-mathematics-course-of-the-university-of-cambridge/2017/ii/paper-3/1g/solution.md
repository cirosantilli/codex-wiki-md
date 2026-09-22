<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

An [Euler pseudoprime](../../../../../euler-pseudoprime.md) is an odd [composite number](../../../../../composite-number.md) $N$ with $\gcd(b,N)=1$ satisfying $b^{(N-1)/2}\equiv(\frac bN)\pmod N$, where the right side is the [Jacobi symbol](../../../../../jacobi-symbol.md). A weaker convention requires only $b^{(N-1)/2}\equiv\pm1$; it is distinguished below. A [strong pseudoprime](../../../../../strong-pseudoprime.md), with $N-1=2^s d$ and $d$ odd, satisfies $b^d\equiv1$ or $b^{2^j d}\equiv-1$ for some $0\leq j<s$.

By the [Chinese remainder theorem for unit groups](../../../../../chinese-remainder-theorem-for-unit-groups.md), the [unit group](../../../../../unit-group.md) modulo $65$ is $C_4\times C_{12}$. Modulo $5$, $b^{32}=1$. Thus the only possible sign in $b^{32}\equiv\pm1\pmod{65}$ is positive. Modulo $13$, writing $b=g^e$ for a [primitive root](../../../../../primitive-root-modulo-n.md), the condition is $12\mid32e$, equivalently $3\mid e$. Consequently $b$ has [multiplicative order](../../../../../multiplicative-order.md) dividing $4$ in each factor. Its square is either $1$ or $-1$ in each factor, but these signs must agree: modulo $5$, the [Legendre symbol](../../../../../legendre-symbol.md) is $1$ for square $1$ and $-1$ for square $-1$, and the same is true modulo $13$. The [Euler pseudoprime](../../../../../euler-pseudoprime.md) condition additionally requires the product of those [Legendre symbols](../../../../../legendre-symbol.md) to be $1$. Hence

$$
\boxed{65\text{ is an Euler pseudoprime to }b\iff b^2\equiv\pm1\pmod{65}.}
$$

Each sign has two roots modulo each [prime](../../../../../prime-number.md), hence four roots modulo $65$. There are **eight [pseudoprime bases](../../../../../pseudoprime-base.md)** modulo $65$ under the [Jacobi symbol](../../../../../jacobi-symbol.md) convention. Under the weaker sign-only convention there are instead sixteen [pseudoprime bases](../../../../../pseudoprime-base.md), since the two signs of the squares need not agree; the stated equivalence therefore specifically uses the [Jacobi symbol](../../../../../jacobi-symbol.md) convention.

For the [strong pseudoprime](../../../../../strong-pseudoprime.md) condition, $s=6,d=1$. Since the [unit group](../../../../../unit-group.md) has [exponent of a finite group](../../../../../exponent-of-a-finite-group.md) $12$, the only possibilities are $b=\pm1$ or $b^2=-1$. The six [pseudoprime bases](../../../../../pseudoprime-base.md) are $1,8,18,47,57,64$. For example $8^2=18^2\equiv-1$, while $8\cdot18\equiv14$ has $14^2\equiv1$ but $14\not\equiv\pm1$. Thus **the strong-pseudoprime [pseudoprime bases](../../../../../pseudoprime-base.md) are not a [subgroup](../../../../../subgroup.md)**.

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
