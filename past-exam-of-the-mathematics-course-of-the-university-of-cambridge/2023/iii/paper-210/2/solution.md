<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Put $r=\lceil\beta\rceil-1$ and $\alpha=\beta-r\in(0,1]$. The density Hölder class $\mathcal F(\beta,L)$ consists of nonnegative functions $f$ integrating to one, with derivatives through order $r$, such that

$$
|f^{(r)}(x)-f^{(r)}(y)|\leq L|x-y|^\alpha.
$$

This is the density version of the [Hölder class](../../../../../holder-class.md). A [kernel for density estimation](../../../../../kernel-for-density-estimation.md) is an integrable function $K$ with $\int K=1$. It has order $\ell$ when $\int u^jK(u)\,du=0$ for $1\leq j<\ell$ and $\int|u|^\ell|K(u)|\,du<\infty$.

Choose a bounded kernel of order at least $\lceil\beta\rceil$ with $\int|u|^\beta|K(u)|\,du<\infty$, and use the [kernel density estimator](../../../../../kernel-density-estimation.md)

$$
\widehat f_h(x)=\frac1{nh}\sum_{i=1}^n
K\left(\frac{x-X_i}{h}\right).
$$

Taylor's theorem at $x$ and the vanishing kernel moments cancel every polynomial term below the remainder. Hence, for a constant depending only on $\beta$ and the fixed kernel,

$$
|\mathbb E_f\widehat f_h(x)-f(x)|
\leq C_\beta Lh^\beta.
$$

We also need a uniform density bound. The standard Hölder interpolation argument combines nonnegativity, $\int f=1$, and the Hölder constraint to give

$$
\lVert f\rVert_\infty\leq C_\beta L^{1/(\beta+1)}.
$$

Indeed, near a point where $f$ is close to its maximum $M$, Taylor's theorem and the derivative bounds implied by the Hölder constraint keep $f$ of order $M$ on an interval of length comparable to $(M/L)^{1/\beta}$; integrating over that interval gives $M^{1+1/\beta}\leq C_\beta L^{1/\beta}$.

Using this bound and independence,

$$
\begin{aligned}
\operatorname{Var}_f(\widehat f_h(x))
&\leq\frac1{nh^2}\mathbb E_f
K^2\left(\frac{x-X_1}{h}\right)\\
&\leq\frac{\lVert K\rVert_2^2\lVert f\rVert_\infty}{nh}
\leq\frac{C_\beta L^{1/(\beta+1)}}{nh}.
\end{aligned}
$$

Thus

$$
\sup_x\sup_{f\in\mathcal F(\beta,L)}
\mathbb E_f(\widehat f_h(x)-f(x))^2
\leq C_\beta\left(L^2h^{2\beta}
+\frac{L^{1/(\beta+1)}}{nh}\right).
$$

Choose

$$
h=L^{-1/(\beta+1)}n^{-1/(2\beta+1)}.
$$

Both terms then have order $L^{2/(\beta+1)}n^{-2\beta/(2\beta+1)}$. Since the infimum over all measurable estimators is no larger than the risk of this particular estimator,

$$
\inf_{\widehat f_n}\sup_x\sup_{f\in\mathcal F(\beta,L)}
\mathbb E_f(\widehat f_n(x)-f(x))^2
\leq C_\beta L^{2/(\beta+1)}n^{-2\beta/(2\beta+1)}.
$$

This is the [pointwise minimax rate for Hölder density estimation](../../../../../pointwise-minimax-rate-for-holder-density-estimation.md) upper bound.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
