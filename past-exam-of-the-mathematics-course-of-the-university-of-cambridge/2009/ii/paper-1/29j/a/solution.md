<h1 id="29j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $b=(1+r)w_0$, $a=\mu-(1+r)p$ and $d=m-b$. The terminal mean and variance are $b+\theta^{\mathsf T}a$ and $\theta^{\mathsf T}V\theta$. A nonsingular [covariance matrix](../../../../../../covariance-matrix.md) is positive definite. If $a\ne0$, define $D=a^{\mathsf T}V^{-1}a>0$. The [Lagrange multiplier](../../../../../../lagrange-multiplier.md) equations for the fixed-mean constraint give $2V\theta=\lambda a$, and thus

$$
\boxed{\theta^*=\frac{m-b}{D}V^{-1}a,\qquad
\operatorname{var}(w_1)^*=\frac{(m-b)^2}{D}.}
$$

For a direct global proof, every feasible portfolio is $\theta^*+h$ with $a^{\mathsf T}h=0$, so its variance is $d^2/D+h^{\mathsf T}Vh$, minimized uniquely at $h=0$. If $a=0$, only $m=b$ is feasible and its minimum variance is zero, attained by the all-bank portfolio; no other required mean is achievable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29J](../../29j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
