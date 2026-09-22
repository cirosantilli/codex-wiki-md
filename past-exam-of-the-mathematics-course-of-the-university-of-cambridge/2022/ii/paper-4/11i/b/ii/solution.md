<h1 id="11i/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $N=\lfloor\sqrt x\rfloor$ and form

$$
P=\prod_{\lceil N/2\rceil\leq n\leq N}(n^2-2).
$$

For sufficiently large $x$, every factor is positive and at most $x$. Every odd prime divisor $p$ of $P$ makes $2$ a [quadratic residue](../../../../../../../quadratic-residue.md) modulo $p$, so part (a) gives $p\equiv1$ or $7\pmod8$.

For an odd prime power $p^a$, the congruence $n^2\equiv2\pmod{p^a}$ has at most two residue classes, because each root modulo $p$ is simple and lifts uniquely. Therefore

$$
v_p(P)
\leq
\sum_{a\geq1}2\left(\frac N{p^a}+1\right)
\leq
\frac{2N}{p-1}+\frac{2\log x}{\log p}.
$$

Since $\log p/(p-1)\leq\log3/2$ for odd $p$,

$$
v_p(P)\log p\leq N\log3+2\log x.
$$

The prime $2$ contributes at most $N\log2$, because $v_2(n^2-2)\leq1$. If

$$
K=\pi_1(x)+\pi_7(x)+1,
$$

then, for all sufficiently large $x$, $2\log x\leq N\log3/2$ and hence

$$
\log P\leq\frac32KN\log3.
$$

On the other hand, the product contains at least $N/3$ factors for large $N$, and every one satisfies

$$
n^2-2\geq\frac{N^2}{4}-2\geq x^{3/4}
$$

once $x$ is sufficiently large. Thus

$$
\log P\geq\frac N3\cdot\frac34\log x
=\frac N4\log x.
$$

Comparing the two estimates gives

$$
\boxed{
\pi_1(x)+\pi_7(x)+1
=K
\geq\frac{\log x}{6\log3}
}
$$

for every sufficiently large $x$. This is the [elementary logarithmic lower bound for primes in the quadratic-residue classes of two](../../../../../../../elementary-logarithmic-lower-bound-for-primes-in-the-quadratic-residue-classes-of-two.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [11I](../../../11i.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
