<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

Since $a=kp\ge2$, we have $a^p\equiv1\pmod{a^p-1}$ and $\gcd(a,a^p-1)=1$. Its [multiplicative order](../../../../../multiplicative-order.md) therefore divides the [prime number](../../../../../prime-number.md) $p$. It cannot be one, because $0<a-1<a^p-1$. Thus **the order is exactly $p$**.

To find the desired prime divisor, use the [cyclotomic polynomial](../../../../../cyclotomic-polynomial.md)

$$
\Phi_p(a)=1+a+\cdots+a^{p-1}>1.
$$

Choose a [prime factor](../../../../../prime-factor.md) $q$ of this integer. Since $p\mid a$, we have $\Phi_p(a)\equiv1\pmod p$, so $q\ne p$. Also $q\nmid a$. If $a\equiv1\pmod q$, then $\Phi_p(a)\equiv p\pmod q$, contradicting $q\ne p$. Consequently $a$ has [multiplicative order](../../../../../multiplicative-order.md) $p$ in the [multiplicative group of a finite field](../../../../../multiplicative-group-of-a-finite-field.md) $\mathbb F_q^\times$. [Lagrange theorem](../../../../../lagrange-s-theorem.md) gives

$$
\boxed{p\mid q-1.}
$$

This $q$ divides $a^p-1$ as required. Notice that order $p$ modulo a composite integer alone would not justify selecting an arbitrary prime divisor; the [cyclotomic polynomial](../../../../../cyclotomic-polynomial.md) selects a suitable one.

If there were only finitely many such primes $q_1,\ldots,q_r$, choose $k=q_1\cdots q_r$, with the empty product interpreted as one. Each $q_i$ divides $a=kp$ and hence does not divide $a^p-1$. The preceding argument supplies a further prime $q\equiv1\pmod p$ dividing that integer, a contradiction. **There are infinitely many primes in this residue class.**

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
