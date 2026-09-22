<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the usual [aggregate claims model](../../../../../../aggregate-claims-model.md) assumption that the [claim count](../../../../../../claim-count.md) $N$ is independent of the sequence of severities. Conditional on $N=n$, the [probability generating function](../../../../../../probability-generating-function.md) of the sum is the product of the $n$ severity generating functions. The empty sum has value zero. Thus the [law of total expectation](../../../../../../law-of-total-expectation.md) gives the [random-sum transform identity](../../../../../../random-sum-transform-identity.md)

$$
G_S(z)=\sum_{n\geq0}p_nG_X(z)^n,\qquad\boxed{G_S(z)=G_N(G_X(z))},
$$

for $|z|<1$, with the usual continuous interpretation at $z=1$.

For a [claim count distribution](../../../../../../claim-count-distribution.md) in the [Panjer claim-count class](../../../../../../panjer-claim-count-class.md), multiply the count recurrence by $n z^{n-1}$ and sum. With $m=n-1$,

$$
G_N'(z)=\sum_{n\geq1}(an+b)p_{n-1}z^{n-1}=a\sum_{m\geq0}mp_mz^m+(a+b)\sum_{m\geq0}p_mz^m.
$$

Consequently $(1-az)G_N'=(a+b)G_N$, or

$$
\boxed{G_N'(z)=\frac{a+b}{1-az}G_N(z).}
$$

The [chain rule](../../../../../../chain-rule.md) applied to the composition then gives

$$
(1-aG_X)G_S'=(a+b)G_SG_X',\qquad\boxed{G_S'=aG_S'G_X+(a+b)G_SG_X'.}
$$

For $r\geq1$, compare the coefficients of $z^{r-1}$. The two products give

$$
rg_r=a\sum_{j=0}^{r-1}(r-j)f_jg_{r-j}+(a+b)\sum_{j=1}^rjf_jg_{r-j}.
$$

Move the $j=0$ term to the left and combine the remaining coefficients, since $a(r-j)+(a+b)j=ar+bj$. The [Panjer recursion with zero severities](../../../../../../panjer-recursion-with-zero-severities.md) is therefore

$$
\boxed{g_r=\frac1{1-af_0}\sum_{j=1}^r\left(a+\frac{bj}{r}\right)f_jg_{r-j}\qquad(r\geq1).}
$$

For the usual nondegenerate proper Panjer laws, $a<1$, so $1-af_0>0$. If a degenerate count $N\equiv0$ is represented by redundant constants making this denominator zero, the aggregate is identically zero and must be handled directly rather than dividing by zero.

Because severities are nonnegative, the aggregate is zero exactly when every included severity is zero. Count-severity independence gives the initialization

$$
\boxed{g_0=\mathbb P(S=0)=\sum_{n\geq0}p_nf_0^n=G_N(f_0).}
$$

In particular $g_0$ generally exceeds $p_0$ when zero severities are possible.

The count-severity independence is necessary and is implicit, rather than explicitly stated, in the printed random-sum setup. For a concrete counterexample without it, take independent Bernoulli-$1/2$ variables $X_j$ and put $N=X_1$. Then $S=X_1$, so $G_S(z)=(1+z)/2$, whereas $G_N(G_X(z))=(3+z)/4$. Independence of the $X_j$ among themselves alone cannot justify the requested formula.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
