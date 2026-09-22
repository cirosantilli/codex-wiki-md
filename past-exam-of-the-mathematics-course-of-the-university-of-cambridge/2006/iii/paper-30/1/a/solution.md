<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use base-two logarithms and the convention $0\log_2 0=0$. Write $p_y=\mathbb P(Y=y)$ and $q_y(x)=\mathbb P(X=x\mid Y=y)$ for $p_y>0$. The [conditional entropy](../../../../../../conditional-entropy.md) is the average of the [information entropies](../../../../../../information-entropy.md) of these conditional laws:

$$
H(X\mid Y)=\sum_{y:p_y>0}p_yH(q_y)
=-\sum_{y:p_y>0}\sum_xp_yq_y(x)\log_2q_y(x).
$$

The careful form of [Gibbs inequality](../../../../../../gibbs-inequality.md) is that, for two [probability mass functions](../../../../../../probability-mass-function.md) $q,p$ on a common countable set,

$$
D(q\Vert p)=\sum_xq(x)\log_2\frac{q(x)}{p(x)}\geq0,
$$

where a term with $q(x)>0=p(x)$ gives $+\infty$. Equality holds exactly when $q=p$. This is the nonnegativity of [relative entropy](../../../../../../kullback-leibler-divergence.md).

First suppose $H(X)<\infty$. For every $y$ of positive probability, $q_y(x)>0$ implies $p_X(x)>0$. Averaging the cross-entropies gives

$$
\sum_y p_y\sum_xq_y(x)\bigl(-\log_2p_X(x)\bigr)
=\sum_xp_X(x)\bigl(-\log_2p_X(x)\bigr)=H(X).
$$

All the summands here are nonnegative, so interchanging the sums is valid, and each conditional cross-entropy is finite. Applying [Gibbs inequality](../../../../../../gibbs-inequality.md) to each $q_y,p_X$ shows that $H(q_y)$ is at most its cross-entropy. Subtracting and averaging therefore gives

$$
H(X)-H(X\mid Y)
=\sum_{y:p_y>0}p_yD(q_y\Vert p_X)\geq0.
$$

Every term on the right is nonnegative. The [equality in the entropy conditioning inequality](../../../../../../equality-in-the-entropy-conditioning-inequality.md) is thus equivalent to $q_y=p_X$ for all $p_y>0$, which is exactly factorization of the joint [probability mass function](../../../../../../probability-mass-function.md). Consequently

$$
\boxed{H(X\mid Y)\leq H(X),\qquad
H(X)<\infty:\ H(X\mid Y)=H(X)\iff X,Y\text{ are independent}.}
$$

For arbitrary countable [discrete random variables](../../../../../../discrete-random-variable.md), the inequality remains valid in $[0,\infty]$: the case $H(X)=\infty$ is immediate. The finite-entropy condition is necessary for the usual equality characterization. For example, let $\mathbb P(A=n)=c/(n(\ln n)^2)$ for $n\geq2$, with $c$ the normalizing constant, and let $B$ be an independent fair bit. The series defining the [probability mass function](../../../../../../probability-mass-function.md) converges, whereas its [information entropy](../../../../../../information-entropy.md) diverges like $\sum_n1/(n\ln n)$. Then $X=(A,B)$ and $Y=B$ are dependent, but $H(X)=H(X\mid Y)=\infty$. In the infinite case, equality means precisely that the [conditional entropy](../../../../../../conditional-entropy.md) is also infinite; it does not imply [independent random variables](../../../../../../independent-random-variables.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
