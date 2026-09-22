<h1 id="1i/solution">Solution</h1>

↑ **Parent:** [1I](../1i.md)

[Legendre formula](../../../../../legendre-s-formula.md) gives

$$
v_p{2n\choose n}=\sum_{j\geq1}(\lfloor2n/p^j\rfloor-2\lfloor n/p^j\rfloor),
$$

whose summands are zero or one. If the sum is at least $k$, some nonzero summand has index $j\geq k$, whence $p^k\leq p^j\leq2n$.

Grouping the von Mangoldt function by prime gives

$$
\psi(x)=\sum_{p\leq x}\lfloor\log x/\log p\rfloor\log p.
$$

Every prime-power contribution to $\log {2n\choose n}$ occurs in $\psi(2n)$ by the first part. Finally ${2n\choose n}=\prod_{j=1}^n(n+j)/j\geq2^n$, so $\psi(2n)\geq n\log2$.

## ↑ Ancestors (10)

1. [1I](../1i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
