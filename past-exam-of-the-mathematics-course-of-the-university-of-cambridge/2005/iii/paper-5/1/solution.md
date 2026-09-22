<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For [conjugate exponents](../../../../../conjugate-exponents.md) $p,q\in[1,\infty]$, $1/p+1/q=1$, [Hölder's inequality](../../../../../holder-s-inequality.md) states that $\int|fg|\leq\|f\|_p\|g\|_q$. If $r=\infty$ in the requested product estimate, every $p_i=\infty$ and multiplication of essential bounds proves it directly. Suppose $r<\infty$. Factors with $p_i=\infty$ can again be bounded pointwise by their [essential suprema](../../../../../essential-supremum.md).

Here is an explicit finite-exponent proof of the remaining [Generalized Holder inequality](../../../../../generalized-holder-inequality.md). Put $q_i=p_i/r$, so $\sum_i1/q_i=1$, and normalize $h_i=|f_i|^r/\|f_i\|_{p_i}^r$. If one [norm](../../../../../norm.md) is zero the product vanishes [almost everywhere](../../../../../almost-everywhere.md). Otherwise $\int h_i^{q_i}=1$. The weighted [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md), applied to $h_i^{q_i}$ with weights $1/q_i$, gives

$$
\prod_i h_i\leq\sum_i\frac{h_i^{q_i}}{q_i}.
$$

Integrating gives $\int\prod_i h_i\leq1$. If only one finite exponent remains, its weight is one and the same argument is an equality. Restoring the normalization and taking the $r$th root proves

$$
\boxed{\|f_1\cdots f_n\|_r\leq\prod_{i=1}^n\|f_i\|_{p_i}.}
$$

In particular the product belongs to $L^r$.

For the projection estimate, use the three-dimensional [functional Loomis-Whitney inequality](../../../../../functional-loomis-whitney-inequality.md)

$$
\int_{\mathbb R^3}
\bigl(g_1(x_2,x_3)g_2(x_1,x_3)g_3(x_1,x_2)\bigr)^{1/2}\,dx
\leq\prod_{j=1}^3\left(\int_{\mathbb R^2}g_j\right)^{1/2}.
$$

This permitted three-dimensional result also follows directly by [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md): integrate the [square root](../../../../../square-root.md) of $g_1g_2$ in $x_3$, obtaining the [square root](../../../../../square-root.md) of the product of their marginal [integrals](../../../../../integral.md), and then apply [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) in $(x_1,x_2)$ against $\sqrt{g_3}$.

Let $f_j$ be any nonnegative [integrable function](../../../../../lebesgue-integrable-function.md) of the three coordinates excluding $x_j$. For $j=1,2,3$, define $G_j$ by integrating $f_j$ in $x_4$. First [Hölder's inequality](../../../../../holder-s-inequality.md) with three equal exponents yields

$$
\int_{\mathbb R}\prod_{j=1}^3 f_j(\widehat x_j)^{1/3}\,dx_4
\leq\prod_{j=1}^3G_j^{1/3}.
$$

The fourth factor $f_4(x_1,x_2,x_3)$ is independent of $x_4$. A further [Hölder's inequality](../../../../../holder-s-inequality.md) with exponents $3$ and $3/2$, followed by the three-dimensional estimate, therefore gives

$$
\begin{aligned}
\int_{\mathbb R^4}\prod_{j=1}^4f_j(\widehat x_j)^{1/3}\,dx
&\leq\left(\int_{\mathbb R^3}f_4\right)^{1/3}
\left(\int_{\mathbb R^3}\prod_{j=1}^3G_j^{1/2}\right)^{2/3}\\
&\leq\prod_{j=1}^4\left(\int_{\mathbb R^3}f_j\right)^{1/3}.
\end{aligned}
$$

The marginal-integral identifications use [Tonelli's theorem](../../../../../tonelli-theorem.md). Now take $f_j=\mathbf1_{K_j}$. The projections are compact and hence measurable with [finite measure](../../../../../finite-measure.md). Every $x\in K$ has all its projected coordinates in the corresponding $K_j$, so $\mathbf1_K(x)\leq\prod_j\mathbf1_{K_j}(\widehat x_j)^{1/3}$. Consequently

$$
\boxed{\lambda_4(K)\leq\left(\prod_{j=1}^4\lambda_3(K_j)\right)^{1/3}.}
$$

This includes zero-measure projections and is sharp for axis-parallel rectangular boxes.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
