<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a fixed $\alpha<1/2$. On the stated high-probability event, strictly more than half of the block means satisfy, simultaneously for every $\|v\|_2\leq1$,

$$
\left|\overline X_{B_j}^Tv-\mu_0^Tv\right|
\leq c_\alpha
\sqrt{\frac{\max\{\operatorname{tr}(\Sigma),\|\Sigma\|_2k\}}n}.
$$

The [median](../../../../../../median.md) of a collection with a strict majority in an interval lies in that interval. Hence the same bound holds for $|\operatorname{MOM}_k(Xv)-\mu_0^Tv|$ uniformly in $v$. Part b then gives

$$
\|\widehat\mu(X)-\mu_0\|_2
\leq2c_\alpha
\sqrt{\frac{\max\{\operatorname{tr}(\Sigma),\|\Sigma\|_2k\}}n}
$$

with probability at least $1-e^{-k/c_\alpha}$. Renaming the constant proves the claim.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
