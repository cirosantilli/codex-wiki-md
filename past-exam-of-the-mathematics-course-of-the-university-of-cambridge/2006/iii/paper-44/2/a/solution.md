<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the incubation times are [independent](../../../../../../independent-random-variables.md) observations from the same upper-[truncated distribution](../../../../../../truncated-distribution.md). Conditional on lying below $M$, the [gamma distribution](../../../../../../gamma-distribution.md) density is $g(t;a,s)/G(M;a,s)$ on its support. With $t_{(n)}=\max_i t_i$, the [likelihood function](../../../../../../likelihood-function.md) is

$$
\boxed{L(a,s,M)=\frac{\prod_{i=1}^n t_i^{a-1}\exp(-t_i/s)}{s^{na}\Gamma(a)^nG(M;a,s)^n}
\mathbf1\{0<t_i<M\text{ for every }i\}.}
$$

In particular, the normalizing factor $G(M;a,s)^{-n}$ cannot be omitted. On the admissible region the [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell=(a-1)\sum_i\log t_i-\frac{\sum_i t_i}{s}
-na\log s-n\log\Gamma(a)-n\log G(M;a,s).
$$

The [profile likelihood](../../../../../../profile-likelihood.md) eliminates the [nuisance parameters](../../../../../../nuisance-parameter.md) $a,s$ by fitting them separately at each candidate endpoint:

$$
L_p(M)=\sup_{a>0,s>0}L(a,s,M).
$$

For fixed $a,s$ and $M>t_{(n)}$,

$$
\frac{\partial\ell}{\partial M}=-n\frac{g(M;a,s)}{G(M;a,s)}<0.
$$

Equivalently, for $t_{(n)}<M_1<M_2$, every nuisance-parameter fit has $L(a,s,M_1)>L(a,s,M_2)$. Taking suprema shows that $L_p$ is nonincreasing. If the nuisance maximum at $M_2$ is attained and finite, evaluating its maximizing parameters at $M_1$ shows strict decrease there as well. Values below the largest observation are inadmissible. Thus [upper-endpoint estimation in a truncated distribution](../../../../../../upper-endpoint-estimation-in-a-truncated-distribution.md) gives the usual boundary estimate

$$
\boxed{\widehat M=t_{(n)}.}
$$

There is a support-convention qualification: the literal strict support $t<M$ excludes $M=t_{(n)}$, so it gives a supremum approached as $M\downarrow t_{(n)}$, rather than an attained [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md). Using the equivalent closed-endpoint density convention for a continuous distribution yields the usual boundary estimate above. The argument presumes a meaningful finite nuisance fit; degenerate samples can instead have an unbounded density [likelihood](../../../../../../likelihood-function.md). Since $M$ changes the support, regular interior-parameter asymptotic formulas are not automatically applicable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
