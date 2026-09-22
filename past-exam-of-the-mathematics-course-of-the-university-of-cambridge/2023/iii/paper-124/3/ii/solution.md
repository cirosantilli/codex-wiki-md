<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Split two $2^{k+1}$-digit numbers into high and low halves:

$$
x=aB+c,\qquad y=bB+d,
$$

where $B$ is the base raised to $2^k$. Their product is

$$
xy=abB^2+(ad+bc)B+cd.
$$

The [Karatsuba multiplication](../../../../../../karatsuba-multiplication.md) identity

$$
ad+bc=(a+c)(b+d)-ab-cd
$$

computes the three required half-size products $ab$, $cd$, and $(a+c)(b+d)$, so

$$
f(k+1)\leq3f(k).
$$

Since $f(0)=1$, induction gives $f(k)\leq3^k$. For $n=2^k$,

$$
3^k=n^{\log_2 3}.
$$

Padding an arbitrary input length to the next power of two changes only the constant, yielding $O(n^\alpha)$ digit multiplications with $\alpha=\log3/\log2$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
