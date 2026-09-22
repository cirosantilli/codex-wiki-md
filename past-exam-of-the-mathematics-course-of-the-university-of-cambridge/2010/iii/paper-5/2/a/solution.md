<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One potential form of the [Hardy–Littlewood–Sobolev inequality](../../../../../../hardy-littlewood-sobolev-inequality.md) is: if $0<\alpha<n$, $1<p<n/\alpha$, and $1/r=1/p-\alpha/n$, then

$$
\boxed{\left\|I_\alpha f\right\|_r\leq C_{n,p,\alpha}\|f\|_p,\qquad I_\alpha f(x)=\int_{\mathbb R^n}|x-y|^{\alpha-n}f(y)\,dy.}
$$

A normalization constant for the [Riesz potential](../../../../../../riesz-potential.md) only changes $C$. Equivalently, for $0<\lambda<n$, $p,s>1$ and $1/p+1/s+\lambda/n=2$,

$$
\boxed{\iint\frac{|f(x)||g(y)|}{|x-y|^\lambda}\,dx\,dy\leq C\|f\|_p\|g\|_s.}
$$

The exponent relation is necessary under dilation. We prove the potential estimate and then derive the bilinear version.

First establish the needed maximal estimate, so it is not an unproved step in the argument. Define the centered [Hardy-Littlewood maximal function](../../../../../../hardy-littlewood-maximal-function.md) by $Mf(x)=\sup_{t>0}|B_t|^{-1}\int_{B_t(x)}|f|$. For integrable $f$, cover a compact subset of $\{Mf>a\}$ by finitely many balls whose averages exceed $a$. Order these balls by decreasing radius and greedily retain a ball if it is disjoint from those already retained. Every discarded ball intersects a retained ball of at least its radius, so lies in its triple. Hence

$$
|\{Mf>a\}|\leq3^n\sum_i|B_i|\leq\frac{3^n}{a}\sum_i\int_{B_i}|f|\leq\frac{3^n}{a}\|f\|_1.
$$

The passage from compact subsets uses [inner regularity of Lebesgue measure](../../../../../../inner-regularity-of-lebesgue-measure.md); the superlevel set is open because fixed-radius local averages are continuous. For $f\in L^p$, split $f=f\mathbf1_{\{|f|>a/2\}}+f\mathbf1_{\{|f|\leq a/2\}}$. The second summand's maximal function is at most $a/2$, and the first is integrable. Therefore

$$
|\{Mf>a\}|\leq\frac{2\cdot3^n}{a}\int_{|f|>a/2}|f|.
$$

The [layer cake representation](../../../../../../layer-cake-representation.md) and [Tonelli theorem](../../../../../../tonelli-theorem.md) give

$$
\begin{aligned}\|Mf\|_p^p&=p\int_0^\infty a^{p-1}|\{Mf>a\}|\,da\\
&\leq2\cdot3^np\int|f(x)|\int_0^{2|f(x)|}a^{p-2}\,da\,dx
=\frac{3^np2^p}{p-1}\|f\|_p^p.
\end{aligned}
$$

Thus the [Strong Lp bound for the Hardy-Littlewood maximal function](../../../../../../strong-lp-bound-for-the-hardy-littlewood-maximal-function.md) is proved for every $p>1$.

For $I_\alpha|f|(x)$, split at radius $R$. Dyadic shells with radii $2^{-j}R$ give

$$
\int_{|x-y|<R}|x-y|^{\alpha-n}|f(y)|\,dy\leq C\sum_{j\geq0}(2^{-j}R)^\alpha Mf(x)\leq CR^\alpha Mf(x).
$$

For the outer part, [Hölder's inequality](../../../../../../holder-s-inequality.md) gives

$$
\int_{|x-y|\geq R}|x-y|^{\alpha-n}|f(y)|\,dy\leq\|f\|_p\left(\int_{|z|\geq R}|z|^{(\alpha-n)p'}dz\right)^{1/p'}=C\|f\|_pR^{\alpha-n/p}.
$$

The last integral is finite exactly because $p<n/\alpha$. Balance the two bounds by $R^{n/p}=\|f\|_p/Mf(x)$ to obtain the [Hedberg inequality](../../../../../../hedberg-inequality.md)

$$
I_\alpha|f|(x)\leq C\|f\|_p^\theta(Mf(x))^{1-\theta},\qquad\theta=\alpha p/n.
$$

The zero cases follow directly or by a limit; $Mf$ is finite almost everywhere by the maximal estimate. Since $r(1-\theta)=p$, integration and the proved maximal bound yield $\|I_\alpha f\|_r\leq C\|f\|_p$. Taking $\alpha=n-\lambda$ and pairing $I_\alpha|f|$ with $|g|\in L^{r'}$ proves the bilinear form by [Hölder's inequality](../../../../../../holder-s-inequality.md), because $s=r'$. All integrals are justified first for nonnegative truncations and then by monotone convergence and the resulting finite bound. The strong estimate does not include $p=1$ or $p=n/\alpha$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
