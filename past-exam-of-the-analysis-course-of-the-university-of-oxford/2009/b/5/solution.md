<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

With $\widehat f(k)=(2\pi)^{-1}\int_{-\pi}^{\pi}f(s)e^{-iks}ds$, the classical [Fourier partial sum](../../../../fourier-partial-sum.md) is $s_N^f(t)=\sum_{|k|\leq N}\widehat f(k)e^{ikt}$. Its [Cesàro mean](../../../../cesaro-mean.md) is

$$
\sigma_N^f=\frac1{N+1}\sum_{n=0}^Ns_n^f=\sum_{|k|\leq N}\left(1-\frac{|k|}{N+1}\right)\widehat f(k)e^{ikt}.
$$

For the uniform [Fejér theorem](../../../../fejer-s-theorem.md), extend the continuous endpoint-matching $f$ periodically. The given [Fejér kernel](../../../../fejer-kernel.md) is nonnegative, even and has total integral $\pi$. Thus

$$
\sigma_N^f(t)-f(t)=\frac1\pi\int_{-\pi}^{\pi}[f(t-u)-f(t)]F_N(u)du.
$$

Given $\varepsilon>0$, uniform [continuity](../../../../continuous-function.md) supplies $\delta>0$ so the bracket has modulus less than $\varepsilon$ for $|u|<\delta$, uniformly in $t$. That part contributes at most $\varepsilon$. On the remainder, $F_N(u)\leq[2(N+1)\sin^2(\delta/2)]^{-1}$, and the bracket is at most $2\|f\|_\infty$. Hence

$$
\|\sigma_N^f-f\|_\infty\leq\varepsilon+\frac{2\|f\|_\infty}{(N+1)\sin^2(\delta/2)}\longrightarrow\varepsilon.
$$

Letting $\varepsilon$ decrease to zero proves **[uniform convergence](../../../../uniform-convergence.md) of the [Fejér sums](../../../../fejer-sum.md)**.

The later assertions attached to the printed factorial-frequency example are inconsistent. The following calculations resolve them while keeping the Fourier definition just given. Put $a_j=e^{i\sqrt{j+1}}-e^{i\sqrt j}$ and consider its formal trigonometric [series](../../../../series-mathematics.md). For $t=\pi p/q$, there is $J_0$ such that $\cos(j!t)=1$ for every $j\geq J_0$, because $2q$ divides $j!$. At $N_J=(J+1)!-1$, its ordinary partial sum therefore telescopes to

$$
s_{N_J}(t)=C(t)+e^{i\sqrt{J+1}}.
$$

The exponential has subsequences tending to $1$ and $-1$: take $J+1$ to be integers nearest $(2\pi m)^2$ and $((2m+1)\pi)^2$. Thus **the ordinary sums diverge at every $t\in\pi\mathbb Q$**.

But their genuine Fourier [Cesàro means](../../../../cesaro-mean.md) also diverge there. Indeed,

$$
\sigma_{N_J}(t)-s_{N_J}(t)=-\frac1{(J+1)!}\sum_{j=0}^Jj!a_j\cos(j!t).
$$

Since $|a_j|\leq2$ and $\sum_{j=0}^Jj!\leq2J!$ for $J\geq3$, its absolute value is at most $4/(J+1)\to0$, uniformly in $t$. Therefore

$$
\boxed{\sigma_{N_J}(t)=C(t)+e^{i\sqrt{J+1}}+o(1),}
$$

which has the same incompatible limit points. This is an instance of [Cesàro sums at factorial cutoffs track ordinary sums](../../../../cesaro-sums-at-factorial-cutoffs-track-ordinary-sums.md). **The printed Cesàro-convergence claim is false.** Averaging the sparse [series](../../../../series-mathematics.md) by its index $j$ would be a different operation from Fourier Cesàro summation by frequency.

There is a further issue: **no $L^1$ function has exactly this [Fourier series](../../../../fourier-series-split.md)**. Here is a direct proof using [strongly lacunary polynomial L1-L2 bound](../../../../strongly-lacunary-polynomial-l1-l2-bound.md). For a [trigonometric polynomial](../../../../trigonometric-polynomial.md) $p$ supported on $\{\pm j!:j\geq3\}$, consecutive positive frequencies have ratio at least four. Every zero sum of four signed frequencies pairs into cancelling equal frequencies: a largest unpaired frequency would exceed the sum of the other three. Expanding the fourth moment with normalized measure $dt/(2\pi)$ and bounding the three possible pairings gives

$$
\|p\|_4^4\leq3\|p\|_2^4.
$$

The [Holder inequality](../../../../holder-inequality.md) gives $\|p\|_2\leq\|p\|_1^{1/3}\|p\|_4^{2/3}$, hence $\|p\|_2\leq\sqrt3\|p\|_1$.

If the asserted $f\in L^1$ existed, positivity and unit mass of the summation kernel would bound $\|\sigma_N^f\|_1\leq\|f\|_1$. Subtract the finitely many modes from $j<3$; their norms stay uniformly bounded, and the remainder is a [polynomial](../../../../polynomial-split.md) of the type above. Its $L^2$ norms would therefore be uniformly bounded. [Orthogonality](../../../../orthogonal-vectors.md) then forces $\sum_{j\geq3}|a_j|^2<\infty$, by fixing any finite coefficient block and letting $N\to\infty$. However,

$$
|a_j|^2=4\sin^2\left(\frac{\sqrt{j+1}-\sqrt j}{2}\right)\sim\frac1{4j},
$$

so that sum diverges. This contradiction disproves the stated existence premise.

Even considered only formally, these coefficients rule out an $L^2$ function by [Bessel's inequality](../../../../bessel-s-inequality.md), and hence rule out a bounded function on the finite interval. Thus a bounded continuous representative cannot satisfy the asserted [series](../../../../series-mathematics.md) either. **The asserted $L^1$ function does not exist.**

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
