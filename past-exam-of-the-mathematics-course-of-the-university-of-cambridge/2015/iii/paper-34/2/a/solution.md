<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [expected value](../../../../../../expected-value.md) and [variance](../../../../../../variance-split.md) under [quota share reinsurance](../../../../../../quota-share-reinsurance.md) follow by scaling the [exponential distribution](../../../../../../exponential-distribution.md):

$$
\boxed{\mathbb E S_I^*=\alpha\mu_S,\qquad
\operatorname{Var}(S_I^*)=\alpha^2\mu_S^2.}
$$

The [retained stop loss moments for an exponential aggregate](../../../../../../retained-stop-loss-moments-for-an-exponential-aggregate.md) follow from the payout $Y=\min(S,M)$, its [survival function](../../../../../../survival-function.md) equals $e^{-x/\mu_S}$ for $0\leq x<M$ and zero for $x\geq M$. The [tail integral formula for moments](../../../../../../tail-integral-formula-for-moments.md) gives, with $m=M/\mu_S$ and $r=e^{-m}$,

$$
\mathbb EY=\int_0^M e^{-x/\mu_S}\,dx=\mu_S(1-r),
\qquad
\mathbb EY^2=2\int_0^M xe^{-x/\mu_S}\,dx
=2\mu_S^2[1-(1+m)r].
$$

Consequently **the retained moments are**

$$
\boxed{\mathbb E\widetilde S_I=\mu_S(1-e^{-M/\mu_S}),\qquad
\operatorname{Var}(\widetilde S_I)
=\mu_S^2[1-2(M/\mu_S)e^{-M/\mu_S}-e^{-2M/\mu_S}].}
$$

Matching the two [expected values](../../../../../../expected-value.md) forces $\alpha=1-r$, which lies strictly between zero and one. The difference of the [variances](../../../../../../variance-split.md) simplifies to

$$
\boxed{\operatorname{Var}(S_I^*)-\operatorname{Var}(\widetilde S_I)
=2\mu_S^2e^{-M/\mu_S}
\left(\frac M{\mu_S}-1+e^{-M/\mu_S}\right)\geq0.}
$$

Indeed $h(m)=m-1+e^{-m}$ has $h(0)=0$ and $h'(m)=1-e^{-m}\geq0$ for $m\geq0$. Because $M>0$, the difference is actually positive. At equal retained [expected value](../../../../../../expected-value.md), [aggregate stop loss reinsurance](../../../../../../aggregate-stop-loss-reinsurance.md) reduces the [variance](../../../../../../variance-split.md) more than [quota share reinsurance](../../../../../../quota-share-reinsurance.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
