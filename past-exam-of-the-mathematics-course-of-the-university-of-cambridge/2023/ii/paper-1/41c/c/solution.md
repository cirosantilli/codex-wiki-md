<h1 id="41c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The first two modified stages give

$$
\widetilde{\mathbf u}^{n+1}
=(I+\mu A_x)(I-\mu A_y)^{-1}\mathbf u^n.
$$

The correction stage is

$$
(I-\mu A_x)\mathbf u^{n+1}
=\widetilde{\mathbf u}^{n+1}-\mu A_x\mathbf u^n.
$$

Using $A_xA_y=A_yA_x$,

$$
\begin{aligned}
\widetilde{\mathbf u}^{n+1}-\mu A_x\mathbf u^n
&=\left[(I+\mu A_x)(I-\mu A_y)^{-1}-\mu A_x\right]\mathbf u^n\\
&=(I+\mu^2A_xA_y)(I-\mu A_y)^{-1}\mathbf u^n.
\end{aligned}
$$

Therefore

$$
\boxed{
\mathbf u^{n+1}=D\mathbf u^n,
\qquad
D=(I-\mu A_x)^{-1}
(I+\mu^2A_xA_y)
(I-\mu A_y)^{-1}
}.
$$

On the common eigenvector $v^{(p,q)}$, the eigenvalue of $D$ is

$$
\boxed{
d_{pq}
=\frac{1+\mu^2\lambda_p\lambda_q}
{(1-\mu\lambda_p)(1-\mu\lambda_q)}
}.
$$

Set $a=-\mu\lambda_p>0$ and $b=-\mu\lambda_q>0$. Then

$$
d_{pq}=\frac{1+ab}{(1+a)(1+b)}.
$$

Both numerator and denominator are positive, and

$$
(1+a)(1+b)-(1+ab)=a+b>0.
$$

Hence

$$
0<d_{pq}<1
$$

for every mode and every $\mu>0$. Orthogonal diagonalization now gives $\|D\|_2<1$, so the method is stable without a time-step restriction. This is the [unconditionally stable corrected directional diffusion splitting](../../../../../../unconditionally-stable-corrected-directional-diffusion-splitting.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [41C](../../41c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
