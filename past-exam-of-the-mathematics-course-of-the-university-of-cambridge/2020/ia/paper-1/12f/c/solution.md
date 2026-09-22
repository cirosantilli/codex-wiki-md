<h1 id="12f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since $Y_1=X_1^2$ and a standard normal variable has second and fourth moments $1$ and $3$,

$$
\boxed{\mu=\mathbb EY_1=1,
\qquad \sigma^2=\operatorname{var}(Y_1)=3-1=2}.
$$

Thus $T_n$ has the [chi-squared distribution](../../../../../../chi-squared-distribution.md) with $n$ degrees of freedom and

$$
V_n=\frac{T_n-n}{\sqrt{2n}}.
$$

[Convergence in distribution](../../../../../../convergence-in-distribution.md) $W_n\Rightarrow W$ means that the [cumulative distribution functions](../../../../../../cumulative-distribution-function.md) satisfy $F_{W_n}(x)\to F_W(x)$ at every continuity point of $F_W$. The [Lévy continuity theorem](../../../../../../levy-continuity-theorem.md) states that this is equivalent to pointwise convergence of [characteristic functions](../../../../../../characteristic-function.md) to the characteristic function of $W$, provided the limiting function is continuous at zero.

For fixed $t$, independence and a Gaussian integral give

$$
\varphi_{V_n}(t)
=\left[e^{-it/\sqrt{2n}}
\left(1-i t\sqrt{\frac2n}\right)^{-1/2}\right]^n.
$$

Using $\log(1-z)=-z-z^2/2+O(z^3)$,

$$
\log\varphi_{V_n}(t)
=n\left[-\frac{it}{\sqrt{2n}}
-\frac12\log\left(1-it\sqrt{\frac2n}\right)\right]
=-\frac{t^2}{2}+O(n^{-1/2}).
$$

Therefore $\varphi_{V_n}(t)\to e^{-t^2/2}$, the characteristic function of the [standard normal distribution](../../../../../../standard-normal-distribution.md). Lévy's theorem now gives

$$
\boxed{V_n\Rightarrow Z}.
$$

This derives the limit directly, without assuming the central limit theorem.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
