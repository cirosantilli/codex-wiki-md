<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

Choose an integer $b$ whose reduction is a [primitive root](../../../../../primitive-root-modulo-n.md) modulo $p$. At least one of $b,b+p$ satisfies $g^{p-1}\not\equiv1\pmod {p^2}$, because the [binomial theorem](../../../../../binomial-theorem.md) gives

$$
(b+p)^{p-1}\equiv b^{p-1}+p(p-1)b^{p-2}\pmod {p^2},
$$

and the added coefficient is nonzero modulo $p$. Both choices still generate the multiplicative [group](../../../../../group-split.md) modulo $p$. Choose such a $g$ and write $g^{p-1}=1+up$ with $p\nmid u$.

For $k\geq1$ and $p\nmid v$, another binomial expansion shows

$$
(1+vp^k)^p\equiv1+vp^{k+1}\pmod {p^{k+2}}.
$$

The intermediate binomial coefficients are divisible by $p$, and the final term also has valuation at least $k+2$ because $p$ is odd. Induction therefore gives

$$
v_p(g^{(p-1)p^j}-1)=j+1.
$$

Thus $g^{p-1}$ has order exactly $p^{n-1}$ modulo $p^n$. The order of $g$ itself is divisible by $p-1$, by reduction modulo $p$, and divides the number $p^{n-1}(p-1)$ of invertible residue classes. Its order must consequently be precisely that number. This proves the [lifting a primitive root to odd prime powers](../../../../../lifting-a-primitive-root-to-odd-prime-powers.md) result and

$$
\boxed{(\mathbb Z/p^n\mathbb Z)^\times\text{ is cyclic for every }n\geq1.}
$$

For the requested example choose $g=2$. Modulo $11$, $2^5\equiv-1$ and $2^2\not\equiv1$, excluding the proper divisors $1,2,5$ of ten, so its order is ten. Also $2^{10}-1=1023=11\cdot93$, which is not divisible by $11^2$. Hence

$$
\boxed{a=2\text{ generates }(\mathbb Z/11^n\mathbb Z)^\times\text{ for every }n\geq1.}
$$

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
