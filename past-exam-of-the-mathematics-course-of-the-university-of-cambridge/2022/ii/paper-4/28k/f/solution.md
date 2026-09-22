<h1 id="28k/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For an exponential proposal of rate $\lambda>0$,

$$
h_\lambda(x)=\lambda e^{-\lambda x}\mathbf1_{x\geq0},
$$

and the smallest valid rejection constant is

$$
\begin{aligned}
M(\lambda)
&=\sup_{x\geq0}\frac{f(x)}{h_\lambda(x)}\\
&=\frac1\lambda\sqrt{\frac2\pi}
\sup_{x\geq0}\exp\left(-\frac{x^2}{2}+\lambda x\right)\\
&=\sqrt{\frac2\pi}\,\frac{e^{\lambda^2/2}}{\lambda},
\end{aligned}
$$

because the exponent is maximized at $x=\lambda$. Differentiating its logarithm gives

$$
\frac d{d\lambda}\log M(\lambda)
=\lambda-\frac1\lambda.
$$

The unique minimum occurs at $\lambda=1$. Since rejection efficiency is $1/M(\lambda)$, choosing any $\lambda\ne1$ makes the algorithm less efficient:

$$
\boxed{\text{the rate-one proposal is optimal within the exponential family}.}
$$

## ↑ Ancestors (11)

1. [F](../f.md)
2. [28K](../../28k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
