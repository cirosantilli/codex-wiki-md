<h1 id="1c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $T_n=n(n+1)/2$, the $n$th [triangular number](../../../../../../triangular-number.md). Pairing the terms of the [arithmetic progression](../../../../../../arithmetic-progression.md) proves $\sum_{r=1}^n r=T_n$. We prove the cube identity by [mathematical induction](../../../../../../mathematical-induction.md). For $n=1$ both sides equal one. If $\sum_{r=1}^n r^3=T_n^2$, then

$$
T_{n+1}^2-T_n^2=\frac{(n+1)^2}{4}\left[(n+2)^2-n^2\right]=(n+1)^3.
$$

Adding $(n+1)^3$ establishes the next case. Thus

$$
\boxed{\sum_{r=1}^n r^3=\left[\frac{n(n+1)}2\right]^2=\left(\sum_{r=1}^n r\right)^2}.
$$

Equivalently, the same displayed difference telescopes from $T_0=0$, providing a direct proof without induction.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1C](../../1c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
