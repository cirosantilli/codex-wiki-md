<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [kernel for density estimation](../../../../../kernel-for-density-estimation.md) is an integrable function $K$ with $\int K=1$. The [kernel density estimator](../../../../../kernel-density-estimation.md) is

$$
\widehat f_{n,h,K}(x)
=\frac1{nh}\sum_{i=1}^nK\left(\frac{x-X_i}{h}\right).
$$

It has order $\ell$ when $\int u^jK(u)\,du=0$ for $1\leq j<\ell$ and $\int|u|^\ell|K(u)|\,du<\infty$.

Differentiation gives the [derivative kernel density estimator](../../../../../derivative-kernel-density-estimator.md)

$$
\widehat f_n'(x)=\frac1{nh^2}\sum_{i=1}^nK'\left(\frac{x-X_i}{h}\right).
$$

Dropping the negative square of its mean from the variance and using Tonelli and the substitution $u=(x-X_1)/h$,

$$
\begin{aligned}
\int_{\mathbb R}\operatorname{Var}\widehat f_n'(x)\,dx
&\leq\frac1{nh^4}\int_{\mathbb R}
\mathbb E K'\left(\frac{x-X_1}{h}\right)^2dx\\
&=\frac1{nh^3}\int_{-1}^1K'(u)^2du.
\end{aligned}
$$

Thus $\alpha=3$ and $C_1(K)=\lVert K'\rVert_2^2$.

For $r=\lfloor\beta\rfloor$, the [Nikolsky class](../../../../../nikolsky-class.md) $\mathcal N(\beta,L)$ consists of functions $g$ with square-integrable derivatives through order $r$ and

$$
\lVert g^{(r)}(\mathord\cdot+t)-g^{(r)}\rVert_2
\leq L|t|^{\beta-r},
$$

using the equivalent finite-difference definition when $\beta$ is an integer. Integration by parts shows

$$
\mathbb E\widehat f_n'=K_h*f'.
$$

Taylor expansion in $L^2$, cancellation of the moments through order $\ell-1$ for $\ell=\lceil\beta\rceil$, and the generalized Minkowski inequality give

$$
\lVert K_h*f'-f'\rVert_2
\leq
\frac{Lh^\beta}{r!}\int|u|^\beta|K(u)|\,du.
$$

Consequently

$$
\int_{\mathbb R}\operatorname{Bias}\{\widehat f_n'(x)\}^2dx
\leq C_2(\beta,L,K)h^{2\beta},
$$

where one admissible choice is

$$
C_2(\beta,L,K)
=\frac{L^2}{(r!)^2}
\left(\int|u|^\beta|K(u)|\,du\right)^2.
$$

Hence $\gamma=2\beta$.

The mean integrated squared error is

$$
\operatorname{MISE}(\widehat f_n')
=\mathbb E\int_{\mathbb R}\{\widehat f_n'(x)-f'(x)\}^2dx,
$$

the sum of integrated variance and squared bias. The preceding bounds give

$$
\operatorname{MISE}(\widehat f_n')
\leq\frac{C_1(K)}{nh^3}+C_2(\beta,L,K)h^{2\beta}.
$$

Taking $h\asymp n^{-1/(2\beta+3)}$ proves the [MISE rate for derivative kernel density estimation](../../../../../mise-rate-for-derivative-kernel-density-estimation.md)

$$
\inf_{h>0}\sup_{f:f'\in\mathcal N(\beta,L)}
\operatorname{MISE}(\widehat f_n')
\leq C_3(\beta,L,K)n^{-2\beta/(2\beta+3)}.
$$

Thus $\delta=2\beta/(2\beta+3)$. Estimating a density of the same smoothness has variance order $(nh)^{-1}$ and rate $n^{-2\beta/(2\beta+1)}$; estimating its derivative is harder because differentiation amplifies high-frequency noise, changing $h^{-1}$ to $h^{-3}$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
