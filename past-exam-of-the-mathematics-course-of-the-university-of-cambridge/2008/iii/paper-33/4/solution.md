<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the [primitive real-analytic Eisenstein series](../../../../../primitive-real-analytic-eisenstein-series.md) with exactly the normalization in the PDF. Its [coset](../../../../../coset.md) expression uses $\Gamma_\infty=\{\pm\begin{pmatrix}1&n\\0&1\end{pmatrix}:n\in\mathbb Z\}$, so primitive bottom rows differing by sign represent the same [coset](../../../../../coset.md). The factor $1/2$ in the primitive-pair sum accounts for this sign identification. Unlike the sum over all nonzero [integer](../../../../../integer.md) pairs, this [Eisenstein series](../../../../../eisenstein-series.md) has no additional factor $2\zeta(2w)$. Write $w$ for the [Rankin–Selberg integral](../../../../../rankin-selberg-integral-for-holomorphic-cusp-forms.md) parameter and $s$ for the [Dirichlet series](../../../../../dirichlet-series.md) parameter to keep their shift visible.

First establish an initial region where all rearrangements are absolute. The [invariant norm of a modular form](../../../../../invariant-norm-of-a-modular-form.md) $y^{k/2}|f(\tau)|$ is bounded: it is $\Gamma$-invariant, continuous on a truncated fundamental domain, and tends to [zero](../../../../../zero-of-a-function.md) at the cusp. Integrating one period of the [Fourier series](../../../../../fourier-series-split.md) gives

$$
a_ne^{-2\pi ny}=\int_0^1 f(x+iy)e^{-2\pi inx}\,dx,
\qquad |a_n|\leq Cy^{-k/2}e^{2\pi ny}.
$$

With $y=1/n$, this proves the [Fourier coefficient bound for a cusp form](../../../../../fourier-coefficient-bound-for-a-cusp-form.md) $a_n=O(n^{k/2})$, and similarly $b_n=O(n^{k/2})$. Hence $D(f,g,s)$ is initially absolutely convergent for $\operatorname{Re}s>k+1$.

For $\operatorname{Re}w>1$, the [primitive real-analytic Eisenstein series](../../../../../primitive-real-analytic-eisenstein-series.md) is locally uniformly convergent and [holomorphic](../../../../../complex-differentiability-at-a-point.md) in $w$. On the standard fundamental domain it has at most [polynomial growth](../../../../../polynomial-growth.md) in $y$, locally uniformly in this half-plane. These are the analytic properties of the [Eisenstein series](../../../../../eisenstein-series.md) needed here; they can also be checked directly from its defining sum. For example, for real $\sigma>1$ and $y\geq1$, majorize the primitive sum by the sum over all nonzero pairs and use

$$
\sum_{n\in\mathbb Z}\big((mx+n)^2+(my)^2\big)^{-\sigma}
\leq C_\sigma\big((|m|y)^{-2\sigma}+(|m|y)^{1-2\sigma}\big)
\quad(m\ne0).
$$

This bound follows by comparing a shifted one-dimensional sum with its integral and a largest summand. Summing over $m\ne0$ gives $E(\tau,\sigma)=O(y^\sigma+y^{1-\sigma})$. For complex $w$, $|E(\tau,w)|\leq E(\tau,\operatorname{Re}w)$, and the estimates are uniform on compact parameter sets. Since $f$ and $g$ decay exponentially on the cusp end, the integral $I(f,g,w)$ is therefore [holomorphic](../../../../../complex-differentiability-at-a-point.md) throughout $\operatorname{Re}w>1$ by dominated integration.

The product $f(\tau)\overline{g(\tau)}y^k$ is $\Gamma$-invariant: the two modular factors cancel the transformation $\operatorname{Im}(\gamma\tau)=y/|c\tau+d|^2$. With the [hyperbolic area](../../../../../hyperbolic-area.md) $d\mu=dx\,dy/y^2$, [Rankin–Selberg unfolding](../../../../../rankin-selberg-method.md) gives, initially for $\operatorname{Re}w>2$,

$$
\begin{aligned}
I(f,g,w)
&=\int_{\Gamma\backslash\mathbb H}f\overline g\,y^k
\sum_{\gamma\in\Gamma_\infty\backslash\Gamma}(\operatorname{Im}\gamma\tau)^w\,d\mu\\
&=\int_{\Gamma_\infty\backslash\mathbb H}f(\tau)\overline{g(\tau)}y^{w+k}\,d\mu\\
&=\int_0^\infty\int_0^1 f(x+iy)\overline{g(x+iy)}y^{w+k-2}\,dx\,dy.
\end{aligned}
$$

Absolute unfolding is justified by replacing $f\overline g$ by $|fg|$ and using the same finite fundamental-domain integral with $E(\tau,\operatorname{Re}w)$. The subsequent termwise integrations can be justified particularly economically by [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md): on each horizontal line,

