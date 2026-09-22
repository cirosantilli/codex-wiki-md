<h1 id="41c/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Eliminating the intermediate vector gives the amplification matrix

$$
\boxed{
\mathbf u^{n+1}=C\mathbf u^n,
\qquad
C=(I+\mu A_x)(I-\mu A_y)^{-1}
}.
$$

The commuting real symmetric matrices admit [simultaneous diagonalization](../../../../../../../simultaneous-diagonalization.md) in the orthonormal basis $v^{(p,q)}$ from the question. On this vector,

$$
\boxed{
c_{pq}=\frac{1+\mu\lambda_p}{1-\mu\lambda_q}
},
\qquad
\lambda_j=-4\sin^2\left(\frac{j\pi h}{2}\right).
$$

Since the basis is orthonormal, stability in the discrete Euclidean norm is equivalent to $|c_{pq}|\leq1$ for every $p,q$.

Put

$$
\alpha=4\sin^2\frac{\pi h}{2},
\qquad
\beta=4\cos^2\frac{\pi h}{2}.
$$

Then $-\beta\leq\lambda_j\leq-\alpha$. The smallest denominator is $1+\mu\alpha$, while the largest numerator modulus occurs at an endpoint of this interval. The condition involving $1-\mu\alpha$ is automatic, and the other is

$$
|1-\mu\beta|\leq1+\mu\alpha.
$$

For $m>1$, this is equivalent to

$$
\mu(\beta-\alpha)\leq2.
$$

Since $\beta-\alpha=4\cos(\pi h)$, the exact finite-grid stability condition is

$$
\boxed{
0<\mu\leq\frac1{2\cos(\pi h)}
}.
$$

For $m=1$ there is only one mode and the method is stable for every $\mu>0$. A simple grid-independent condition, and the limiting condition as $h\to0$, is

$$
\boxed{0<\mu\leq\frac12}.
$$

This is the [stability limit of one-implicit-direction diffusion splitting](../../../../../../../stability-limit-of-one-implicit-direction-diffusion-splitting.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [41C](../../../41c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
