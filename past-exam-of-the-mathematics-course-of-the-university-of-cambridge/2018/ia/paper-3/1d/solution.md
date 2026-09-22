<h1 id="1d/solution">Solution</h1>

↑ **Parent:** [1D](../1d.md)

Composing the [permutation cycles](../../../../../permutation-cycle.md) from right to left gives

$$
(13)(2457)(815)=(1\,7\,2\,4\,5\,8\,3),
$$

with $6$ fixed. It therefore has **order $7$** and, as a seven-cycle, **sign $(-1)^6=+1$**.

An element of $S_6$ has order $6$ precisely for cycle type $(6)$ or $(3,2,1)$. These contribute

$$
\frac{6!}{6}=120,\qquad
\binom63(3-1)!\binom32=120,
$$

so there are **$240$ elements of order $6$**. Order $3$ has cycle type $(3,1,1,1)$ or $(3,3)$, contributing

$$
\binom63(3-1)!=40,\qquad \frac{6!}{3^2\,2!}=40,
$$

so there are **$80$ elements of order $3$**.

Inspecting the partitions of $9$ shows that the largest cycle-length least common multiple available in $S_9$ is $20$, from the partition $5+4$, but such a permutation is odd. Among integers from $16$ through $20$, orders $17$ and $19$ would require cycles of those prime lengths, order $16$ requires a cycle length divisible by $16$, and order $18$ requires disjoint cycles using at least $9+2>9$ letters. The disjoint product of a five-cycle and a three-cycle is even and has order $15$. Hence **the greatest order in $A_9$ is $15$**.

## ↑ Ancestors (10)

1. [1D](../1d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
