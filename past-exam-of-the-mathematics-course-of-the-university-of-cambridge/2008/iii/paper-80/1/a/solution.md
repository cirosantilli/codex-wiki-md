<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [exponential-symbol order criterion for a multistep method](../../../../../../exponential-symbol-order-criterion-for-a-multistep-method.md). The exact-solution residual of the [linear multistep method](../../../../../../linear-multistep-method.md) is encoded by $E(z)=\rho(e^z)-z\sigma(e^z)$; vanishing through degree $p$ is equivalent to the [order conditions for a linear multistep method](../../../../../../order-conditions-for-a-linear-multistep-method.md) through order $p$. Here $\rho(1)=0$, $\rho'(1)=\sigma(1)=1-\alpha$, and direct [Taylor expansion](../../../../../../taylor-expansion.md) gives

$$
E(z)=-\frac{1+\alpha}{24}z^4-\frac{17+13\alpha}{360}z^5+O(z^6).
$$

For example, for $n\geq2$ the coefficient of $z^n$ can be calculated as

$$
\frac{2^n-(1+\alpha)}{n!}
-\frac{\tfrac23(1-\alpha)+2^{n-1}(5+\alpha)/12}{(n-1)!}.
$$

For $n=2,3$ this is zero, verifying the lower conditions explicitly. The constant and linear coefficients also vanish for every $\alpha$. Therefore **the formal order is at least three for every $\alpha$**.

The fourth-degree term vanishes exactly when $\alpha=-1$. For that value the fifth-degree coefficient is $-1/90\ne0$, so

$$
\boxed{p=3\text{ if }\alpha\ne-1,\qquad p=4\text{ precisely when }\alpha=-1.}
$$

At $\alpha=1$ these are formal residual conditions only: the [characteristic polynomial](../../../../../../characteristic-polynomial.md) has a double root at one, so the method is not convergent. Canceling its common polynomial factor would change the recurrence and give a different order calculation. This distinction is relevant to part (b).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
