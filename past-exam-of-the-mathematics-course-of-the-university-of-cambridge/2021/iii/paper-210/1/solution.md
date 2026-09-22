<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A centered random variable is [sub-Gaussian](../../../../../sub-gaussian-distribution.md) with parameter $\sigma^2$ when

$$
\mathbb Ee^{\lambda X}\leq e^{\sigma^2\lambda^2/2}
\qquad(\lambda\in\mathbb R).
$$

For $\lambda>0$, the [Chernoff bound](../../../../../chernoff-bound.md) gives

$$
\mathbb P(X\geq x)\leq
\exp\left(-\lambda x+\frac{\sigma^2\lambda^2}{2}\right).
$$

Minimizing at $\lambda=x/\sigma^2$ yields $e^{-x^2/(2\sigma^2)}$. Applying the same argument to $-X$ proves the left-tail bound.

The moment-generating-function inequality and its version at $-\lambda$ imply

$$
\mathbb E\cosh(\lambda X)\leq e^{\sigma^2\lambda^2/2}.
$$

Comparing the second-order terms as $\lambda\to0$ gives $\mathbb EX^2\leq\sigma^2$. Since $\mathbb EX=0$,

$$
\operatorname{Var}(X)\leq\sigma^2.
$$

A centered $Z$ is [Sub-Gamma random variable in the right tail](../../../../../sub-gamma-random-variable-in-the-right-tail.md) with variance factor $v$ and scale factor $c$ when

$$
\log\mathbb Ee^{\lambda Z}
\leq\frac{v\lambda^2}{2(1-c\lambda)}
\qquad(0<\lambda<c^{-1}).
$$

The corresponding [Bernstein's inequality](../../../../../bernstein-inequalities-probability-theory.md) is

$$
\mathbb P(Z\geq x)
\leq\exp\left(-\frac{x^2}{2(v+cx)}\right).
$$

A standard squared-sub-Gaussian lemma, obtained by integrating the sub-Gaussian tail or expanding exponential moments, states that

$$
X^2-\mathbb EX^2\in\Gamma_+(16\sigma^4,2\sigma^2),
\qquad
\mathbb EX^2-X^2\in\Gamma_+(16\sigma^4,\sigma^2).
$$

Scaling a sub-Gamma variable by $a\geq0$ multiplies its variance factor by $a^2$ and its scale by $a$; independent sums add variance factors and take the largest scale. Decompose

$$
a_i(X_i^2-\mathbb EX_i^2)
=a_i^+(X_i^2-\mathbb EX_i^2)
+a_i^-(\mathbb EX_i^2-X_i^2).
$$

Their sum is therefore sub-Gamma on the right with variance factor

$$
\sigma^4v
=16\sigma^4\{\lVert a^+\rVert_2^2+\lVert a^-\rVert_2^2\}
$$

and scale factor

$$
\sigma^2c
=\sigma^2\max\{2\lVert a^+\rVert_\infty,\lVert a^-\rVert_\infty\}.
$$

Apply Bernstein to the sum at threshold $nx$ to obtain

$$
\boxed{
\mathbb P\left\{\frac1n\sum_{i=1}^na_i(X_i^2-\mathbb EX_i^2)\geq x\right\}
\leq
\exp\left[-\frac{n^2x^2}{2\{\sigma^4v+cn\sigma^2x\}}\right]}.
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
