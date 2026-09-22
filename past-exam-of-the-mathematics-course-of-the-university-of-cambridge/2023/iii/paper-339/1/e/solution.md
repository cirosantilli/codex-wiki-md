<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Choose

$$
\beta=\frac{2\log m}{\epsilon},
$$

so the [smooth maximum](../../../../../../smooth-maximum.md) error is at most $\epsilon/2$ and the [Lipschitz gradient](../../../../../../lipschitz-gradient.md) constant is

$$
L=\frac{2G^2\log m}{\epsilon}.
$$

Suppose a minimizer of $f_\beta$ lies within distance $R$ of the starting point. The [Nesterov accelerated gradient method](../../../../../../nesterov-accelerated-gradient-method.md) can find $x$ such that

$$
f_\beta(x)-\min f_\beta\leq\frac\epsilon2
$$

in

$$
O\left(\sqrt{\frac{LR^2}{\epsilon}}\right)
=O\left(\frac{GR\sqrt{\log m}}{\epsilon}\right)
=O(\epsilon^{-1})
$$

iterations. If $x_*$ minimizes $f$, then the smoothing inequalities imply

$$
\begin{aligned}
f(x)-f(x_*)
&\leq f_\beta(x)-\min f_\beta
+\min f_\beta-f(x_*)\\
&\leq\frac\epsilon2+\frac{\log m}{\beta}
=\epsilon.
\end{aligned}
$$

This improves the nonsmooth [subgradient method](../../../../../../subgradient-method.md) dependence from $O(\epsilon^{-2})$ to $O(\epsilon^{-1})$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
