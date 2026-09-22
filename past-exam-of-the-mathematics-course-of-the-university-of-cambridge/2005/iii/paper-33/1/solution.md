<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use a fixed [logarithm](../../../../../logarithm.md) base $b>1$, and write $c=\log_b e=1/\ln b$. All [relative entropies](../../../../../kullback-leibler-divergence.md) below use this same base. Adopt $0\log(0/q)=0$ and $p\log(p/0)=+\infty$ for $p>0$.

For [Gibbs inequality](../../../../../gibbs-inequality.md), if $q(x)=0<p(x)$ at some point, the [relative entropy](../../../../../kullback-leibler-divergence.md) is infinite and the required conclusion is immediate. Otherwise let $S=\{x:p(x)>0\}$. The elementary inequality $\ln u\leq u-1$, with equality only at $u=1$, gives, for every $x\in S$,

$$
p(x)\log_b\frac{p(x)}{q(x)}\geq c\bigl(p(x)-q(x)\bigr).
$$

Consequently

$$
D(p\Vert q)\geq c\left(1-\sum_{x\in S}q(x)\right)\geq0.
$$

This argument applies to a countable [discrete probability distribution](../../../../../discrete-probability-distribution-split.md) too: the difference between the two sides of the pointwise inequality is nonnegative, and the negative part of the entropy summand is bounded by $cq(x)$, hence summable. Thus no subtraction of divergent series is involved. Equality forces both $\sum_Sq=1$ and equality in every pointwise inequality; hence $q(x)=p(x)$ on $S$ and $q=0=p$ off $S$. Conversely $p=q$ plainly gives zero. Therefore $\boxed{D(p\Vert q)\geq0,\quad D(p\Vert q)=0\iff p=q}$.

For the [log-sum inequality](../../../../../log-sum-inequality.md), set $F=\sum_Af$, $G=\sum_Ag$, and normalize to the [probability distributions](../../../../../probability-distribution.md) $p_A=f/F$, $q_A=g/G$. When $A$ is nonempty, positivity ensures $F,G>0$, and direct expansion gives

$$
\sum_{x\in A}f(x)\log_b\frac{f(x)}{g(x)}
=F D(p_A\Vert q_A)+F\log_b\frac FG
\geq F\log_b\frac FG.
$$

Thus **normalization reduces the log-sum inequality to Gibbs inequality**. Equality holds exactly when $f/F=g/G$. The empty-set case is the zero identity under the usual zero-mass convention.

For the final bound, partition the alphabet using $A=\{x:p(x)>q(x)\}$ and put $a=p(A)$, $d=q(A)$. Since the total signed difference is zero,

$$
a-d=\sum_{x\in A}(p(x)-q(x))
=\frac12\sum_x|p(x)-q(x)|.
$$

Apply the [log-sum inequality](../../../../../log-sum-inequality.md) separately to $A$ and its complement. The same normalization argument works for countable sets of finite total mass, using the countable [Gibbs inequality](../../../../../gibbs-inequality.md) just proved. It yields the [binary partition bound for relative entropy](../../../../../binary-partition-bound-for-relative-entropy.md)

$$
D(p\Vert q)\geq a\log_b\frac ad+(1-a)\log_b\frac{1-a}{1-d}.
$$

Zero block masses are interpreted by the stated conventions; a positive mass divided by zero makes the bound infinite. The given binary estimate now implies

$$
D(p\Vert q)\geq2c(a-d)^2
=\boxed{\frac{\log_b e}{2}\left(\sum_x|p(x)-q(x)|\right)^2}.
$$

This is [Pinsker's inequality](../../../../../pinsker-s-inequality.md). Equivalently, for the [total variation distance](../../../../../total-variation-distance.md) $\|p-q\|_{\mathrm{TV}}=\frac12\sum_x|p(x)-q(x)|$, the bound is $D(p\Vert q)\geq2\log_b e\,\|p-q\|_{\mathrm{TV}}^2$. The factor $\log_b e$ keeps the statement valid for either bits or natural-logarithm units.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
