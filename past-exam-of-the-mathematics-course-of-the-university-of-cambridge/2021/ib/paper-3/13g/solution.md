<h1 id="13g/solution">Solution</h1>

↑ **Parent:** [13G](../13g.md)

Fix $a\notin[\gamma]$ and let

$$
d=\operatorname{dist}(a,[\gamma])>0.
$$

For $|z-a|<d$ and $\lambda\in[\gamma]$, the [geometric series](../../../../../geometric-series.md) gives

$$
\frac1{\lambda-z}
=\frac1{\lambda-a}\frac1{1-(z-a)/(\lambda-a)}
=\sum_{n=0}^{\infty}\frac{(z-a)^n}{(\lambda-a)^{n+1}}.
$$

The series converges uniformly on every smaller closed disc, so it may be integrated term by term along the curve. Hence

$$
\boxed{
f(z)=\sum_{n=0}^{\infty}c_n(z-a)^n,
\qquad
c_n=\int_\gamma\frac{\phi(\lambda)}
{(\lambda-a)^{n+1}}\,d\lambda
},
$$

which is a [power series](../../../../../power-series.md) about $a$.

If $f$ is holomorphic on a neighbourhood of the closed disc $\overline D(a,r)$, the [Cauchy integral formula](../../../../../cauchy-integral-formula.md) says

$$
f(z)=\frac1{2\pi i}\int_{|\zeta-a|=r}
\frac{f(\zeta)}{\zeta-z}\,d\zeta,
\qquad |z-a|<r.
$$

Differentiation under the integral is valid uniformly on smaller discs and gives the [Cauchy derivative formula](../../../../../cauchy-derivative-formula.md)

$$
\boxed{
f^{(n)}(z)=\frac{n!}{2\pi i}
\int_{|\zeta-a|=r}
\frac{f(\zeta)}{(\zeta-z)^{n+1}}\,d\zeta
}.
$$

This proves inductively that every holomorphic function has complex derivatives of every order. In particular,

$$
\boxed{
f'(z)=\frac1{2\pi i}
\int_{|\zeta-a|=r}\frac{f(\zeta)}{(\zeta-z)^2}\,d\zeta
}.
$$

Now suppose $f_n\to f$ [locally uniformly](../../../../../locally-uniform-convergence.md) on $U$. Given a compact set $K\subset U$, choose finitely many closed discs whose slightly larger concentric discs remain in $U$ and whose interiors cover $K$. Applying the derivative formula to $f_n-f$ on the larger boundary circles gives a uniform [Cauchy estimate](../../../../../cauchy-estimate.md)

$$
\sup_K|f_n'-f'|
\leq C\sup_L|f_n-f|,
$$

where $L\subset U$ is the compact union of those circles. The right-hand side tends to zero, proving that

$$
\boxed{f_n'\to f'\text{ locally uniformly}}.
$$

Finally, choose open neighbourhoods $U_j$ of the closed discs $D_j$ so small that

$$
U_1\cap U_2
$$

lies in the given neighbourhood on which $f$ is holomorphic. Inside that neighbourhood choose a positively oriented piecewise smooth contour $\Gamma$ surrounding $D_1\cap D_2$. It may be chosen as the boundary of a slightly enlarged lens and split into arcs

$$
\Gamma=\Gamma_1+\Gamma_2
$$

so that $\Gamma_1$ stays away from $D_1$ and $\Gamma_2$ stays away from $D_2$. Define

$$
f_1(z)=\frac1{2\pi i}\int_{\Gamma_1}
\frac{f(\zeta)}{\zeta-z}\,d\zeta
\quad\text{near }D_1,
$$

and

$$
f_2(z)=\frac1{2\pi i}\int_{\Gamma_2}
\frac{f(\zeta)}{\zeta-z}\,d\zeta
\quad\text{near }D_2.
$$

Because each arc avoids the corresponding disc, these formulas define holomorphic functions on possibly smaller neighbourhoods $U_1,U_2$. On their overlap, the [Cauchy integral formula](../../../../../cauchy-integral-formula.md) for the full contour gives

$$
\boxed{f=f_1+f_2}.
$$

## ↑ Ancestors (10)

1. [13G](../13g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
