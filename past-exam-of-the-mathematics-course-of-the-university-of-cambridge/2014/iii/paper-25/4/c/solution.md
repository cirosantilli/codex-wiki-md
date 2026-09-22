<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $\varepsilon=1-\sigma\in[0,1)$ and $L=\log(t+2)$. By the [Hardy-Littlewood approximation to the Riemann zeta function](../../../../../../hardy-littlewood-approximation-to-the-riemann-zeta-function.md) at $x=t$, it is enough to bound $\sum_{n\le t}n^{-\sigma-it}$: the integral term has size $O(t^{-\sigma})$ because $|s-1|\ge t$.

On a dyadic interval $(N,N']\subset(N,2N]$ with $N'\le t$, the assumed estimate holds for every initial subinterval. [Abel summation](../../../../../../abel-s-summation-formula.md) with $n^{-\sigma}$ therefore gives

$$
\left|\sum_{N<n\le N'}n^{-\sigma-it}\right|\ll N^\varepsilon\exp\left(-\frac{c(\log N)^2}L\right)+N^{\varepsilon-1/5}.
$$

Indeed the weighted endpoint and integral of the term proportional to the subinterval length are $O(N^{1-\sigma})$, and those of the constant $N^{4/5}$ term are $O(N^{4/5-\sigma})$. The constants can be uniform in $0<\sigma\le1$.

For the first term, write $u=j\log2$ and complete the square:

$$
\varepsilon u-\frac{cu^2}L=-\frac cL\left(u-\frac{\varepsilon L}{2c}\right)^2+\frac{\varepsilon^2L}{4c}.
$$

The sum of a shifted [Gaussian function](../../../../../../gaussian-function.md) on a fixed-spaced lattice is $O(\sqrt L)$, uniformly in the shift. Thus these dyadic contributions are $O(\sqrt L\,e^{\varepsilon^2L/(4c)})$. This is the [Gaussian dyadic summation bound](../../../../../../gaussian-dyadic-summation-bound.md).

For the second term, if $\varepsilon\le1/10$ its dyadic sum is bounded. If $\varepsilon>1/10$, a crude bound is $O(L\exp(\max(\varepsilon-1/5,0)L))$. The positive exponent obeys $\varepsilon-1/5\le(5/4)\varepsilon^2$, and $L$ can be absorbed into $\sqrt L\,e^{C\varepsilon^2L}$ uniformly on $\varepsilon>1/10$ by increasing the fixed constant $C$. The finitely many initial terms cause no problem. We conclude, with one fixed sufficiently large $C$,

$$
\boxed{|\zeta(\sigma+it)|\ll t^{C(1-\sigma)^2}\log^{1/2}t,\qquad0<\sigma\le1.}
$$

In particular the endpoint $\sigma=1$ gives $O(\sqrt{\log t})$ under the assumed exponential-sum hypothesis. This conditional conclusion uses that hypothesis, not an unconditional improvement of the stated [Richert bound for the Riemann zeta function](../../../../../../richert-bound-for-the-riemann-zeta-function.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
