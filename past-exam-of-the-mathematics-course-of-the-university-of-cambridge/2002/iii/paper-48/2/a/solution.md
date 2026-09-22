<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For real $s$, the multiplier $e^{ias}$ has modulus one and

$$
|ia+\log x|=\sqrt{a^2+\log^2x}.
$$

The [triangle inequality](../../../../../../triangle-inequality.md) applied to the [integral](../../../../../../integral.md) therefore gives

$$
\boxed{|g(s;t,a,\sigma)|\le\frac1a\int_0^\infty
\frac{x^{s+\sigma-1}e^{-tx}}{\sqrt{a^2+\log^2x}}\,dx}.
$$

The hypotheses $s+\sigma>0$ and $t>0$ ensure endpoint convergence. Differentiation in $s$ is justified on compact parameter intervals by integrable bounds with an additional factor $1+|\log x|$. Differentiating both the exponential multiplier and the power of $x$ makes the logarithmic denominator cancel:

$$
\begin{aligned}
g_s(s;t,a,\sigma)
&=-\frac1a e^{ias}\int_0^\infty
\frac{(ia+\log x)x^{s+\sigma-1}e^{-tx}}{ia+\log x}\,dx\\
&=-\frac1a e^{ias}\frac{\Gamma(s+\sigma)}{t^{s+\sigma}}.
\end{aligned}
$$

Here the scaled [Gamma function](../../../../../../gamma-function.md) [integral](../../../../../../integral.md) is obtained by $u=tx$. Integrating this [derivative](../../../../../../derivative.md) from zero to $s$ yields

$$
\boxed{g(0;t,a,\sigma)=\frac1a\int_0^s
 e^{iar}\Gamma(r+\sigma)t^{-r-\sigma}\,dr+g(s;t,a,\sigma)}.
$$

The same modulus bound also gives the useful [parameter-shift remainder bound for a logarithmic Laplace integral](../../../../../../parameter-shift-remainder-bound-for-a-logarithmic-laplace-integral.md)

$$
\boxed{|g(s;t,a,\sigma)|\le\frac{\Gamma(s+\sigma)}{a^2t^{s+\sigma}}},
$$

because the denominator magnitude is at least $a$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
