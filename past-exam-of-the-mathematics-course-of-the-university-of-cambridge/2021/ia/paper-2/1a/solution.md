<h1 id="1a/solution">Solution</h1>

↑ **Parent:** [1A](../1a.md)

The homogeneous [linear recurrence relation](../../../../../linear-recurrence-relation.md)

$$
y_{n+2}-4y_{n+1}+4y_n=0
$$

has characteristic polynomial $(r-2)^2$, so

$$
y_n^{(h)}=(C+Dn)2^n.
$$

For a particular solution, substitute $y_n=an+b$. The left-hand side becomes

$$
an+(b-2a),
$$

so matching $n$ gives $a=1$ and $b=2$. Hence

$$
y_n=(C+Dn)2^n+n+2.
$$

The conditions $y_0=1$ and $y_1=0$ give $C=-1$ and $D=-1/2$. Therefore

$$
\boxed{y_n=n+2-\left(1+\frac n2\right)2^n}.
$$

## ↑ Ancestors (10)

1. [1A](../1a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
