<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [linear congruential generator](../../../../../../linear-congruential-generator.md) starts with an integer seed $S_0\in\{0,\ldots,M-1\}$ and iterates

$$
S_{i+1}=(aS_i+c)\bmod M,\qquad U_i=S_i/M.
$$

The outputs lie in $[0,1)$ and are used as [pseudorandom numbers](../../../../../../pseudorandom-number.md) approximating a [uniform distribution](../../../../../../continuous-uniform-distribution.md). They are deterministic once the seed is fixed. The largest possible period is $M$, since there are only $M$ states; good period alone does not establish [independence](../../../../../../independent-random-variables.md) or good multivariate uniformity.

The [full-period criterion for a mixed congruential generator](../../../../../../full-period-criterion-for-a-mixed-congruential-generator.md) says that period $M$ for every seed occurs exactly when

$$
\boxed{\gcd(c,M)=1,\quad p\mid(a-1)\text{ for every prime }p\mid M,\quad
4\mid M\ \Longrightarrow\ 4\mid(a-1).}
$$

For $M=12^k=2^{2k}3^k$, these conditions reduce to

$$
\boxed{a\equiv1\pmod{12},\qquad \gcd(c,6)=1.}
$$

The multiplier must satisfy both $a\equiv1\pmod3$ and $a\equiv1\pmod4$. A positive shift alone is insufficient: for example, a shift divisible by three cannot give period $M$ when the multiplier is one modulo three. If the required coprime shift has already been chosen, the condition on the multiplier alone is $a=1+12r$ for an integer $r$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
