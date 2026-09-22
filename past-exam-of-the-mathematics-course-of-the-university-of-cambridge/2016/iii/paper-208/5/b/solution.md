<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [support condition for importance sampling](../../../../../../support-condition-for-importance-sampling.md) is missing from the printed assertion. Assume $M>1$, $E_f|h|<\infty$, and $Mg(z)>f(z)$ for $f$-almost every $z$. For a proposal $Z\sim g$, rejection has conditional probability $1-f(Z)/(Mg(Z))$. Its unconditional probability is $(M-1)/M$, so the [conditional density](../../../../../../conditional-density.md) of a rejected draw is

$$
r(z)=\frac{g(z)(1-f(z)/(Mg(z)))}{(M-1)/M}=\frac{Mg(z)-f(z)}{M-1}.
$$

Thus the rejected-draw weight is precisely $f(z)/r(z)$, and

$$
E_r\left[h(Z)\frac{(M-1)f(Z)}{Mg(Z)-f(Z)}\right]
=\int h(z)f(z)\,dz.
$$

Conditionally on any positive rejection count $n$ among $N$ independent proposals, the rejected locations have this iid [conditional density](../../../../../../conditional-density.md). Hence

$$
\boxed{\frac1n\sum_{i=1}^nh(Z_i)\frac{(M-1)f(Z_i)}{Mg(Z_i)-f(Z_i)}}
$$

is an [unbiased estimator](../../../../../../unbiased-estimator.md) conditionally on $n$, and therefore also conditionally on the event $0<n<N$. This is [importance sampling](../../../../../../importance-sampling.md) from the [rejected-proposal distribution](../../../../../../rejected-proposal-distribution.md).

The nonstrict assumption $f\leq Mg$ alone does not suffice: the rejected distribution may completely miss part of the target support. For example, let $g$ be uniform on $[0,1]$, $f(z)=2\mathbf1_{[0,1/2]}(z)$, $M=2$, and $h=1$. All rejected proposals lie in $(1/2,1]$, where $f=0$, so the displayed estimator is always $0$, whereas $E_fh=1$. This remains a counterexample after conditioning on $0<n<N$. A strict envelope, such as choosing $M$ larger than the essential supremum of $f/g$, repairs the missing support condition. Near-equality can still give high-[variance](../../../../../../variance-split.md) weights, even when it remains an [unbiased estimator](../../../../../../unbiased-estimator.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
