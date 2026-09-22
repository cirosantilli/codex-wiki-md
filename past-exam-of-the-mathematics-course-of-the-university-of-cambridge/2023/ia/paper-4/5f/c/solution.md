<h1 id="5f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $z=2\cos(\pi/n)$. The recurrence

$$
S_0(z)=2,\quad S_1(z)=z,\quad S_{k+1}(z)=zS_k(z)-S_{k-1}(z)
$$

defines monic integer [polynomials](../../../../../../polynomial-split.md) and gives $S_k(z)=2\cos(k\pi/n)$. Hence $z$ is an algebraic integer. If $\cos(\pi/n)$ is rational, then the rational algebraic integer $z$ is an integer. Since $-2\leq z<2$, this leaves the values corresponding to

$$
n=1:\cos\pi=-1,\qquad n=2:\cos(\pi/2)=0,\qquad n=3:\cos(\pi/3)=\frac12.
$$

This is the [rational cosine of an integral submultiple of pi](../../../../../../rational-cosine-of-an-integral-submultiple-of-pi.md) result. For every $n\geq4$, the value lies strictly between $1/2$ and $1$, so it is irrational.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5F](../../5f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
