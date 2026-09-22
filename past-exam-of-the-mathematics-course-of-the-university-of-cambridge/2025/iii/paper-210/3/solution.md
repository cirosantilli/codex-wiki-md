<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $r=\lceil\beta\rceil-1$. The [Hölder class](../../../../../holder-class.md) $\mathcal H(\beta,L)$ consists of functions with $r$ continuous derivatives whose $r$th derivative satisfies

$$
|m^{(r)}(x)-m^{(r)}(y)|\leq L|x-y|^{\beta-r},
$$

with the equivalent Lipschitz convention when $\beta$ is an integer.

The degree-$p$ [local polynomial regression](../../../../../local-polynomial-regression.md) estimator minimizes

$$
\sum_{i=1}^nK_h(x_i-x)
\left[Y_i-\sum_{j=0}^pb_j\frac{(x_i-x)^j}{j!}\right]^2
$$

and takes $\widehat m_n(x;p,h)=\widehat b_0$. Put $X_i^T=Q((x_i-x)/h)^T$, $W_{ii}=K_h(x_i-x)$, and rescale $b_j$ by $h^j$. If $X^TWX$ is positive definite, weighted least squares gives

$$
\widehat b=(X^TWX)^{-1}X^TWY,
\qquad
\widehat m_n=e_0^T\widehat b.
$$

Define

$$
w_i(x)=e_0^T\left(\frac1nX^TWX\right)^{-1}X_iW_{ii}.
$$

Then $\widehat m_n=n^{-1}\sum_iw_iY_i$. If $R$ has degree at most $p$, fitting the noiseless response $R(x_i)$ reproduces that polynomial exactly, and hence

$$
\frac1n\sum_iw_i(x)R(x_i)=R(x).
$$

For nonzero $a$, the polynomial $a^TQ(u)$ cannot vanish throughout $[0,1]$. Therefore

$$
a^T\left(\int_0^1Q(u)Q(u)^Tdu\right)a>0,
$$

and compactness of the unit sphere makes its minimum eigenvalue $\Lambda_p$ positive. Choose $a(p)$ and $n_0(p)$ so that $nh\geq a(p)$ makes the supplied lower bound on $\lambda_0$ at least $\Lambda_p/4$. On the kernel support, $Q$ is bounded by a constant depending only on $p$, and $K_h\leq1/(2h)$. It follows that only $O(nh)$ weights are nonzero and

$$
|w_i(x)|\leq C_p/h,
\quad
\frac1{n^2}\sum_iw_i(x)^2\leq\frac{C_p}{nh},
\quad
\frac1n\sum_i|w_i(x)|\leq C_p.
$$

Polynomial reproduction cancels the Taylor polynomial of degree $r\leq p$. The Hölder remainder on $|x_i-x|\leq h$ is at most $C_pLh^\beta$, so the squared bias is at most $C_pL^2h^{2\beta}$. Independence and $\operatorname{Var}\varepsilon_i\leq\sigma^2$ bound the variance by $C_p\sigma^2/(nh)$. Combining them uniformly in $x$ and $m$ proves

$$
\boxed{\sup_{x\in[0,1]}\sup_{m\in\mathcal H(\beta,L)}
\mathbb E(\widehat m_n(x;p,h)-m(x))^2
\leq C(p)\left(\frac{\sigma^2}{nh}+L^2h^{2\beta}\right).}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
