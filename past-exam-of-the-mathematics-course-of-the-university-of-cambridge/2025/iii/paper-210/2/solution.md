<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [kernel for density estimation](../../../../../kernel-for-density-estimation.md) is an integrable function $K$ with $\int K=1$, usually also bounded and nonnegative, and its scaled version is $K_h(u)=h^{-1}K(u/h)$. For suitable $g_1,g_2$, their [convolution](../../../../../convolution.md) is

$$
(g_1*g_2)(x)=\int_{\mathbb R}g_1(x-u)g_2(u)du.
$$

Because the observations have length-biased density $g(u)=uf(u)/\mu$,

$$
\mathbb E\widehat f_n(x)
=\frac\mu h\int_0^\infty\frac1uK\left(\frac{x-u}{h}\right)
\frac{uf(u)}\mu du
=(K_h*f)(x).
$$

Thus the exact bias is $(K_h*f)(x)-f(x)$, exactly the same as for the ordinary [kernel density estimator](../../../../../kernel-density-estimation.md) based directly on observations from $f$.

Write $R(K)=\int K(u)^2du$. The estimator is the average of $Y_i(x)=\mu X_i^{-1}K_h(x-X_i)$, so

$$
\int\mathbb EY_i(x)^2dx
=\mu^2\mathbb E_g(X_i^{-2})\int K_h^2
=\frac{\mu\bar\mu R(K)}h.
$$

Its mean is $K_h*f$. Integrating the pointwise variance therefore gives

$$
\int\operatorname{Var}\widehat f_n(x)dx
=\frac{\mu\bar\mu R(K)}{nh}
-\frac1n\int(K_h*f)(x)^2dx.
$$

Finally, [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) under density $f$ gives

$$
\mu\bar\mu=\mathbb E_fX\,\mathbb E_f(X^{-1})
\geq(\mathbb E_f1)^2=1.
$$

Equality would require $X$ to be constant almost surely, impossible for a density, so $\mu\bar\mu>1$. The ordinary KDE has the same negative term but leading integrated variance $R(K)/(nh)$; length-biased sampling strictly inflates it.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
