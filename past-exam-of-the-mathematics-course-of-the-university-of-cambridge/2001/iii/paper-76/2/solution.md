<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

[Vinogradov's three-primes theorem](../../../../../vinogradov-s-three-primes-theorem.md) states that every sufficiently large odd positive integer is a sum of three primes, with repetitions allowed. The parity restriction is a genuine local obstruction to the main asymptotic, not merely a technical convenience.

Let $n$ be large and define the prime-weighted [exponential sum](../../../../../exponential-sum.md)

$$
S(\theta)=\sum_{m\le n}\Lambda(m)e(m\theta),\qquad
R_\Lambda(n)=\sum_{m_1+m_2+m_3=n}\Lambda(m_1)\Lambda(m_2)\Lambda(m_3),
$$

where $\Lambda$ is the [Von Mangoldt function](../../../../../von-mangoldt-function.md). [Character orthogonality](../../../../../character-orthogonality.md) gives the [Hardy-Littlewood circle method](../../../../../hardy-littlewood-circle-method.md) identity

$$
R_\Lambda(n)=\int_0^1S(\theta)^3e(-n\theta)\,d\theta.
$$

The task is to extract a positive main term from rational neighborhoods and make the remaining integral smaller.

Take $Q=(\log n)^B$, with a fixed sufficiently large $B$, and use [major arcs](../../../../../major-arc.md) $|\theta-a/q|\le Q/n$ around reduced fractions with $q\le Q$. They are disjoint once $n$ is large relative to $Q^3$. The [minor arcs](../../../../../minor-arc.md) are their complement. On a major arc put $\theta=a/q+\beta$. The [Siegel–Walfisz theorem](../../../../../siegel-walfisz-theorem.md), followed by partial summation in each residue class, gives

$$
S(a/q+\beta)=\frac{\mu(q)}{\varphi(q)}V(\beta)+O_A\big(n(\log n)^{-A}\big),\qquad
V(\beta)=\int_0^n e(\beta t)\,dt,
$$

uniformly on these arcs after choosing the underlying logarithmic error exponent sufficiently large. The reduced residue-class sum is the [Ramanujan sum](../../../../../ramanujan-sum.md) $c_q(a)=\mu(q)$ when $(a,q)=1$. Prime powers dividing $q$ and the partial-summation factor $1+n|\beta|$ are absorbed in the stated error choice.

Cubing and integrating produces the [singular series](../../../../../singular-series.md) and singular integral:

$$
\mathfrak S(n)=\sum_{q\ge1}\frac{\mu(q)^3c_q(n)}{\varphi(q)^3},\qquad
\int_{\mathbb R}V(\beta)^3e(-n\beta)\,d\beta=\frac{n^2}{2}.
$$

The last identity is Fourier inversion for the volume of the simplex $t_1+t_2+t_3=n$, $t_i\ge0$; the upper bounds $t_i\le n$ do not restrict its interior. The tails and approximation errors are $o(n^2)$. Since $\mu(q)^3=\mu(q)$ on squarefree $q$, multiplicativity gives

$$
\mathfrak S(n)=\prod_p\left(1-\frac{c_p(n)}{(p-1)^3}\right),\qquad
c_p(n)=\begin{cases}p-1,&p\mid n,\\-1,&p\nmid n.\end{cases}
$$

For even $n$ the factor at $2$ vanishes. For odd $n$ it is $2$, and

$$
\mathfrak S(n)=2\prod_{\substack{p>2\\p\mid n}}\left(1-\frac1{(p-1)^2}\right)
\prod_{\substack{p>2\\p\nmid n}}\left(1+\frac1{(p-1)^3}\right)
\ge2\prod_{p>2}\left(1-\frac1{(p-1)^2}\right)>0.
$$

The lower bound is uniform in odd $n$. The product converges because the sums of the local deviations converge. It describes how congruence restrictions alter the otherwise random prime-summand density.

For the minor arcs, a Type I/II prime-sum estimate provides the necessary cancellation. One useful form, obtainable from [Vaughan's identity](../../../../../vaughan-s-identity.md) and bilinear estimates, is

$$
S(\theta)\ll\left(nq^{-1/2}+n^{4/5}+(nq)^{1/2}\right)(\log n)^4
$$

when $|\theta-a/q|\le q^{-2}$. [Dirichlet's approximation theorem](../../../../../dirichlet-s-approximation-theorem.md) supplies a denominator $q\le n/Q$ with $|\theta-a/q|\le Q/(qn)$. On the minor arcs its denominator must exceed $Q$, so both denominator-dependent terms are at most $n/\sqrt Q$. Choosing $B$ large gives $\sup_{\mathfrak m}|S(\theta)|=o(n/\log n)$. The mechanism is to split $\Lambda$ into short-divisor Type I sums and bilinear Type II sums; geometric-sum bounds treat Type I, while [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md) exposes correlations and rational spacing in Type II. The displayed estimate is the substantive analytic input, rather than a consequence of bounding each summand separately.

Meanwhile [Parseval identity](../../../../../parseval-identity.md) and the elementary prime-weight second moment give

$$
\int_0^1|S(\theta)|^2\,d\theta=\sum_{m\le n}\Lambda(m)^2\ll n\log n.
$$

Therefore

$$
\left|\int_{\mathfrak m}S(\theta)^3e(-n\theta)\,d\theta\right|
\le\sup_{\mathfrak m}|S|\int_0^1|S|^2=o(n^2).
$$

Combining the two regions yields $R_\Lambda(n)=\tfrac12\mathfrak S(n)n^2+o(n^2)$. Proper prime powers account for only $O(n^{3/2}(\log n)^4)$: there are $O(\sqrt n\log n)$ such choices for one coordinate, at most $n$ choices for another, and each weight is at most $\log n$. Hence they cannot account for the positive main term. The weighted count using primes alone is positive for every sufficiently large odd $n$, proving the asserted representation. **The conclusion is the sufficiently-large three-prime theorem**; no verification of every small odd integer is supplied by this argument.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
