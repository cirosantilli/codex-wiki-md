<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

On an independent Bernoulli [product measure](../../../../../product-measure.md), the [Harris-Kleitman inequality](../../../../../harris-inequality.md) states that [increasing events](../../../../../increasing-event.md) $E,F$ obey

$$
\boxed{\Pr(E\cap F)\ge\Pr(E)\Pr(F).}
$$

The same holds for two [decreasing events](../../../../../decreasing-event.md); an increasing and a [decreasing event](../../../../../decreasing-event.md) have the reversed inequality.

Prove the stronger function version by induction on the number of coordinates. For increasing bounded functions $f,g$, condition on the last coordinate $Z$, with $\Pr(Z=1)=p$. The [law of total covariance](../../../../../law-of-total-covariance.md) gives

$$
\operatorname{Cov}(f,g)
=\mathbb E[\operatorname{Cov}(f,g\mid Z)]
+p(1-p)(\mathbb E[f\mid1]-\mathbb E[f\mid0])
(\mathbb E[g\mid1]-\mathbb E[g\mid0]).
$$

The first term is nonnegative by induction, and the other factors are nonnegative by monotonicity. The one-coordinate case is the same formula without the first term. Event indicators prove the assertion. Two decreasing functions follow by replacing both by their negatives; replacing only one gives [negative correlation of increasing and decreasing events](../../../../../negative-correlation-of-increasing-and-decreasing-events.md).

Here is a precise [Janson inequality](../../../../../janson-inequality.md) and its lower-tail concentration form. Let $I_i$ indicate containment of a specified set of independent Bernoulli coordinates, set $X=\sum_iI_i$, $\mu=\mathbb EX$, and let

$$
\Delta=\sum_{i\ne j:\,S_i\cap S_j\ne\varnothing}\mathbb E(I_iI_j).
$$

This [Janson dependency sum](../../../../../janson-dependency-sum.md) is ordered and excludes the diagonal. Then

$$
\boxed{\Pr(X=0)\le e^{-\mu+\Delta/2},\qquad
\Pr(X\le\mu-a)\le\exp\left[-\frac{a^2}{2(\mu+\Delta)}\right]\quad(0\le a\le\mu).}
$$

A zero denominator means the trivial case $X=0$ almost surely.

To prove the avoidance bound, expose the avoidance events in order. For a fixed $i$, separate earlier indices into those whose supports are disjoint from $S_i$ and those overlapping it. Write $C$ for avoidance of the first group and $D$ for avoidance of the second. The event $C$ is independent of $I_i$, while $C$ is decreasing and $\{I_i=I_j=1\}$ is increasing. The correlation inequality therefore gives

$$
\Pr(I_i=1\mid C\cap D)
\ge\Pr(I_i=1,D\mid C)
\ge\mathbb EI_i-\sum_{j<i:j\sim i}\mathbb E(I_iI_j).
$$

The first inequality divides a nonnegative numerator by $\Pr(D\mid C)\le1$; the second uses a [union bound](../../../../../boole-s-inequality.md) and negative correlation with $C$. Conditioning events of zero [probability](../../../../../probability.md) already make full avoidance impossible. Multiply the resulting conditional avoidance bounds to obtain the [Janson sequential product lemma](../../../../../janson-sequential-product-lemma.md). Taking logarithms and using $\log(1-u)\le-u$ gives $-\mu+\Delta/2$, since each unordered dependency pair is counted once in the sequential sum.

For the [Janson lower-tail bound by independent thinning](../../../../../janson-lower-tail-bound-by-independent-thinning.md), attach independent selectors of [probability](../../../../../probability.md) $t$ to the events. Their total expectation and dependency sum are $t\mu,t^2\Delta$, so avoidance of the selected events gives

$$
\mathbb E(1-t)^X\le\exp(-t\mu+t^2\Delta/2).
$$

Set $t=1-e^{-s}$ and apply the [exponential Markov bound](../../../../../exponential-markov-bound.md) to $e^{-sX}$. Using $s-s^2/2\le1-e^{-s}\le s$ yields

$$
\Pr(X\le\mu-a)
\le\exp\bigl[-sa+s^2(\mu+\Delta)/2\bigr].
$$

Choosing $s=a/(\mu+\Delta)$ proves the concentration assertion. For avoidance alone, optimizing $-t\mu+t^2\Delta/2$ also gives $e^{-\mu^2/(2\Delta)}$ when $\Delta\ge\mu$, and the original bound gives $e^{-\mu/2}$ when $\Delta\le\mu$.

To outline the sharp chromatic application, view an [independent set](../../../../../independent-set-graph-theory.md) of $G(n,p)$ as a clique of its complement, whose [edge](../../../../../edge-of-a-graph.md) [probability](../../../../../probability.md) is $q=1-p$. Fix $0<\varepsilon<1$, let $m=\lceil n/(\log n)^2\rceil$ and $r=\lfloor(2-\varepsilon)\log_b n\rfloor$. For a particular $m$-vertex set, let $X$ count independent $r$-sets. Then $\mu=\binom mr q^{\binom r2}$, and the overlap calculation gives

$$
\frac{\Delta}{\mu^2}
\le\sum_{\ell=2}^{r-1}
\frac{\binom r\ell\binom{m-r}{r-\ell}}{\binom mr}
 b^{\binom\ell2}
=O_{p,\varepsilon}\left(\frac{r^4}{m^2}\right).
$$

Overlap of only one [vertex](../../../../../vertex-graph-theory.md) shares no [edge](../../../../../edge-of-a-graph.md), hence is independent. For completeness, the summand is at most $(r^2/(m-r))^\ell b^{\binom\ell2}/\ell!$. Since $r\le(2-\varepsilon/2)\log_b m$ eventually, large overlaps are bounded by $m^{-c_\varepsilon\ell}$; finitely many smaller overlaps are dominated by $\ell=2$. Also $\log\mu=\Omega_{p,\varepsilon}((\log m)^2)$, so the diagonal contribution $1/\mu$ is negligible. The concentration bound consequently gives

$$
\Pr(X=0)\le\exp[-c_{p,\varepsilon}m^2/(\log n)^4].
$$

A [union bound](../../../../../boole-s-inequality.md) over at most $2^n$ [vertex](../../../../../vertex-graph-theory.md) sets still tends to zero. Thus [independent sets in every large subset of a dense random graph](../../../../../independent-sets-in-every-large-subset-of-a-dense-random-graph.md) are available uniformly, including adaptively obtained remainders. Repeatedly remove an independent $r$-set and give it a new colour, then colour the fewer than $m$ leftover [vertices](../../../../../vertex-graph-theory.md) individually. This uses at most $n/r+m$ colours. Combining with the first-moment lower bound and letting fixed $\varepsilon$ be arbitrarily small gives the accurate leading asymptotic

$$
\boxed{\chi(G(n,p))=\frac{n}{2\log_b n}(1+o(1))\quad\text{with probability tending to one}.}
$$

The uniform subset estimate, rather than merely the existence of one large [independent set](../../../../../independent-set-graph-theory.md), is what makes the sharp upper bound possible.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
