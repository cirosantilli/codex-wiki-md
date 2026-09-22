<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We use the [Van der Corput sum-integral lemma](../../../../../../van-der-corput-sum-integral-lemma.md). Put $e(u)=e^{2\pi iu}$ and $I_h=\int_a^b e(f(x)-hx)\,dx$. The [Fourier series](../../../../../../fourier-series-split.md) of the periodization of $1_{[a,b]}(x)e(f(x))$ gives

$$
\sum_{a\le n\le b}'e(f(n))=\lim_{H\to\infty}\sum_{|h|\le H}I_h,
$$

where integer endpoints have half weight. This is the [Dirichlet-Jordan convergence theorem](../../../../../../dirichlet-jordan-convergence-theorem.md) for a piecewise smooth, or more generally bounded-variation, periodic function. Here $f$ is $C^1$, so the periodized function has [bounded variation](../../../../../../total-variation-of-a-function.md). Changing to the requested endpoint convention costs at most one.

Write $u=f'$. For $h\ne0$, $|u-h|\ge|h|-\delta>0$. Since $u$ is continuous and [monotone](../../../../../../monotonic-function.md), the reciprocal has [bounded variation](../../../../../../total-variation-of-a-function.md), and [integration by parts](../../../../../../integration-by-parts.md) in the Riemann-Stieltjes sense yields

$$
I_h=\left[\frac{e(f(x)-hx)}{2\pi i(u(x)-h)}\right]_a^b-\frac1{2\pi i}\int_a^b e(f(x)-hx)\,d\!\left(\frac1{u(x)-h}\right).
$$

The variation of the reciprocal is at most $2\delta/(h^2-\delta^2)$. Summing over $h\ne0$ gives $O((1-\delta)^{-1})$, separating $|h|=1$ and using convergence of $\sum_{h\ge2}h^{-2}$. For each endpoint, use

$$
\frac1{u-h}=-\frac1h+\frac{u}{h(u-h)}.
$$

The symmetric partial sums of the first term are a constant multiple of $\sum_{h=1}^H\sin(2\pi hx)/h$, uniformly bounded in $H$ and $x$; this standard [Fourier series](../../../../../../fourier-series-split.md) bound follows by splitting at $h\asymp1/\|x\|$ and applying [Abel summation](../../../../../../abel-s-summation-formula.md) to the remaining sine sum. The second term is absolutely summable with bound $O((1-\delta)^{-1})$. The same bound therefore holds for the whole sum of the $h\ne0$ integrals. Since $I_0$ is the ordinary integral,

$$
\boxed{\sum_{a<n\le b}e(f(n))=\int_a^be(f(x))\,dx+O\bigl((1-\delta)^{-1}\bigr).}
$$

No second derivative is required; monotonicity supplies the needed variation estimate.

For the [Hardy-Littlewood approximation to the Riemann zeta function](../../../../../../hardy-littlewood-approximation-to-the-riemann-zeta-function.md), take $f(w)=-t\log w/(2\pi)$. On $w\ge x\ge|t|/\pi$, $|f'(w)|\le1/2$ and $f'$ is [monotone](../../../../../../monotonic-function.md). The proved lemma says that the difference between the partial sum of $w^{-it}$ and its integral over $(x,Y]$ is $O(1)$ uniformly in $Y$. Weighted [Abel summation](../../../../../../abel-s-summation-formula.md) with the decreasing weight $w^{-\sigma}$ then makes the weighted difference $O(x^{-\sigma})$, since its total variation on $[x,\infty)$ is $x^{-\sigma}$. Initially for $\sigma>1$, the tail integral is $x^{1-s}/(s-1)$. The bounded primitive of the discrepancy gives a [locally uniformly convergent](../../../../../../locally-uniform-convergence.md) weighted discrepancy integral for every $\sigma>0$, continuing the identity to that region. Thus, away from the [pole](../../../../../../pole.md),

$$
\boxed{\zeta(s)=\sum_{n\le x}n^{-s}+\frac{x^{1-s}}{s-1}+O(x^{-\sigma}),\qquad x\ge|t|/\pi.}
$$

If $t=0$ the ordinary sum-integral comparison supplies the same estimate. At $s=1$ the formula is understood meromorphically. It approximates the [Riemann zeta function](../../../../../../riemann-zeta-function.md) by a finite [Dirichlet polynomial](../../../../../../dirichlet-polynomial.md), transfers [exponential sum](../../../../../../exponential-sum.md) estimates to bounds in the [critical strip](../../../../../../critical-strip.md), yields elementary near-one bounds for $\zeta$ and its [derivative](../../../../../../derivative.md), and supports estimates for the [mean value of Dirichlet polynomials](../../../../../../mean-value-of-dirichlet-polynomials.md) and numerical calculations.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