$$
\int_0^1|f(x+iy)g(x+iy)|\,dx
\leq\left(\sum_{n\geq1}|a_n|^2e^{-4\pi ny}\right)^{1/2}
\left(\sum_{n\geq1}|b_n|^2e^{-4\pi ny}\right)^{1/2}.
$$

The coefficient bounds make the right side $O(y^{-k-1})$ as $y\downarrow0$, and it decays exponentially as $y\to\infty$. Multiplication by $y^{\operatorname{Re}w+k-2}$ is integrable at [zero](../../../../../zero-of-a-function.md) when $\operatorname{Re}w>2$. Thus the integral of the inner [Fourier series](../../../../../fourier-series-split.md) may be evaluated first. [Orthogonality](../../../../../orthogonal-vectors.md) of the exponentials gives

$$
\int_0^1 f(x+iy)\overline{g(x+iy)}\,dx
=\sum_{n\geq1}a_n\overline{b_n}e^{-4\pi ny}.
$$

The [Mellin transform](../../../../../mellin-transform.md) of each exponential is

$$
\int_0^\infty e^{-4\pi ny}y^{w+k-2}\,dy
=\frac{\Gamma(w+k-1)}{(4\pi n)^{w+k-1}}.
$$

In the same initial region the sum of the absolute values of these integrals is finite by $a_n\overline{b_n}=O(n^k)$. Consequently the exact [Rankin–Selberg integral](../../../../../rankin-selberg-integral-for-holomorphic-cusp-forms.md) identity is

$$
\boxed{I(f,g,w)=\frac{\Gamma(w+k-1)}{(4\pi)^{w+k-1}}D(f,g,w+k-1).}
$$

In particular the two parameters are not equal: the [Dirichlet series](../../../../../dirichlet-series.md) argument is shifted by $k-1$.

The holomorphy of $I$ on $\operatorname{Re}w>1$ now gives the required continuation:

$$
\boxed{D(f,g,s)=\frac{(4\pi)^s}{\Gamma(s)}I(f,g,s-k+1),\qquad \operatorname{Re}s>k.}
$$

The right side agrees with the original [Dirichlet series](../../../../../dirichlet-series.md) on $\operatorname{Re}s>k+1$ and is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on the larger half-plane. No continuation of the [Eisenstein series](../../../../../eisenstein-series.md) beyond $\operatorname{Re}w>1$ is needed.

It is important to supply a further argument for [absolute convergence](../../../../../absolute-convergence.md): analytic continuation alone does not imply it. For real $w>1$, both $E(\tau,w)$ and $|f(\tau)|^2$ are nonnegative, and their fundamental-domain integral is finite by the cusp estimates above. [Tonelli theorem](../../../../../tonelli-theorem.md) therefore unfolds $I(f,f,w)$ even before knowing convergence of the [Dirichlet series](../../../../../dirichlet-series.md). On each fixed horizontal line, the [Fourier series](../../../../../fourier-series-split.md) converges absolutely and uniformly, so integration in $x$ gives

$$
\int_0^1|f(x+iy)|^2\,dx=\sum_{n\geq1}|a_n|^2e^{-4\pi ny}.
$$

A second use of [Tonelli theorem](../../../../../tonelli-theorem.md), now in $y$, proves the [positive unfolding of a cusp-form square](../../../../../positive-unfolding-of-a-cusp-form-square.md):

$$
I(f,f,w)=\frac{\Gamma(w+k-1)}{(4\pi)^{w+k-1}}
\sum_{n\geq1}\frac{|a_n|^2}{n^{w+k-1}}<\infty.
$$

Since every real $s>k$ has $s=w+k-1$ with $w>1$, we have **[absolute convergence](../../../../../absolute-convergence.md) of $D(f,f,s)$ for $\operatorname{Re}s>k$**. [Absolute convergence](../../../../../absolute-convergence.md) for complex $s$ follows by taking its real part. In fact [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) also gives [absolute convergence](../../../../../absolute-convergence.md) of $D(f,g,s)$ there from the two corresponding square sums.

Finally let $\sigma>(k+1)/2$ and choose $k<\beta<2\sigma-1$. The preceding square-coefficient bound and [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) give

$$
\sum_{n\geq1}|a_n|n^{-\sigma}
\leq\left(\sum_{n\geq1}|a_n|^2n^{-\beta}\right)^{1/2}
\left(\sum_{n\geq1}n^{-(2\sigma-\beta)}\right)^{1/2}<\infty.
$$

This proves [absolute convergence of cusp-form L-series from square coefficients](../../../../../absolute-convergence-of-cusp-form-l-series-from-square-coefficients.md), and hence

$$
\boxed{L(f,s)\text{ converges absolutely for }\operatorname{Re}s>\frac{k+1}{2}.}
$$

Equivalently, the suggested elementary inequality works by choosing $k-\sigma<\alpha<\sigma-1$: after multiplication by $n^{-\sigma}$ its two bounds sum to a convergent $\sum n^{-(\sigma-\alpha)}$ and a convergent $\sum|a_n|^2n^{-(\sigma+\alpha)}$. The existence of this interval is precisely $2\sigma>k+1$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
