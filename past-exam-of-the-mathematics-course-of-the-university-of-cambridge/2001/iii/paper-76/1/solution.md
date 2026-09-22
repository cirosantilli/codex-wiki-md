<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $e(t)=e^{2\pi it}$ and let $P(n)=\theta n^k+\cdots$ be a real polynomial of degree $k\ge2$. A standard form of [Weyl inequality](../../../../../weyl-inequality.md) is: if $(a,q)=1$ and $|\theta-a/q|\le q^{-2}$, then for every $\eta>0$

$$
\boxed{\left|\sum_{n=1}^Ne(P(n))\right|\ll_{k,\eta}N^{1+\eta}
\left(\frac1q+\frac1N+\frac q{N^k}\right)^{1/2^{k-1}}.}
$$

The implied constant is uniform in all lower coefficients. For degree one the [finite geometric series](../../../../../finite-geometric-series.md) bound is $|\sum e(\theta n+\beta)|\le\min(N,(2\|\theta\|)^{-1})$, where $\|t\|$ is distance to the nearest integer.

Here is the [Weyl differencing](../../../../../weyl-differencing.md) proof. Extend $z_n=e(P(n))$ by zero outside $[1,N]$. Expanding $|\sum z_n|^2$ by differences of indices gives a sum of correlations $\sum_nz_{n+h}\overline{z_n}$. Repeated [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and this correlation identity yield, after $k-1$ steps, with $p=2^{k-1}$,

$$
|S|^p\ll_k N^{p-k}
\sum_{|h_1|,\ldots,|h_{k-1}|<N}
\left|\sum_{n\in I(\mathbf h)}e(\Delta_{h_{k-1}}\cdots\Delta_{h_1}P(n))\right|.
$$

The interval $I(\mathbf h)$ ensures that every shifted argument remains in $[1,N]$. For completeness, the induction is the following: at stage $j$, the factor is $N^{2^j-j-1}$ and there is a sum over $j$ shifts. Squaring, [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md) over those $O(N^j)$ shifts supplies $N^j$; expanding the square of each remaining interval sum introduces the next shift. The new factor is $N^{2^{j+1}-j-2}$, as asserted for stage $j+1$.

The final differenced phase is linear, of slope $k!\theta h_1\cdots h_{k-1}$. Zero products contribute $O_k(N^{k-1})$ to the sum. For nonzero products the [finite geometric series](../../../../../finite-geometric-series.md) bound applies. Grouping by $r=|h_1\cdots h_{k-1}|\le N^{k-1}$, the [subpower bound for the divisor function](../../../../../subpower-bound-for-the-divisor-function.md) bounds the number of representations by $O_{k,\rho}(N^\rho)$ for any chosen $\rho>0$. The divisor input is elementary: for $t=k-1$, the number of ordered factorizations of $r$ is $\prod_{p^v\parallel r}\binom{v+t-1}{t-1}$. For all sufficiently large primes this is bounded factorwise by $p^{\epsilon v}$, and for the finitely many smaller primes the polynomial in $v$ is bounded by a constant times $p^{\epsilon v}$. Multiplication gives $O_{t,\epsilon}(r^\epsilon)$. Thus

$$
|S|^p\ll_{k,\rho}N^{p-k}\left[N^{k-1}+N^\rho\sum_{r\le N^{k-1}}
\min(N,\|k!\theta r\|^{-1})\right].
$$

The reduced denominator of $k!a/q$ is between $q/k!$ and $q$. Its approximation error is bounded by a constant depending on $k$ times the inverse square of that denominator. Split the $r$-range into blocks of length a sufficiently small fixed multiple of $q$. Within a block the values $k!\theta r$ are separated modulo one by a constant multiple of $1/q$: rational differences have spacing at least $1/q$, while the approximation error in a block difference is smaller than half that spacing. At most a bounded number of values occupy each distance interval of width $1/q$. Summing reciprocals of their ordered distances proves the [reciprocal fractional-part sum near a rational](../../../../../reciprocal-fractional-part-sum-near-a-rational.md) estimate

$$
\sum_{r\le N^{k-1}}\min(N,\|k!\theta r\|^{-1})
\ll_k\left(\frac{N^{k-1}}q+1\right)(N+q\log(2q)).
$$

For $q>N^k$, the proposed inequality follows from $|S|\le N$. Otherwise the last display and the differencing estimate give

$$
|S|^p\ll_{k,\rho}N^{p+\rho}\log(2N)
\left(q^{-1}+N^{-1}+qN^{-k}\right).
$$

Choose $\rho$ sufficiently small, absorb the logarithm into a further arbitrarily small power of $N$, and take $p$th roots. This proves the stated [Weyl inequality](../../../../../weyl-inequality.md).

For the recurrence assertion, a rational $a=u/v$ gives an integer $am^2$ with $m=v$. For irrational $a$, [Weyl differencing](../../../../../weyl-differencing.md) implies that $am^2$ is an [equidistributed sequence](../../../../../equidistributed-sequence.md) modulo one. One way to avoid a rate issue for unusually good rational approximations is to keep a fixed differencing range $H$: the [Van der Corput inequality for finite scalar sequences](../../../../../van-der-corput-inequality-for-finite-scalar-sequences.md) gives, for each nonzero integer $j$, a limsup bound $\limsup_N|N^{-1}\sum_{m\le N}e(jam^2)|^2\ll1/H$, because every fixed nonzero difference has irrational linear slope and its geometric average tends to zero. Let $H\to\infty$ and apply the [Weyl criterion](../../../../../weyl-criterion.md). Hence some $m$ always enters the open $\epsilon$-neighborhood of zero.

Finally, $U_m=\{a\in\mathbb R/\mathbb Z:\|am^2\|<\epsilon\}$ are open sets covering the compact [circle group](../../../../../circle-group.md). A finite subcover has a largest index $N$. **That single $N$ works for every real $a$.** This is [uniform square recurrence on the circle](../../../../../uniform-square-recurrence-on-the-circle.md); the compactness step gives existence, not an explicit quantitative bound.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
