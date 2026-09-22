<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The rational approximation below is taken in lowest terms, $(a,q)=1$, with $1\le q\le Q$, and $X>0$. This is necessary for denominator-sensitive [exponential sum](../../../../../exponential-sum.md) estimates and for the final [Ramanujan sum](../../../../../ramanujan-sum.md) to equal $\mu(q)$. If $0<X<1$, the defining sum over $a\le X$ is empty and $S_4=0$; hence we may assume $1\le X<\sqrt N$.

Set $c_u=\sum_{a\mid u,\ a\le X}\mu(a)$, so $|c_u|\le\tau(u)$, and write the given [Vaughan identity](../../../../../vaughan-s-identity.md) term as the [Type II sum](../../../../../type-ii-sum.md)

$$
S_4=-\sum_{\substack{u>X,\ d>X\\ud\le N}}c_u\Lambda(d)e(\theta ud),\qquad e(t)=e^{2\pi it}.
$$

Use a [dyadic decomposition](../../../../../dyadic-decomposition.md) into $u\in(U,2U]$, $d\in(D,2D]$, retaining $ud\le N$. Empty blocks may be discarded; every remaining block has $U,D\ge X$, $UD<N$, and there are $O(\log^2(2N))$ blocks. Denote a block by $T$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
|T|^2\le\left(\sum_{U<u\le2U}|c_u|^2\right)
\sum_{U<u\le2U}\left|\sum_{\substack{D<d\le2D\\ud\le N}}\Lambda(d)e(\theta ud)\right|^2.
$$

By the allowed [divisor-square summatory bound](../../../../../divisor-square-summatory-bound.md), the first factor is $O(U\log^3(2N))$. Expand the second factor. The diagonal $d_1=d_2$ contributes $O(UD\log^2(2N))$, using $0\le\Lambda(d)\le\log(2N)$. For a pair $d_1\ne d_2$, the allowed $u$ form the interval

$$
U<u\le\min(2U,N/d_1,N/d_2).
$$

Thus the [exponential geometric sum bound](../../../../../exponential-geometric-sum-bound.md) applies to this interval even though the original block has a hyperbolic cutoff. For each difference $h=|d_1-d_2|\le D$, there are $O(D)$ ordered pairs, giving an upper bound

$$
\ll D\log^2(2N)\left(U+\sum_{1\le h\le D}\min(CU,\|\theta h\|^{-1})\right)
$$

for the expanded second factor, with an absolute constant $C$ accommodating integer endpoints. The supplied [reciprocal fractional-part sum near a rational](../../../../../reciprocal-fractional-part-sum-near-a-rational.md), with $M\asymp D$ and $R\asymp U$, bounds the last sum by

$$
O\left((UD/q+U+q+D)\log(2N)\right).
$$

One may also derive this directly from the [separated reciprocal-distance sum](../../../../../separated-reciprocal-distance-sum.md) by splitting $h$ into blocks of length at most $q/2$; the approximation error between two block points is at most $1/(2q)$, and the rational rotations are separated by $1/q$.

Combining the estimates yields

$$
|T|^2\ll UD\left(UD/q+U+q+D\right)\log^6(2N).
$$

Since $UD<N$ and $U,D\ge X$, both $U,D\le N/X$. Taking square roots proves

$$
|T|\ll\left(\frac N{\sqrt q}+\frac N{\sqrt X}+\sqrt{Nq}\right)\log^3(2N).
$$

Summing the dyadic blocks establishes the [rational-phase Type II estimate](../../../../../rational-phase-type-ii-estimate.md) and, in particular, the requested bound with an explicit logarithmic power:

$$
\boxed{|S_4|\ll\left(\frac N{\sqrt q}+\frac N{\sqrt X}+\sqrt{Nq}\right)\log^5(2N).}
$$

The [Siegel–Walfisz theorem](../../../../../siegel-walfisz-theorem.md) states that for fixed $A,C>0$, uniformly for $q\le(\log N)^A$ and $(b,q)=1$,

$$
\psi(N;q,b):=\sum_{\substack{n\le N\\n\equiv b\pmod q}}\Lambda(n)
=\frac N{\varphi(q)}+O_{A,C}\left(N(\log N)^{-C}\right).
$$

The constant is allowed to be ineffective. Apply this with $C=A+B+2$ to the reduced residue classes. Their contribution to the prime [exponential sum](../../../../../exponential-sum.md) is

$$
\sum_{\substack{n\le N\\(n,q)=1}}\Lambda(n)e(an/q)
=\frac N{\varphi(q)}\sum_{\substack{1\le b\le q\\(b,q)=1}}e(ab/q)
+O_{A,B}\left(N(\log N)^{-B}\right),
$$

since there are at most $q\le(\log N)^A$ residue classes. To evaluate the [Ramanujan sum](../../../../../ramanujan-sum.md), the [Möbius divisor-sum identity](../../../../../mobius-divisor-sum-identity.md) gives $\mathbf1_{(b,q)=1}=\sum_{d\mid(b,q)}\mu(d)$. Then the [finite geometric series](../../../../../finite-geometric-series.md) gives

$$
\begin{aligned}
c_q(a)&=\sum_{d\mid q}\mu(d)\sum_{v=1}^{q/d}e(av/(q/d))\\
&=\sum_{\substack{m\mid q\\m\mid a}}m\mu(q/m).
\end{aligned}
$$

When $(a,q)=1$, only $m=1$ remains, giving $c_q(a)=\mu(q)$. The omitted nonunits contribute only [prime powers](../../../../../prime-power.md) $p^j$ with $p\mid q$. For each such prime, the sum of their [Von Mangoldt function](../../../../../von-mangoldt-function.md) weights is at most $\log N$, so their total is at most $\omega(q)\log N=O_A(\log N\log\log(3N))$, absorbed by the stated error. This proves the [major-arc value of the prime exponential sum](../../../../../major-arc-value-of-the-prime-exponential-sum.md):

$$
\boxed{\widehat\Lambda_N(a/q)=\frac{\mu(q)}{\varphi(q)}N
+O_{A,B}\left(N(\log N)^{-B}\right)\quad((a,q)=1).}
$$

The original PDF does not state coprimality in this last request. Without it the asserted main term is genuinely false: $a=q=2$ makes $e(an/q)=1$ and hence $\widehat\Lambda_N(a/q)=\psi(N)\sim N$, whereas $\mu(2)/\varphi(2)=-1$. For an arbitrary numerator the correct main term is $N c_q(a)/\varphi(q)$, with $c_q(a)$ given by the divisor formula above. Reducing the fraction before applying the boxed result is the equivalent repair.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
