<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $q$ be the genuine rain probability and $p$ the reported probability. The [linear probability score](../../../../../../linear-probability-score.md) has expected reward

$$
s(p,q)=qp+(1-q)(1-p)=1-q+(2q-1)p.
$$

This is linear in $p$, so its optimal report and expected reward are

$$
\boxed{p^*=1\ (q>1/2),\qquad p^*=0\ (q<1/2),
\qquad s(p^*,q)=\max(q,1-q).}
$$

At $q=1/2$ every report scores $1/2$ on average. Truthful reporting scores $q^2+(1-q)^2$, strictly below the optimum for interior $q\ne1/2$. Thus **the rule is not proper**: it rewards maximal confidence in the more likely outcome. The expected total over days is $\sum_t\max(q_t,1-q_t)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
