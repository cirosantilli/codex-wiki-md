<h1 id="19/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [root limit of a finite sum of powers](../../../../../../root-limit-of-a-finite-sum-of-powers.md). Put $M=\max\{1,a,a^2/2\}\geq1$. For every $x>0$, at least one of the three terms is $M^x$ and none is larger, so

$$
M^x\leq1+a^x+(a^2/2)^x\leq3M^x.
$$

Taking the positive $x$th root gives

$$
M\leq\left(1+a^x+(a^2/2)^x\right)^{1/x}\leq3^{1/x}M.
$$

Since $3^{1/x}\to1$, the [squeeze theorem](../../../../../../squeeze-theorem.md) gives

$$
\boxed{\lim_{x\to\infty}\left(1+a^x+(a^2/2)^x\right)^{1/x}=\begin{cases}1,&0\leq a\leq1,\\a,&1<a\leq2,\\a^2/2,&a>2.\end{cases}}
$$

Indeed, for $a\leq1$ both remaining bases are at most $1$; for $1\leq a\leq2$, $a\geq a^2/2$; and for $a\geq2$, $a^2/2\geq a$. The endpoint cases $a=0,1,2$ are included in the same bound.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [19](../../../19.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
