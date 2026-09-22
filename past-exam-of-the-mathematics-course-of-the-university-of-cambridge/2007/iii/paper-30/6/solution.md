<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Extend $f$ by zero outside $[1,N]\cap\mathbb Z$. Here is a dyadic endpoint convention for [small Type I and Type II sums](../../../../../small-type-i-and-type-ii-sums.md). Write $D_M=[M,2M)\cap\mathbb Z$, with $M$ a power of two. [Type I sums](../../../../../type-i-sum.md) are $\delta$-small if, for every $M\le N^{1/100}$, dyadic $K$ with $MK\le N$, and arbitrary integer intervals $I_m\subset D_K$,

$$
\frac1N\sum_{m\in D_M}\left|\sum_{n\in I_m}f(mn)\right|\le\delta.
$$

[Type II sums](../../../../../type-ii-sum.md) are $\delta$-small if, for all dyadic $M,K\in[N^{1/100},N^{99/100}]$ and sequences $|a_m|,|b_n|\le1$,

$$
\frac1N\left|\sum_{m\in D_M}\sum_{n\in D_K}a_mb_nf(mn)\right|\le\delta.
$$

Zero extension handles boxes crossing the endpoint $mn=N$. Fixed choices of open or closed dyadic endpoints do not matter, but interval uniformity and uniformity in both bounded coefficient sequences do matter. These are the estimates used in the [Vinogradov Type I–II method](../../../../../vinogradov-type-i-ii-method.md).

An interesting technical step is [Fourier separation of interval cutoffs](../../../../../fourier-separation-of-interval-cutoffs.md). For an integer interval $I_m$, let $\widehat{1_{I_m}}(\theta)=\sum_{r\in I_m}e(-r\theta)$. Discrete [Fourier inversion](../../../../../fourier-inversion-theorem.md) gives

$$
1_{I_m}(n)=\int_0^1\widehat{1_{I_m}}(\theta)e(n\theta)\,d\theta.
$$

The [exponential geometric sum bound](../../../../../exponential-geometric-sum-bound.md) gives a common envelope $H_N(\theta)\ll\min(N,\|\theta\|^{-1})$, with $\int_0^1H_N\ll\log(2N)$. Divide the interval transform by this envelope: at each frequency it is a bounded coefficient depending on $m$, and $e(n\theta)$ is a bounded coefficient depending on $n$. The [Type II sum](../../../../../type-ii-sum.md) assumption therefore bounds the interval-cutoff sum by $O(\delta N\log N)$. Choosing the outer unit phases to turn each inner sum into its modulus extends the [Type I sum](../../../../../type-i-sum.md) bound to boxes where both variables are in the Type II range.

Take $U=V=\lfloor N^{1/3}\rfloor$. With subscripts denoting truncation of arithmetic functions, the [Vaughan identity](../../../../../vaughan-s-identity.md) is

$$
\Lambda=\Lambda_{\le V}+\mu_{\le U}*\log-\mu_{\le U}*\Lambda_{\le V}*1+\mu_{>U}*\Lambda_{>V}*1,
$$

where $*$ now means [Dirichlet convolution](../../../../../dirichlet-convolution.md). For completeness it follows from $\mu*1=\epsilon$ and $\Lambda*1=\log$: expand $\mu_{>U}*\Lambda_{>V}*1$, cancel the short terms, and retain $\Lambda$. The short first term contributes $O(N^{1/3}\log N)$ to the sum against $f$.

The next two terms give [Type I sums](../../../../../type-i-sum.md). The logarithmic term has outer coefficient $\mu(m)$, $m\le U$, and inner factor $\log n$, removed by [partial summation](../../../../../abel-s-summation-formula.md) at a cost $O(\log N)$. In the other term the outer variable is $m=cd\le UV$ with coefficient

$$
\omega_m=\sum_{\substack{cd=m\\c\le U,d\le V}}\mu(c)\Lambda(d),\qquad |\omega_m|\le\sum_{d\mid m}\Lambda(d)=\log m.
$$

This [logarithmic coefficient bound in Vaughan identity](../../../../../logarithmic-coefficient-bound-in-vaughan-identity.md) avoids a loss from a divisor weight. On boxes with short outer variable use the hypothesis directly; on boxes where both variables are at least $N^{1/100}$ use the extended bound proved above. Boxes with inner variable less than $N^{1/100}$ contain at most $O(N^{2/3+1/100})$ pairs in total and are treated trivially. All remaining inner scales are at most $N^{99/100}$ whenever the outer scale exceeds $N^{1/100}$.

