<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

For finite [sets](../../../../../set-split.md) $A_1,\ldots,A_s$, the [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) states

$$
\left|\bigcup_{i=1}^sA_i\right|
=\sum_{\varnothing\ne J\subseteq\{1,\ldots,s\}}(-1)^{|J|+1}
\left|\bigcap_{j\in J}A_j\right|.
$$

To prove it, count the contribution of an element lying in exactly $r\ge1$ of the [sets](../../../../../set-split.md). Its total coefficient is

$$
\sum_{j=1}^r(-1)^{j+1}\binom rj=1-(1-1)^r=1,
$$

by the [binomial theorem](../../../../../binomial-theorem.md). An element in none contributes zero. Summing these elementwise counts proves the formula. Applying the same argument to [indicator functions](../../../../../indicator-function.md) and taking [expectations](../../../../../expected-value.md) proves the corresponding probability formula.

Factor $4199=13\cdot17\cdot19$. An integer is [coprime](../../../../../coprime-integers.md) to this product precisely when none of its three [prime factors](../../../../../prime-factor.md) divides it. [Inclusion-exclusion](../../../../../inclusion-exclusion-principle.md) applied to the multiples of those [prime numbers](../../../../../prime-number.md) among $1,\ldots,4199$ gives [Euler's totient function](../../../../../euler-totient-function.md)

$$
\begin{aligned}
\varphi(4199)
&=4199-(323+247+221)+(19+17+13)-1\\
&=4199\left(1-\frac1{13}\right)\left(1-\frac1{17}\right)\left(1-\frac1{19}\right)\\
&=12\cdot16\cdot18=\boxed{3456}.
\end{aligned}
$$

For the survey, let $H,D,S$ be the three detestation [events](../../../../../event.md) and use proportions as [probabilities](../../../../../probability.md). The union $H\cup D$ is the reported total union with the only-$S$ group removed, so $\mathbb P(H\cup D)=0.90-0.27=0.63$. The two-set [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) gives $\mathbb P(H\cap D)=0.45+0.28-0.63=0.10$. Removing the all-three group leaves

$$
\boxed{\mathbb P((H\cap D)\setminus S)=0.10-0.06=0.04.}
$$

The required proportion is **4%**. The separately reported total $S$ proportion is consistent with, but unnecessary for, this calculation.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
