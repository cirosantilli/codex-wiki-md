<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $t_i=(x_i-x)/h$, $r_p(t)=(1,t,\ldots,t^p)^T$, and define

$$
X_{ij}=t_i^j,\qquad
W=\operatorname{diag}(K(t_1),\ldots,K(t_n)).
$$

The degree-$p$ [local polynomial regression](../../../../../local-polynomial-regression.md) fit minimizes

$$
\sum_{i=1}^nK(t_i)\{Y_i-r_p(t_i)^T\beta\}^2.
$$

Assume its [local polynomial Gram matrix](../../../../../local-polynomial-gram-matrix.md)

$$
B_n(x)=\frac1{nh}X^TWX
$$

is positive definite. The normal equations then give

$$
\widehat\beta=(X^TWX)^{-1}X^TWY,
\qquad
\widehat m_n(x)=\widehat\beta_0.
$$

Because the polynomial is written in the scaled coordinate, the [local polynomial derivative estimator](../../../../../local-polynomial-derivative-estimator.md) is $\widehat m_n'(x)=\widehat\beta_1/h$. If $e_1=(0,1,0,\ldots,0)^T$, then

$$
\widehat m_n'(x)
=\frac1n\sum_{i=1}^nv_{p,i}(x)Y_i,
\qquad
v_{p,i}(x)=\frac1{h^2}
e_1^TB_n(x)^{-1}r_p(t_i)K(t_i).
$$

For a polynomial $R$ of degree at most $p$, the local least-squares fit to $Y_i=R(x_i)$ is exactly the Taylor polynomial $R(x+ht)$, so its scaled linear coefficient is $hR'(x)$. Therefore the [polynomial reproduction property of local polynomial regression](../../../../../polynomial-reproduction-property-of-local-polynomial-regression.md) gives

$$
\frac1n\sum_{i=1}^nv_{p,i}(x)R(x_i)=R'(x).
$$

Positive definiteness and the fixed finite-dimensional basis provide a number $\lambda_0>0$ such that

$$
\sup_{|t|\leq1}
|e_1^TB_n(x)^{-1}r_p(t)|\leq\frac2{\lambda_0}.
$$

Since $K(t_i)=0$ outside $|x_i-x|\leq h$,

$$
\max_i\frac1n|v_{p,i}(x)|
\leq\frac{2\lVert K\rVert_\infty}{\lambda_0nh^2}
$$

and

$$
\frac1n\sum_i|v_{p,i}(x)|
\leq\frac{2\lVert K\rVert_\infty}{\lambda_0nh^2}
\sum_i\mathbf1_{\{|x_i-x|\leq h\}}.
$$

The regular design has at most $2nh+2\leq4nh$ points in this window when $h\geq1/(2n)$. Since the errors are independent with variance at most $\sigma^2$,

$$
\begin{aligned}
\operatorname{Var}(\widehat m_n'(x))
&\leq\frac{\sigma^2}{n^2}\sum_i v_{p,i}(x)^2\\
&\leq\frac{\sigma^2}{n^2}
\max_i|v_{p,i}(x)|\sum_i|v_{p,i}(x)|\\
&\leq\frac{16\lVert K\rVert_\infty^2\sigma^2}
{\lambda_0^2nh^3}.
\end{aligned}
$$

Finally let $\beta_0=\lceil\beta\rceil-1$ and take the degree-$\beta_0$ Taylor polynomial $R$ of $m$ at $x$. The [Hölder class](../../../../../holder-class.md) remainder satisfies

$$
|m(x_i)-R(x_i)|
\leq\frac L{\beta_0!}|x_i-x|^\beta.
$$

Polynomial reproduction removes $R$ from the bias. On the kernel window the remainder is at most $Lh^\beta/\beta_0!$, so the weight-sum bound gives

$$
\boxed{|\operatorname{Bias}(\widehat m_n'(x))|
\leq\frac{8L\lVert K\rVert_\infty}
{\lambda_0\beta_0!}h^{\beta-1}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
