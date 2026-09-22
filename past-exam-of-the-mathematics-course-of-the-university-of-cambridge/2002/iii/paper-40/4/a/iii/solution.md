<h1 id="4/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [Gaussian likelihood Gibbs annealing](../../../../../../../gaussian-likelihood-gibbs-annealing.md) target $\pi_T(\mu,v)\propto L(\mu,v)^{1/T}$ relative to $d\mu\,dv$, with $S>0$. Completing the normal square and recognizing an inverse-gamma kernel give

$$
\boxed{\mu\mid v,T,x\sim N\left(\bar x,\frac{Tv}{n}\right),\qquad
v\mid\mu,T,x\sim\operatorname{IG}\left(\frac{n}{2T}-1,\frac{S+n(\mu-\bar x)^2}{2T}\right).}
$$

The shape is $n/(2T)-1$, because the [probability density function](../../../../../../../probability-density-function.md) in $v$ is $v^{-n/(2T)}e^{-[S+n(\mu-\bar x)^2]/(2Tv)}$. The base measure matters: inserting a prior factor $1/v$ would change this shape.

Integrating out $\mu$ contributes a factor proportional to $v^{1/2}$, so the marginal is $v\sim\operatorname{IG}(n/(2T)-3/2,S/(2T))$. Thus the joint target is proper for $T<n/3$. Choose a decreasing sequence $0<T_m\leq n/10$ tending to zero and a finite starting value $v_0>0$. At iteration $m$, sample $\mu_m$ from the first conditional using $v_{m-1}$, then sample $v_m$ from the second using $\mu_m$. This is an explicit annealing algorithm entirely using [Gibbs sampling](../../../../../../../gibbs-sampler.md), with all its inverse-gamma moments finite for the convergence proof.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
