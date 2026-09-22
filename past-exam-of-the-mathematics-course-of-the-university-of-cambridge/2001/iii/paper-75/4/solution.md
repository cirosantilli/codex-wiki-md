<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $d\mu=dx\,dy/y^2$ and distinguish the all-pairs [Eisenstein series](../../../../../eisenstein-series.md) in this problem from its primitive version

$$
E_0(z,w)=\frac12\sum_{(c,d)=1}\frac{y^w}{|cz+d|^{2w}}
=\sum_{\Gamma_\infty\backslash SL_2(\mathbb Z)}(\operatorname{Im}\gamma z)^w.
$$

Separating each nonzero integer pair into a positive integer multiple of a primitive pair gives

$$
E(z,w)=2\pi^{-w}\Gamma(w)\zeta(2w)E_0(z,w).
$$

The factor two accounts for the two signs of a primitive pair. It must not be omitted in the [Rankin–Selberg unfolding](../../../../../rankin-selberg-method.md).

Because $f\overline g y^k$ and $d\mu$ are invariant, unfolding its integral against $E_0$ produces the strip $0\leq x<1$, $y>0$:

$$
\int_{\mathcal F}f(z)\overline{g(z)}y^kE_0(z,w)d\mu
=\int_0^\infty\int_0^1 f(x+iy)\overline{g(x+iy)}y^{w+k-2}dx\,dy.
$$

The $x$ integral of the product [Fourier expansions](../../../../../fourier-series-split.md) is $\sum_{n\geq1}a(n)\overline{b(n)}e^{-4\pi ny}$. The [Gamma function](../../../../../gamma-function.md) integral then gives

$$
\int_{\mathcal F}f\overline g y^kE_0(z,w)d\mu
=\frac{\Gamma(w+k-1)}{(4\pi)^{w+k-1}}F(w+k-1).
$$

These steps first follow by absolute convergence sufficiently far right. For $f=g$, positive unfolding and [modular cusp](../../../../../cusp-of-a-modular-group.md) decay show the square-coefficient series converges for $\operatorname{Re}s>k$; the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives the same absolute-convergence range for the mixed series.

Put $w=s-k+1$ and define

$$
\boxed{\mathcal R(s):=2\pi^{-w}\Gamma(w)\zeta(2w)\frac{\Gamma(s)}{(4\pi)^s}F(s)
=\int_{\mathcal F}f(z)\overline{g(z)}y^kE(z,w)d\mu.}
$$

This is the [zeta-completed Rankin-Selberg coefficient series](../../../../../zeta-completed-rankin-selberg-coefficient-series.md). Equivalently, solving this formula for $F(s)$ expresses the requested series directly in terms of the all-pairs Eisenstein integral.

The exponential decay of [cusp forms](../../../../../cusp-form.md) at infinity dominates the [polynomial](../../../../../polynomial-split.md) growth in $y$ of the [Eisenstein series](../../../../../eisenstein-series.md) and its parameter derivatives, locally uniformly away from its poles. Thus its stated continuation can be passed through the integral. The completed series is meromorphic on $\mathbb C$, with possible simple poles only at $s=k-1,k$, and its [functional equation](../../../../../functional-equation.md) is

$$
\boxed{\mathcal R(s)=\mathcal R(2k-1-s).}
$$

Indeed $w\mapsto1-w$ corresponds to $s\mapsto2k-1-s$. If $\langle f,g\rangle=0$, both pole residues vanish and the completion is entire.

The normalization of the poles can also be made explicit. The constant term of the given [Eisenstein series](../../../../../eisenstein-series.md) is

$$
2\pi^{-w}\Gamma(w)\zeta(2w)y^w
+2\pi^{1/2-w}\Gamma(w-\tfrac12)\zeta(2w-1)y^{1-w}.
$$

The second term has residue one at $w=1$, since the pole of $\zeta(2w-1)$ has residue $1/2$; the [functional equation](../../../../../functional-equation.md) gives residue minus one at $w=0$. Hence the residues of $\mathcal R$ at $k$ and $k-1$ are respectively $\langle f,g\rangle$ and $-\langle f,g\rangle$, the [Petersson inner product](../../../../../petersson-inner-product.md).

It is important to separate this completed statement from the raw $F$. Inverting the completion gives [meromorphic continuation](../../../../../meromorphic-continuation.md) of $F$, but zeros of $\zeta(2s-2k+2)$ in the denominator can give additional possible poles unless canceled by the integral. Nor does $F$ itself satisfy the unweighted symmetry $s\leftrightarrow2k-1-s$. At the two displayed completion poles, for a nontrivial [modular cusp](../../../../../cusp-of-a-modular-group.md) [modular weight](../../../../../weight-of-a-modular-form.md),

$$
\boxed{\operatorname*{Res}_{s=k}F(s)=\frac{3(4\pi)^k}{\pi\Gamma(k)}\langle f,g\rangle,
\qquad F(k-1)=\frac{(4\pi)^{k-1}}{\Gamma(k-1)}\langle f,g\rangle.}
$$

The latter is finite because the pole of $\Gamma(w)$ cancels that of the integral at $w=0$, using $\zeta(0)=-1/2$. In particular, taking $f=g\ne0$ gives a raw-series pole at $k$ and regularity at $k-1$. The direct analogue of the stipulated two-pole Eisenstein properties is therefore the completed function $\mathcal R$, not the raw series with all completion factors suppressed.

Finally suppose the two $L$-series have [Euler products](../../../../../euler-product.md). With first [coefficients](../../../../../coefficient.md) normalized to one, their [coefficients](../../../../../coefficient.md) are multiplicative, so $a(n)\overline{b(n)}$ is multiplicative too. Therefore

$$
\boxed{F(s)=\prod_p\left(\sum_{r\geq0}a(p^r)\overline{b(p^r)}p^{-rs}\right),}
$$

initially in its absolute-convergence half-plane. For unnormalized forms multiply the product by $a(1)\overline{b(1)}$ and use normalized [coefficients](../../../../../coefficient.md) inside it.

For the usual degree-two Hecke products of Question 3, take roots $\alpha_p,\beta_p$ with sum $a(p)$ and product $p^{k-1}$, and $\gamma_p,\delta_p$ with sum $b(p)$ and the same product. The prime-power recurrence gives $a(p^r)=(\alpha_p^{r+1}-\beta_p^{r+1})/(\alpha_p-\beta_p)$ and the analogous expression for $b$. Multiplying and summing four geometric series proves the [Euler factor of a coefficientwise product of Hecke eigenforms](../../../../../euler-factor-of-a-coefficientwise-product-of-hecke-eigenforms.md):

$$
\boxed{F_p(X)=\frac{1-p^{2k-2}X^2}
{(1-\alpha_p\overline\gamma_pX)(1-\alpha_p\overline\delta_pX)
(1-\beta_p\overline\gamma_pX)(1-\beta_p\overline\delta_pX)},\qquad X=p^{-s}.}
$$

Repeated roots are handled by continuity, or directly by the recurrence. Multiplication by $\zeta(2s-2k+2)$ cancels the local numerators and yields the degree-four convolution product. This also explains why the zeta factor belongs in the natural analytic completion.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
