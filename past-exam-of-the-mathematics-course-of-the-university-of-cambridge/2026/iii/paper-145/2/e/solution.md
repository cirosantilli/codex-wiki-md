<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

In an independent-block partition of $P_n$, either $v_1,v_n$ lie in different blocks, giving a partition valid for $C_n$, or they lie in the same block. Contracting those endpoints in the second case gives an independent-block partition of $C_{n-1}$. This bijection proves the recurrence. Multiplying by $x^{\underline k}$ and summing gives

$$
\chi_{P_n}(x)=\chi_{C_n}(x)+\chi_{C_{n-1}}(x).
$$

Using $\chi_{P_n}=x(x-1)^{n-1}$ and induction from $C_2=P_2$ yields

$$
\boxed{\chi_{C_n}(x)=(x-1)^n+(-1)^n(x-1).}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 145](../../../paper-145-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
