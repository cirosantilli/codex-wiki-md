<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the probability-system convention $\mu(X)=1$. The [Birkhoff ergodic theorem](../../../../../birkhoff-ergodic-theorem.md), also called the [pointwise ergodic theorem](../../../../../birkhoff-ergodic-theorem.md), states that for a [measure-preserving system](../../../../../measure-preserving-system.md) and $f\in L^1(\mu)$,

$$
A_Nf(x)=\frac1N\sum_{n=0}^{N-1}f(T^nx)
\longrightarrow\mathbb E_\mu[f\mid\mathcal I](x)
\quad\text{almost everywhere},
$$

where $\mathcal I$ is the [invariant sigma-algebra](../../../../../invariant-sigma-algebra.md). The limit is integrable and has the same integral as $f$. On a probability space the convergence also holds in $L^1$, as in the allowed mean ergodic theorem. If $T$ is an [ergodic transformation](../../../../../ergodicity.md), $\mathcal I$ is trivial modulo null sets, giving

$$
\boxed{A_Nf(x)\longrightarrow\int_X f\,d\mu\quad\text{almost everywhere}.}
$$

The [integer multiplication map on the circle](../../../../../integer-multiplication-map-on-the-circle.md) preserves [Lebesgue measure](../../../../../lebesgue-measure.md): for any integrable $g$ on $[0,1)$,

$$
\int_0^1g(Kx\bmod1)\,dx
=\sum_{j=0}^{K-1}\int_{j/K}^{(j+1)/K}g(Kx-j)\,dx
=\int_0^1g(y)\,dy.
$$

To prove the [ergodicity of integer multiplication on the circle](../../../../../ergodicity-of-integer-multiplication-on-the-circle.md), suppose $u\in L^2(m)$ satisfies $u\circ T_K=u$. Let $c_j$ be its [Fourier coefficients](../../../../../fourier-coefficient.md) in the [Fourier basis](../../../../../fourier-basis.md) $e_j(x)=e^{2\pi ijx}$. Since $e_j\circ T_K=e_{Kj}$, the [Fourier coefficients](../../../../../fourier-coefficient.md) of $u\circ T_K$ at index $j$ are zero if $K$ does not divide $j$, and are $c_{j/K}$ otherwise. This identity holds for all $L^2$ functions by approximation with [trigonometric polynomials](../../../../../trigonometric-polynomial.md) and the isometry $u\mapsto u\circ T_K$. Invariance gives

$$
c_j=\begin{cases}c_{j/K},&K\mid j,\\0,&K\nmid j.\end{cases}
$$

Every nonzero integer $j$ can be divided by $K$ only finitely often. Thus $c_j=0$ for every $j\ne0$, and completeness of the [Fourier basis](../../../../../fourier-basis.md) makes $u$ constant [almost everywhere](../../../../../almost-everywhere.md). Applying this to the [indicator function](../../../../../indicator-function.md) of an invariant set gives measure zero or one, so

$$
\boxed{T_K\text{ is ergodic for }m\quad(K\geq2).}
$$

A [normal number](../../../../../normal-number.md) in base $K$ has every word $w=(w_1,\ldots,w_r)$ of $r$ base-$K$ digits occurring with limiting overlapping frequency $K^{-r}$. Use the expansion that is not eventually equal to $K-1$ when there are two expansions. The word $w$ corresponds to the half-open interval

$$
I_w=\left[\frac{j(w)}{K^r},\frac{j(w)+1}{K^r}\right),\qquad
j(w)=\sum_{i=1}^r w_iK^{r-i}.
$$

A word starting at position $n+1$ occurs exactly when $T_K^nx\in I_w$. The [Birkhoff ergodic theorem](../../../../../birkhoff-ergodic-theorem.md), applied to $\mathbf1_{I_w}$, gives frequency $m(I_w)=K^{-r}$ [almost everywhere](../../../../../almost-everywhere.md). There are countably many pairs $(K,w)$, so their full-measure sets have a full-measure intersection. In particular,

$$
\boxed{m\{x\in[0,1):x\text{ is normal in every integer base }K\geq2\}=1.}
$$

These are [absolutely normal numbers](../../../../../absolutely-normal-number.md), so existence follows as well. This interval description also proves [normality and equidistribution under integer multiplication](../../../../../normality-and-equidistribution-under-integer-multiplication.md): the base-$K$ intervals form arbitrarily fine grids, so their frequencies imply the correct frequency for every interval by approximation from inside and outside.

For the growth assertion, put $g=|f|$. For every $\varepsilon>0$, the [Tonelli theorem](../../../../../tonelli-theorem.md) gives the useful summability bound

$$
\sum_{n=1}^\infty\mu(g>\varepsilon n)
=\int_X\sum_{n=1}^\infty\mathbf1_{\{g(x)>\varepsilon n\}}\,d\mu(x)
\leq\frac{\|f\|_1}{\varepsilon}.
$$

Since $T$ is a [measure-preserving transformation](../../../../../measure-preserving-transformation.md), $\mu(g\circ T^n>\varepsilon n)=\mu(g>\varepsilon n)$. The first [Borel-Cantelli lemma](../../../../../borel-cantelli-lemmas.md) shows that $g(T^nx)>\varepsilon n$ occurs only finitely often [almost everywhere](../../../../../almost-everywhere.md). Intersecting the resulting full-measure sets for $\varepsilon=1,1/2,1/3,\ldots$ proves the [linear growth bound for integrable observables](../../../../../linear-growth-bound-for-integrable-observables.md), $f(T^nx)/n\to0$. Multiplication by $n^{1-a}\leq1$ then gives

$$
\boxed{\frac{f(T^nx)}{n^a}\longrightarrow0\quad\text{almost everywhere, for every }a\geq1.}
$$

The threshold is sharp. For $0<a<1$, choose $p$ with $1<p<1/a$, and take the [Bernoulli shift](../../../../../bernoulli-shift.md) on $X=(0,1)^{\mathbb Z}$ with the [product measure](../../../../../product-measure.md) of independent uniform coordinates. The left shift preserves that measure because it preserves the probability of every finite-coordinate event. Define $f(x)=x_0^{-1/p}$; it is integrable because

$$
\int_X f\,d\mu=\int_0^1u^{-1/p}\,du=\frac{p}{p-1}<\infty.
$$

The variables $f(T^nx)=x_n^{-1/p}$ are independent. For any fixed $M\geq1$,

$$
\mu\{f(T^nx)>Mn^a\}=M^{-p}n^{-ap},\qquad ap<1.
$$

The probability sum diverges, so the second [Borel-Cantelli lemma](../../../../../borel-cantelli-lemmas.md) makes these events occur infinitely often [almost surely](../../../../../almost-sure-convergence.md). Intersecting over positive integer $M$ even yields $\limsup_n f(T^nx)/n^a=\infty$. For $a\leq0$, the constant observable $f=1$ already fails to give limit zero. Thus the [sharpness of the linear growth bound for integrable observables](../../../../../sharpness-of-the-linear-growth-bound-for-integrable-observables.md) gives

$$
\boxed{\text{There is no }a<1\text{ for which the asserted limit holds in every system for every }f\in L^1.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 108](../../paper-108-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
