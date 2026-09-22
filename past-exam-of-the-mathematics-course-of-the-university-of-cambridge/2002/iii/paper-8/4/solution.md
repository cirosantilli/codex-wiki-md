<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $M f$ be the [uncentered maximal function](../../../../../uncentered-maximal-function-of-a-finite-measure.md) of $|f|$, defined by its averages over balls. First establish the strong $L^p$ estimate needed below. The [uncentered maximal weak-type inequality](../../../../../uncentered-maximal-weak-type-inequality.md) gives the weak $L^1$ bound with $C_d=3^d$, and plainly $M f\leq\|f\|_\infty$ for bounded inputs. For $f\in L^p$, split it into its parts on $\{|f|>a/2\}$ and $\{|f|\leq a/2\}$. The first part is in $L^1$, since $|f|1_{\{|f|>a/2\}}\leq(a/2)^{1-p}|f|^p$, and the second part contributes at most $a/2$ to the maximal function. Sublinearity therefore gives

$$
\lambda\{Mf>a\}\leq\frac{2C_d}{a}\int_{\{|f|>a/2\}}|f|.
$$

Integrating this bound with [layer cake representation](../../../../../layer-cake-representation.md) and [Tonelli theorem](../../../../../tonelli-theorem.md) yields

$$
\|Mf\|_p^p\leq2C_dp\int|f(x)|\int_0^{2|f(x)|}a^{p-2}\,da\,dx=2^p C_d\frac p{p-1}\|f\|_p^p.
$$

This proves the [strong Lp bound from weak L1 and L-infinity bounds](../../../../../strong-lp-bound-from-weak-l1-and-l-infinity-bounds.md) directly. In particular $Mf$ is finite [almost everywhere](../../../../../almost-everywhere.md).

Now split the positive [Riesz potential](../../../../../riesz-potential.md) of $|f|$ at a radius $r$. In the near region, decompose into annuli $2^{-j-1}r<|x-y|\leq2^{-j}r$. On the $j$th annulus,

$$
\int |x-y|^{\alpha-d}|f(y)|\,dy\leq(2^{-j-1}r)^{\alpha-d}|B(x,2^{-j}r)|Mf(x)\leq C_{d,\alpha}(2^{-j}r)^\alpha Mf(x).
$$

The geometric series converges because $\alpha>0$. In the far region, [Hölder's inequality](../../../../../holder-s-inequality.md), with $p'=p/(p-1)$, gives

$$
\int_{|x-y|>r}|x-y|^{\alpha-d}|f(y)|\,dy\leq\|f\|_p\left(\int_{|z|>r}|z|^{(\alpha-d)p'}\,dz\right)^{1/p'}\leq C_{d,p,\alpha}\|f\|_p r^{\alpha-d/p}.
$$

The radial integral is finite exactly because $p<d/\alpha$. Combining these bounds, including the fixed Riesz normalization constant, gives

$$
I_\alpha|f|(x)\leq C\bigl[r^\alpha Mf(x)+r^{\alpha-d/p}\|f\|_p\bigr].
$$

For $0<Mf(x)<\infty$, choose $r=(\|f\|_p/Mf(x))^{p/d}$. If $Mf(x)=0$, every ball average vanishes and $f=0$ almost everywhere, so the assertion is trivial. The zero-norm case is likewise trivial. The resulting [Hedberg inequality](../../../../../hedberg-inequality.md) is

$$
\boxed{I_\alpha|f|(x)\leq C\|f\|_p^{\alpha p/d}(Mf(x))^{1-\alpha p/d}}.
$$

This proves absolute convergence of the defining integral for almost every $x$, also for signed or complex $f$. Put $\theta=\alpha p/d\in(0,1)$. The proposed exponent satisfies $q=p/(1-\theta)$, so $(1-\theta)q=p$. Raising the pointwise estimate to the $q$th power and using the proved maximal bound gives

$$
\boxed{\|I_\alpha f\|_q\leq C\|f\|_p^\theta\|Mf\|_p^{1-\theta}\leq A_{d,p,\alpha}\|f\|_p}.
$$

Thus the [Hardy–Littlewood–Sobolev inequality](../../../../../hardy-littlewood-sobolev-inequality.md) follows from the estimates just derived, rather than being quoted in place of its proof.

For uniqueness of the target exponent, suppose such a uniform estimate holds with index $r$ instead. Choose a nonzero nonnegative [bump function](../../../../../bump-function.md) $f$ and let $f_t(x)=f(tx)$ for $t>0$. Homogeneity of the [Riesz potential](../../../../../riesz-potential.md) gives

$$
I_\alpha f_t(x)=t^{-\alpha}(I_\alpha f)(tx),\qquad \|f_t\|_p=t^{-d/p}\|f\|_p.
$$

The assumed estimate at $t=1$ makes the nonzero output's $L^r$ norm finite. For all $t>0$ it must therefore satisfy

$$
t^{-\alpha-d/r}\|I_\alpha f\|_r\leq A t^{-d/p}\|f\|_p,
$$

with $d/r=0$ when $r=\infty$. Letting $t$ tend to zero or infinity forces the power of $t$ to vanish:

$$
\boxed{\frac1r=\frac1p-\frac\alpha d}.
$$

Hence no other target index is possible.

For the [Sobolev embedding](../../../../../failure-of-first-order-sobolev-embedding-into-linfinity-in-two-dimensions.md), take $d>1$ and $1<p<d$, so the preceding result is available with $\alpha=1$. For $u\in C_c^\infty(\mathbb R^d)$, the vector field $(x-y)/|x-y|^d$ has zero divergence in $y$ away from $x$. Integrating by parts outside the ball $|x-y|\leq\varepsilon$, its inner boundary contributes $|\mathbb S^{d-1}|$ times the spherical average of $u$ about $x$. The outer boundary contributes zero because $u$ has compact support. Letting $\varepsilon\downarrow0$ proves

$$
u(x)=\frac1{|\mathbb S^{d-1}|}\int\frac{x-y}{|x-y|^d}\cdot\nabla u(y)\,dy.
$$

The absolute value is at most $C I_1(|\nabla u|)(x)$. Thus

$$
\boxed{\|u\|_{q_1}\leq C_{d,p}\|\nabla u\|_p,\qquad \frac1{q_1}=\frac1p-\frac1d}.
$$

For a general member of the [first-order Sobolev space](../../../../../first-order-sobolev-space.md) $W^{1,p}(\mathbb R^d)=L_1^p(\mathbb R^d)$, approximate in the Sobolev norm by compactly supported smooth functions. This [density of smooth functions in a Sobolev space](../../../../../density-of-smooth-functions-in-a-sobolev-space.md) follows from cutoffs tending to one and subsequent mollification: the cutoff-gradient term tends to zero in $L^p$, and a [mollifier](../../../../../mollifier.md) approximates both the function and each [weak derivative](../../../../../weak-derivative.md). The displayed estimate makes the approximants Cauchy in $L^{q_1}$. Their $L^p$ limit is the original function, so subsequences converging almost everywhere identify the $L^{q_1}$ limit with it. This proves continuous embedding. The range $1<p<d$ is essential for this consequence; the formula is not a general critical $p=d$ embedding into $L^\infty$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
