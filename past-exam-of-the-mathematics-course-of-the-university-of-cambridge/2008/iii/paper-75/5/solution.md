<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Set $r=k-1$, with $k\ge2$ for the final linear-reproduction assertion, and use the normalized knot [polynomial](../../../../../polynomial-split.md) $\psi_i=\omega_i/r!$. Differentiate the [Marsden identity](../../../../../marsden-identity.md) $r-j$ times with respect to the auxiliary variable $x$, for $0\le j\le r$. This gives

$$
\frac{r!}{j!}(x-t)^j=\sum_i\omega_i^{(r-j)}(x)N_i(t),
\qquad
\frac{(x-t)^j}{j!}=\sum_i\psi_i^{(r-j)}(x)N_i(t).
$$

The [Taylor polynomial](../../../../../taylor-polynomial.md) expansion of an arbitrary [polynomial](../../../../../polynomial-split.md) $p$ of degree at most $r$ about $x$ is exact:

$$
p(t)=\sum_{j=0}^r\frac{p^{(j)}(x)}{j!}(t-x)^j.
$$

Substitute the differentiated identity into each term and collect the [B-spline](../../../../../b-spline.md) coefficients. The result is

$$
p(t)=\sum_i\lambda_i(p)N_i(t),\qquad
\boxed{\lambda_i(p)=\sum_{j=0}^r(-1)^jp^{(j)}(x)\psi_i^{(r-j)}(x).}
$$

This is the [normalized Marsden dual functional](../../../../../normalized-marsden-dual-functional.md). There is no extra factorial outside the sum, because it is already included in $\psi_i$.

To prove independence of $x$ directly, differentiate the finite sum. The contribution from differentiating $\psi_i$ in term $j$ cancels the contribution from differentiating $p$ in term $j-1$. Explicitly,

$$
\frac{d}{dx}\lambda_i(p)
=\sum_{j=0}^r(-1)^jp^{(j+1)}\psi_i^{(r-j)}
+\sum_{j=0}^r(-1)^jp^{(j)}\psi_i^{(r-j+1)}=0.
$$

The two uncancelled endpoint terms vanish because $p^{(r+1)}=\psi_i^{(r+1)}=0$. Thus the coefficient functional is constant in the auxiliary variable, as required.

The leading two terms of the knot [polynomial](../../../../../polynomial-split.md) give

$$
\psi_i^{(r)}(x)=1,\qquad
\psi_i^{(r-1)}(x)=x-\frac1r\sum_{j=1}^rt_{i+j}=x-t_i^*.
$$

For a linear [polynomial](../../../../../polynomial-split.md) $p(t)=A+Bt$, only $j=0,1$ survive, whence

$$
\lambda_i(p)=p(x)-(x-t_i^*)p'(x)=A+Bt_i^*=p(t_i^*).
$$

The coefficient points $t_i^*$ are the [Greville abscissae](../../../../../greville-abscissa.md). Inserting these coefficients proves exact linear reproduction:

$$
\boxed{p(t)=\sum_i p(t_i^*)N_i(t)\quad\text{for every }p\in\mathcal P_1.}
$$

All identities hold on the basic knot interval $[t_k,t_{n+1}]$, including the endpoints with the standard continuous endpoint convention. Repeated knots cause no difficulty in these [polynomial](../../../../../polynomial-split.md) differentiations.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
