<h1 id="30k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $V(n,x)=A_n+B_nx+C_nx^2$. The terminal values are $(A_N,B_N,C_N)=(0,0,1)$. Since the noise is centred, backward induction keeps $B_n=0$. Completing the square in the Bellman equation gives

$$
u^*=-\frac{C_n}{1+C_n}x,qquad
C_{n-1}=\frac{C_n}{1+C_n},qquad
A_{n-1}=A_n+C_n\sigma^2.
$$

Hence

$$
\boxed{C_n=\frac1{N-n+1},\quad B_n=0,\quad
A_n=\sigma^2\sum_{j=n+1}^{N}\frac1{N-j+1}}
$$

(with the empty sum equal to zero). This proves the asserted quadratic form of the [value function](../../../../../../value-function.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