For the final convolution, group the variables as

$$
\sum_{\substack{m>U,n>V\\mn\le N}}\mu(m)b(n)f(mn),\qquad b(n)=\sum_{\substack{d\mid n\\d>V}}\Lambda(d),\qquad 0\le b(n)\le\log n.
$$

Both variables lie between constant multiples of $N^{1/3}$ and $N^{2/3}$, well inside the Type II range. Divide $b(n)$ by $\log N$, and apply the [Type II sum](../../../../../type-ii-sum.md) estimate. If the product cutoff is kept explicitly, [Fourier separation of interval cutoffs](../../../../../fourier-separation-of-interval-cutoffs.md) costs only one extra logarithm; zero extension also permits its omission. There are $O(\log^2N)$ boxes in the [dyadic decomposition](../../../../../dyadic-decomposition.md). The coefficient bound and, where needed, [partial summation](../../../../../abel-s-summation-formula.md) cost at most one more logarithm. These estimates give the convenient bound

$$
\left|\sum_{n\le N}\Lambda(n)f(n)\right|\ll\delta N\log^4N+N^{2/3+1/100}\log N+N^{1/3}\log N.
$$

With $\delta=(\log N)^{-20}$, each term is $o(N)$, proving the assertion. The grouping of the long term uses the nonnegativity of the [Von Mangoldt function](../../../../../von-mangoldt-function.md); more usual groupings instead control a divisor coefficient by a second-moment truncation. [Ben Green's notes, Sections 2.3–2.4](https://arxiv.org/pdf/0710.0823) describe that standard alternative.

Now take the sign version of the [Thue–Morse sequence](../../../../../thue-morse-sequence.md), $f(n)=(-1)^{s_2(n)}$. Concatenation of [binary digits](../../../../../binary-digit.md) gives $f(a2^j+r)=f(a)f(r)$ for $0\le r<2^j$. Expanding over all choices of digits proves the [Thue–Morse Fourier product](../../../../../thue-morse-fourier-product.md)

$$
S_j(\theta):=\sum_{0\le r<2^j}f(r)e(r\theta)=\prod_{l=0}^{j-1}(1-e(2^l\theta)).
$$

Pair adjacent factors. If $u=|\cos(\pi t)|$, their modulus is

$$
|(1-e(t))(1-e(2t))|=8u(1-u^2)\le\frac{16}{3\sqrt3}=:B<4,
$$

since the maximum on $[0,1]$ occurs at $u=1/\sqrt3$. Thus $|S_j(\theta)|\ll2^{\sigma j}$ uniformly, where $\sigma=\frac12\log_2B=2-\frac34\log_23<1$.

Every integer interval $J\subset[0,N]$ is a disjoint union of aligned binary blocks with at most two blocks of each length. On such a block the digit concatenation identity and the [Thue–Morse Fourier product](../../../../../thue-morse-fourier-product.md) give the same bound, up to a unit phase. Summing the [geometric series](../../../../../geometric-series.md) proves the [uniform interval cancellation for binary digit parity](../../../../../uniform-interval-cancellation-for-binary-digit-parity.md)

$$
\sup_{\theta,J}\left|\sum_{r\in J}f(r)e(r\theta)\right|\ll N^\sigma.
$$

For a fixed $m$, the sum $\sum_{n\in I_m}f(mn)$ is a sum over multiples of $m$ in an integer interval $J\subset[1,N]$. The additive [character orthogonality](../../../../../character-orthogonality.md) filter gives

$$
\sum_{\substack{r\in J\\m\mid r}}f(r)=\frac1m\sum_{a=0}^{m-1}\sum_{r\in J}f(r)e(ar/m).
$$

Its modulus is $O(N^\sigma)$, independently of $m$ and the interval. Summing at most $O(N^{1/100})$ outer values proves the [small Type I sums for binary digit parity](../../../../../small-type-i-sums-for-binary-digit-parity.md):

$$
\boxed{\frac1N\sum_{m\in D_M}\left|\sum_{n\in I_m}f(mn)\right|\ll N^{\sigma+1/100-1},\qquad \sigma+1/100<1.}
$$

This is smaller than $(\log N)^{-20}$ for sufficiently large $N$. It proves the required Type I cancellation; the substantially harder Type II cancellation is not needed for this final clause.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
