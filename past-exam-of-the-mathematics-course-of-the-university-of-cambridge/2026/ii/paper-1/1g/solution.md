<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

A [primitive root](../../../../../primitive-root-modulo-n.md) modulo $N$ is a unit of order $\varphi(N)$; a nonzero [quadratic residue](../../../../../quadratic-residue.md) modulo an odd prime $p$ is a square.

If a primitive root $g$ modulo $p$ were $x^2$, then its order would divide $(p-1)/2$, the order of the [subgroup](../../../../../subgroup.md) of squares, contradicting $\operatorname{ord}_p(g)=p-1$.

Modulo $11$, $2$ has order $10$, so the primitive roots are $2^k$ for $\gcd(k,10)=1$:

$$
2,\quad 8,\quad 7,\quad 6.
$$

Finally $2^{10}=1024\equiv56\not\equiv1\pmod{121}$, so the lifting criterion makes $2$ primitive modulo $121$. It is plainly the smallest possible positive primitive root.

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
