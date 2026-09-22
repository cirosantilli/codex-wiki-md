<h1 id="25i/solution">Solution</h1>

↑ **Parent:** [25I](../25i.md)

For $0\le\alpha<1$, symmetry gives $\mathbb EY_1=0$ and

$$
\mathbb E|Y_1|=2\int_0^\infty\frac{x^\alpha}{\pi(1+x^2)}\,dx<\infty,
$$

because the tail integrand is $O(x^{\alpha-2})$. The [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) for independent identically distributed integrable variables therefore gives $S_n/n\to0$ almost surely and hence in distribution. At $\alpha=0$, $Y_1$ is an equally likely sign, which is included in this argument.

For $\alpha=1$, $Y_1=X_1$ has the standard [Cauchy distribution](../../../../../cauchy-distribution.md). Its [characteristic function](../../../../../characteristic-function.md) is

$$
\varphi(u)=\frac1\pi\int_{\mathbb R}\frac{e^{iux}}{1+x^2}\,dx=e^{-|u|}.
$$

For $u>0$, close a contour in the upper half-plane; the pole at $i$ has residue $e^{-u}/(2i)$ and the semicircle [integral](../../../../../integral.md) vanishes. For $u<0$, symmetry gives the same value with $|u|$, and $u=0$ gives one. Independence now yields $\mathbb Ee^{iuS_n/n}=\varphi(u/n)^n=e^{-|u|}$. Thus $S_n/n$ is exactly standard Cauchy for every $n$. Consequently

$$
\boxed{S_n/n\Rightarrow\delta_0\ (0\le\alpha<1),\qquad
S_n/n\Rightarrow\operatorname{Cauchy}(0,1)\ (\alpha=1).}
$$

For $0\le\alpha<1/2$, the [variance](../../../../../variance-split.md) is finite and equals $\mathbb EY_1^2=2m(2\alpha)$, using the [integral](../../../../../integral.md) notation in the question. The [central limit theorem](../../../../../central-limit-theorem.md) for independent identically distributed variables with finite [variance](../../../../../variance-split.md) gives

$$
\boxed{S_n/\sqrt n\Rightarrow N(0,2m(2\alpha)).}
$$

In particular $m(0)=1/2$ gives [variance](../../../../../variance-split.md) one at $\alpha=0$. The invoked implications from almost-sure to distributional convergence and the characteristic-function uniqueness theorem are the standard probability results used above.

## ↑ Ancestors (10)

1. [25I](../25i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
