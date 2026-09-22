<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

For every odd [prime](../../../../../prime-number.md) $p$ and $n\geq1$, the [group of units modulo an integer](../../../../../multiplicative-group-of-integers-modulo-n.md) $(\mathbb Z/p^n\mathbb Z)^\times$ is a [cyclic group](../../../../../cyclic-group.md), of order $\varphi(p^n)=p^{n-1}(p-1)$; a generator is a [primitive root](../../../../../primitive-root-modulo-n.md).

Modulo seven, $3,3^2,\ldots,3^6$ are $3,2,6,4,5,1$, so three has order six. Moreover $3^6-1=728=7\cdot104$ is divisible by seven exactly once. We prove the lifting needed here. If $u=1+7^r v$ with $r\geq1$ and $7\nmid v$, the binomial expansion gives $u^7=1+7^{r+1}v+O(7^{r+2})$, so $v_7(u^7-1)=r+1$. Induction therefore gives

$$
v_7(3^{6\cdot7^j}-1)=j+1.
$$

Any exponent giving one modulo $7^n$ is divisible by six. The order also divides $6\cdot7^{n-1}$ by [Lagrange theorem](../../../../../lagrange-s-theorem.md), while the displayed valuation rules out each proper divisor of this form. Consequently **three is a [primitive root](../../../../../primitive-root-modulo-n.md) modulo every $7^n$**.

Since $2^3=1\pmod7$ and two is not one, its order modulo seven is three. A generator modulo $7^n$ would reduce to a generator modulo seven, because reduction is a surjective [group homomorphism](../../../../../group-homomorphism.md). Thus **two is never a [primitive root](../../../../../primitive-root-modulo-n.md) modulo $7^n$**. Finally every unit modulo eight is odd, and $(2k+1)^2=1+4k(k+1)\equiv1\pmod8$. All unit orders are at most two, whereas the unit group has four elements. **There is no [primitive root](../../../../../primitive-root-modulo-n.md) modulo eight.**

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
