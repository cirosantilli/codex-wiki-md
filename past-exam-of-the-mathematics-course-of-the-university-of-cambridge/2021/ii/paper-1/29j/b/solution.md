<h1 id="29j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $f_\theta(x)$ for the joint density and assume regularity permits differentiation under the [integral](../../../../../../integral.md). Since

$$
\int f_\theta(x)\,dx=1,
$$

one differentiation gives

$$
\mathbb E_\theta S_n(\theta)
=\int \frac{\partial_\theta f_\theta}{f_\theta}f_\theta\,dx
=\partial_\theta\int f_\theta\,dx=0.
$$

Differentiating the score itself,

$$
\partial_\theta S_n
=\frac{\partial_\theta^2f_\theta}{f_\theta}
-\left(\frac{\partial_\theta f_\theta}{f_\theta}\right)^2.
$$

Taking expectation gives

$$
\begin{aligned}
\mathbb E_\theta[\partial_\theta S_n(\theta)]
&=\int\partial_\theta^2f_\theta(x)\,dx
-\mathbb E_\theta[S_n(\theta)^2]\\
&=-I_n(\theta).
\end{aligned}
$$

Thus the [information identity](../../../../../../information-identity.md) is

$$
\boxed{I_n(\theta)
=-\mathbb E_\theta\!\left[
\frac{\partial}{\partial\theta}S_n(\theta)
\right]
=-\mathbb E_\theta[\ell_n''(\theta)]}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29J](../../29j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
