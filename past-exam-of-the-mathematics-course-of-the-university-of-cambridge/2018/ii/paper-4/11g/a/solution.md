<h1 id="11g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Fermat-Euler theorem](../../../../../../euler-s-theorem.md) states that

$$
\gcd(a,n)=1\quad\Longrightarrow\quad a^{\varphi(n)}\equiv1\pmod n.
$$

Indeed, if $r_1,\ldots,r_{\varphi(n)}$ are the reduced residue classes modulo $n$, multiplication by $a$ permutes them. Therefore

$$
\prod_i ar_i\equiv\prod_i r_i\pmod n.
$$

The product $\prod_i r_i$ is invertible modulo $n$, so cancellation gives the theorem.

Now let $p$ be prime. If $k\equiv1\pmod{p-1}$, then for $p\nmid b$, [Fermat little theorem](../../../../../../fermat-little-theorem.md) gives $b^{k-1}\equiv1\pmod p$, while $p\mid b$ makes $b^k\equiv b\equiv0$. Thus $b^k\equiv b$ for every integer $b$.

Conversely, assume this congruence holds for every $b$. Choose a [primitive root](../../../../../../primitive-root-modulo-n.md) $g$ modulo $p$. Then $g^{k-1}\equiv1\pmod p$. Since $g$ has order $p-1$, one has $p-1\mid k-1$. Hence

$$
\boxed{b^k\equiv b\pmod p\text{ for every }b
\iff k\equiv1\pmod{p-1}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11G](../../11g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
