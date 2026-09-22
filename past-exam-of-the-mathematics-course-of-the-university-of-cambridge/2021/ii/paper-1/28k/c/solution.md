<h1 id="28k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
S_g=\sum_{x\in\Pi}g(x).
$$

The compact support of $g$ ensures that this sum has only finitely many nonzero terms almost surely. The intensity measure of the ideal gas is

$$
\mu(dx)=z\,dx.
$$

Applying the first-moment identity in [Campbell theorem](../../../../../../campbell-s-theorem.md) gives

$$
\boxed{\mathbb E S_g=z\int_{\mathbb R^3}g(x)\,dx}.
$$

For the second moment, separate equal and distinct particles:

$$
\begin{aligned}
\mathbb E S_g^2
&=\mathbb E\sum_{x\in\Pi}g(x)^2
+\mathbb E\sum_{\substack{x,y\in\Pi\\x\ne y}}g(x)g(y)\\
&=z\int_{\mathbb R^3}g(x)^2\,dx
+z^2\left(\int_{\mathbb R^3}g(x)\,dx\right)^2.
\end{aligned}
$$

Subtracting $(\mathbb ES_g)^2$ yields

$$
\boxed{\operatorname{Var}(S_g)
=z\int_{\mathbb R^3}g(x)^2\,dx}.
$$

These are the mean and variance formulas in Campbell's theorem for a homogeneous Poisson point process.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28K](../../28k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
