<h1 id="11g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Since $p\ge5$ is odd, $2^p\equiv2\pmod3$ and

$$
N=\frac{4^p-1}{3}=(2^p-1)\frac{2^p+1}{3}
$$

is a product of two odd [integers](../../../../../../integer.md) greater than one. Thus $N$ is odd and composite. Also $2^{2p}=4^p\equiv1\pmod N$. Fermat's theorem modulo $p$ gives $p\mid4^{p-1}-1$, and $p\ne3$, so $p\mid N-1=4(4^{p-1}-1)/3$. This number is even; hence $2p\mid N-1$. Therefore

$$
\boxed{2^{N-1}\equiv1\pmod N,}
$$

proving that $N$ is a base-two [Fermat pseudoprime](../../../../../../fermat-pseudoprime.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11G](../../11g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
