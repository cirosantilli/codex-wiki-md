<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Write $L_n(t)=\sum_{k=0}^na_kt^k$. Matching coefficients in the differential equation gives

$$
(k+1)^2a_{k+1}+(n-k)a_k=0.
$$

Taking $a_0=1$ yields

$$
\boxed{L_n(t)=\sum_{k=0}^n(-1)^k\binom nk\frac{t^k}{k!}.}
$$

The top coefficient is $(-1)^n/n!\ne0$, so this is a real [polynomial](../../../../polynomial-split.md) of degree exactly $n$.

Put $D_n=L_n'-L_n$. [Integration by parts](../../../../integration-by-parts.md), with vanishing endpoint terms because of the factor $t$ at zero and exponential decay at infinity, gives

$$
\begin{aligned}
\int_0^\infty tD_nD_me^{-t}dt
&=-\int_0^\infty[(tD_ne^{-t})'+tD_ne^{-t}]L_mdt\\
&=-\int_0^\infty[D_n+tD_n']L_me^{-t}dt\\
&=(n+1)\int_0^\infty L_nL_me^{-t}dt.
\end{aligned}
$$

The last step uses $D_n+tD_n'=tL_n''+(1-t)L_n'-L_n=-(n+1)L_n$. The left side is symmetric in $m,n$. Interchanging them therefore gives $(n-m)\int L_nL_me^{-t}=0$, proving [orthogonality](../../../../orthogonal-vectors.md) for distinct indices. These integrals are exactly $\langle\varphi_n,\varphi_m\rangle$, and each $\varphi_n$ is square-integrable and nonzero. Thus they form an [orthogonal](../../../../orthogonal-vectors.md) sequence in $L^2(0,\infty)$.

Multiplying the equations by $z^n$ and summing gives

$$
\boxed{tG_{tt}+(1-t)G_t+zG_z=0.}
$$

Conversely equality of power-series coefficients recovers every [polynomial](../../../../polynomial-split.md) equation. For the proposed expression,

$$
\frac{G_t}G=-\frac z{1-z},\qquad\frac{G_{tt}}G=\frac{z^2}{(1-z)^2},\qquad\frac{G_z}G=\frac1{1-z}-\frac t{(1-z)^2}.
$$

Substitution makes the PDE left side zero. Its coefficient of $z^n$ has value one at $t=0$, so it corresponds to the normalization $L_n(0)=1$ chosen above.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
