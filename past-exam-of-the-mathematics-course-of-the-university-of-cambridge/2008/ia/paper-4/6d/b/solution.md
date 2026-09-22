<h1 id="6d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take a generator $u$ of the [multiplicative group of a finite field](../../../../../../multiplicative-group-of-a-finite-field.md) $\mathbb F_p^\times$, which has order $p-1$. Write $x=u^a$. Since any possible nonzero base is $y=u^r$, the condition of being a $k$th power is

$$
x=y^k\iff u^a=u^{kr}\iff kr\equiv a\pmod {p-1}.
$$

By part (a), this [linear congruence](../../../../../../linear-congruence.md) is soluble exactly when $d=\gcd(k,p-1)$ divides $a$. Meanwhile

$$
x^{(p-1)/d}=1\iff u^{a(p-1)/d}=1\iff (p-1)\mid a(p-1)/d\iff d\mid a.
$$

Thus the required test is

$$
\boxed{x\text{ is a }k\text{th power in }\mathbb F_p^\times\iff x^{(p-1)/d}\equiv1\pmod p.}
$$

The exponent [residue classes](../../../../../../residue-class.md) divisible by $d$ are $0,d,\ldots,p-1-d$, so there are exactly $(p-1)/d$ distinct nonzero $k$th powers. Equivalently, part (a) shows each value has exactly $d$ preimages under the power map.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6D](../../6d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
