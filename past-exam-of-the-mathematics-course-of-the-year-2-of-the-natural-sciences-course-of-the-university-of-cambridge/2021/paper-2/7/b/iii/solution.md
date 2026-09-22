<h1 id="7/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Substitute $D_N=\beta^N$ into the recurrence. Since $k>0$, its roots are nonzero and satisfy

$$
\beta^2-d\beta+k^2=0,\qquad\boxed{\beta_1+\beta_2=d,\quad\beta_1\beta_2=k^2.}
$$

For distinct roots, the general recurrence solution is $D_N=c_1\beta_1^N+c_2\beta_2^N$. The initial values require $c_1+c_2=1$ and $c_1\beta_1+c_2\beta_2=d=\beta_1+\beta_2$, giving

$$
\boxed{c_1=\frac{\beta_1}{\beta_1-\beta_2},\qquad c_2=-\frac{\beta_2}{\beta_1-\beta_2},\qquad D_N=\frac{\beta_1^{N+1}-\beta_2^{N+1}}{\beta_1-\beta_2}.}
$$

At a repeated root, $d=\pm2k$ and $\beta_1=\beta_2=\beta=\pm k$, this quotient must be replaced by its limit:

$$
\boxed{D_N=(N+1)\beta^N.}
$$

It also follows by solving the repeated-root recurrence as $(c_1+c_2N)\beta^N$. This exceptional case is necessary to avoid introducing a false root in the next part; it is included in the [fixed-end spring-chain determinant and its repeated-root limit](../../../../../../fixed-end-spring-chain-determinant-and-its-repeated-root-limit.md).

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
