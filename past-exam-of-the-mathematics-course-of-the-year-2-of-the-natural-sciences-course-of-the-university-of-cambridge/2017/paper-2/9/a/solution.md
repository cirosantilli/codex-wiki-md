<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $A(a,b,c)$ with $a$ in entry $(1,2)$, $b$ in entry $(1,3)$ and $c$ in entry $(2,3)$, and perform all arithmetic in the [finite field](../../../../../finite-field.md) $\mathbb F_5$. Direct multiplication gives

$$
\boxed{A(a,b,c)A(a',b',c')=A(a+a',\ b+b'+ac',\ c+c').}
$$

Thus the set is closed. [Associativity](../../../../../associative-property.md) comes from [matrix multiplication](../../../../../matrix-multiplication.md). The [identity element](../../../../../identity-element.md) is $A(0,0,0)$, and solving the product formula for it gives

$$
\boxed{A(a,b,c)^{-1}=A(-a,\ ac-b,\ -c).}
$$

Both orders of multiplication with this inverse give the identity. Hence these matrices form a [finite group](../../../../../finite-group.md), an instance of the [Heisenberg group over a prime field](../../../../../heisenberg-group-over-a-prime-field.md). Each coordinate has five independent possibilities, with distinct triples giving distinct matrices, so

$$
\boxed{|G|=5^3=125.}
$$

The explicit coordinate convention matters because the central coordinate is $b$ here; other descriptions of the [Heisenberg group over a prime field](../../../../../heisenberg-group-over-a-prime-field.md) may place the central coordinate last.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
