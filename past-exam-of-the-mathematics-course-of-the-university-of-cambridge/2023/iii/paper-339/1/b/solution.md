<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $G=\max_i\|a_i\|_2$. By the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md),

$$
\begin{aligned}
f(x)-f(y)
&\leq\max_i\langle a_i,x-y\rangle\\
&\leq G\|x-y\|_2.
\end{aligned}
$$

Interchanging $x$ and $y$ proves the [Lipschitz bound](../../../../../../lipschitz-bound.md)

$$
\boxed{|f(x)-f(y)|\leq G\|x-y\|_2.}
$$

The [subgradient method](../../../../../../subgradient-method.md) chooses $g_k\in\partial f(x_k)$ and a [step size](../../../../../../step-size.md) $t_k>0$, then sets

$$
\boxed{x_{k+1}=x_k-t_kg_k.}
$$

Assume, as the question's use of $\min f$ requires, that a minimizer $x_*$ exists, and write $R=\|x_0-x_*\|_2$. Since every subgradient here has [Euclidean norm](../../../../../../euclidean-norm.md) at most $G$, the standard best-iterate estimate is

$$
\min_{0\leq j<k}(f(x_j)-f(x_*))
\leq\frac{R^2+G^2\sum_{j<k}t_j^2}{2\sum_{j<k}t_j}.
$$

Taking a suitable constant step when the target accuracy is known, or a standard diminishing sequence, gives error at most $\epsilon$ in

$$
\boxed{O(R^2G^2\epsilon^{-2})=O(\epsilon^{-2})}
$$

iterations, so the requested exponent is $p=2$.

## ↑ Ancestors (11)

1. [B](../b.md)
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
