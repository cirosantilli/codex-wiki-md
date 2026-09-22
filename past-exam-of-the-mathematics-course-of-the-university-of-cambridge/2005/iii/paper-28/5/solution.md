<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A suitable [large sieve](../../../../../large-sieve.md) statement is the following. If $\alpha_j$ are separated modulo one by at least $0<\delta\leq1$ and $a_n$ is supported on $N$ consecutive [integers](../../../../../integer.md), then

$$
\sum_j\left|\sum_n a_ne(n\alpha_j)\right|^2
\leq(8N+\delta^{-1})\sum_n|a_n|^2.
$$

The sharper classical constant $N-1+\delta^{-1}$ also suffices, but is unnecessary for the requested bound. This is the [exponential-sum large sieve](../../../../../exponential-sum-large-sieve.md).

Put $M=|A|$, $S(\alpha)=\sum_{n\in A}e(n\alpha)$, and $A_p(r)=\#\{n\in A:n\equiv r\pmod p\}$. By the [orthogonality of roots of unity](../../../../../orthogonality-of-roots-of-unity.md),

$$
\sum_{h=0}^{p-1}|S(h/p)|^2=p\sum_{r=0}^{p-1}A_p(r)^2.
$$

At most $p-k(p)$ of these residue counts are nonzero. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $M^2\leq(p-k(p))\sum_rA_p(r)^2$, and the frequency $h=0$ contributes exactly $M^2$. Thus, if $k(p)<p$,

$$
\sum_{h=1}^{p-1}|S(h/p)|^2
\geq\frac{k(p)}{p-k(p)}M^2
\geq\frac{k(p)}pM^2.
$$

If $k(p)=p$ for some [prime](../../../../../prime-number.md), $A$ is empty and the result is immediate.

All fractions $h/p$, $1\leq h<p$, $p\leq X$, are distinct reduced fractions. Their circular spacing is at least $X^{-2}$, because two distinct fractions of these denominators differ modulo one by at least $1/(pp')$. Apply the [large sieve](../../../../../large-sieve.md) with $a_n=\mathbf1_A(n)$ and $\delta=X^{-2}$, and sum the preceding lower bounds:

$$
M^2\sum_{p\leq X}\frac{k(p)}p
\leq\sum_{p\leq X}\sum_{h=1}^{p-1}|S(h/p)|^2
\leq(8N+X^2)M.
$$

For $M>0$ and a positive sieve denominator, division proves

$$
\boxed{|A|\leq(8N+X^2)
\left(\sum_{p\leq X}\frac{k(p)}p\right)^{-1}.}
$$

When the denominator is zero this asserts no restriction; that degenerate case is interpreted as a vacuous bound.

For the least-nonresidue application, first establish the [positive density of power-smooth integers](../../../../../positive-density-of-power-smooth-integers.md). Fix $\eta=1/k$, with an [integer](../../../../../integer.md) $k\geq2$, and let $H$ tend to infinity. Choose ordered [primes](../../../../../prime-number.md), with repetitions allowed, in the interval

$$
H^{\eta-\eta^2}\leq\ell_1,\ldots,\ell_k\leq H^\eta.
$$

Their product $d$ satisfies $H^{1-\eta}\leq d\leq H$. Every number $m d\leq H$ has $m\leq H^\eta$, so is $H^\eta$-smooth. By [partial summation](../../../../../abel-s-summation-formula.md) of the [Prime number theorem](../../../../../prime-number-theorem.md), or the [Mertens theorem for reciprocal primes](../../../../../mertens-second-theorem.md),

$$
\sum_{H^{\eta-\eta^2}\leq\ell\leq H^\eta}\frac1\ell
\longrightarrow\log\frac\eta{\eta-\eta^2}=-\log(1-\eta)>0.
$$

The number of ordered representations $(m,\ell_1,\ldots,\ell_k)$ is at least

$$
\frac H2\left(\sum_{H^{\eta-\eta^2}\leq\ell\leq H^\eta}\frac1\ell\right)^k\gg_\eta H,
$$

because $\lfloor H/d\rfloor\geq H/(2d)$ for $1\leq d\leq H$.

This representation count must not be confused with a count of distinct [integers](../../../../../integer.md). A number at most $H$ has at most $\lfloor1/(\eta-\eta^2)\rfloor$ [prime factors](../../../../../prime-factor.md) in that interval, counted with multiplicity. There are therefore only a bounded number, depending on $\eta$, of ordered $k$-tuples which can occur as [divisors](../../../../../divisor.md) of it; the cofactor is then fixed. Dividing by this bounded multiplicity proves

$$
\#\{m\leq H:m\text{ is }H^\eta\text{-smooth}\}\geq\kappa_\eta H
$$

for a fixed $\kappa_\eta>0$ and all sufficiently large $H$.

Now work on a dyadic [prime](../../../../../prime-number.md) interval $Q<p\leq2Q$ and let $\mathcal E_Q$ be the [primes](../../../../../prime-number.md) there with $n(p)>p^{0.01}$. Take $H=Q^2$ and $\eta=1/200$, so $H^\eta=Q^{0.01}$. Let $A$ be the $Q^{0.01}$-smooth [integers](../../../../../integer.md) at most $Q^2$. The density lemma gives $|A|\geq\kappa Q^2$ for an absolute $\kappa>0$.

For each $p\in\mathcal E_Q$, every [prime factor](../../../../../prime-factor.md) of a member of $A$ is at most $Q^{0.01}\leq p^{0.01}<n(p)$ and is smaller than $p$. Hence it is a nonzero [quadratic residue](../../../../../quadratic-residue.md) modulo $p$. Multiplicativity of the [Legendre symbol](../../../../../legendre-symbol.md) makes every member of $A$ a nonzero [quadratic residue](../../../../../quadratic-residue.md) modulo $p$. It therefore avoids all $(p-1)/2$ quadratic-nonresidue classes. In the sieve inequality set $k(p)=(p-1)/2$ at exceptional [primes](../../../../../prime-number.md) and zero at every other [prime](../../../../../prime-number.md) up to $X=2Q$. For odd $p$, $k(p)/p\geq1/3$, so

$$
\frac{|\mathcal E_Q|}{3}
\leq\sum_{p\leq2Q}\frac{k(p)}p
\leq\frac{8Q^2+(2Q)^2}{|A|}\leq\frac{12}{\kappa}.
$$

Thus each dyadic interval has at most $36/\kappa$ exceptional [primes](../../../../../prime-number.md). The finitely many small intervals can be absorbed into this absolute bound. Summing the $O(\log N)$ intervals up to $N$ proves the [large-sieve logarithmic exceptional-prime bound for least quadratic nonresidues](../../../../../large-sieve-logarithmic-exceptional-prime-bound-for-least-quadratic-nonresidues.md):

$$
\boxed{\#\{p\leq N:n(p)>p^{0.01}\}\leq C\log N.}
$$

The least nonresidue is normally defined for odd [primes](../../../../../prime-number.md); any convention at the [prime](../../../../../prime-number.md) two changes the count by at most one.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
