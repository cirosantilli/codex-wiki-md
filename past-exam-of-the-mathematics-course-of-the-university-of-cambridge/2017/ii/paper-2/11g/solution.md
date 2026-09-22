<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

For a discrete [random variable](../../../../../random-variable-split.md) with probabilities $p_i$, its [Shannon entropy](../../../../../information-entropy.md) in bits is $H(X)=-\sum_ip_i\log_2p_i$, with $0\log_20=0$. [Gibbs inequality](../../../../../gibbs-inequality.md) states that

$$
D(p\Vert q)=\sum_ip_i\log_2\frac{p_i}{q_i}\geq0,
$$

with equality exactly when $p=q$. If $q_i=0<p_i$, the left side is infinite. Otherwise apply $-\ln u\geq1-u$ to $u=q_i/p_i$ for $p_i>0$:

$$
(\ln2)D(p\Vert q)\geq\sum_{p_i>0}(p_i-q_i)\geq0.
$$

Equality requires $q_i=p_i$ on the support and no remaining mass outside it. In particular, comparison with the uniform [probability distribution](../../../../../probability-distribution.md) on two outcomes gives binary [Shannon entropy](../../../../../information-entropy.md) at most $1$.

Write $q=1-p_1$. For $q>0$, grouping the last two outcomes gives

$$
H(p_1,p_2,p_3)=H(p_1,q)+qH(p_2/q,p_3/q)\leq H(p_1,q)+q.
$$

Equality holds if $p_2=p_3$; if $q=0$ it also holds, and then both are zero. Thus **equality holds exactly when $p_2=p_3$**.

For the [discrete memoryless channel](../../../../../discrete-memoryless-channel.md), assume $\alpha,\beta\geq0$ and $\alpha+\beta\leq1$, and set $w=1-\alpha-\beta$. Both conditional output [probability distributions](../../../../../probability-distribution.md) have [Shannon entropy](../../../../../information-entropy.md) $H(w,\alpha,\beta)$. The third output has [probability](../../../../../probability.md) $\beta$ regardless of the input; the first two have total [probability](../../../../../probability.md) $1-\beta$. Their [Shannon entropy](../../../../../information-entropy.md) is maximized by making them equal, which a uniform input achieves. Hence the [channel capacity](../../../../../channel-capacity.md) is

$$
C=H\left(\frac{1-\beta}{2},\frac{1-\beta}{2},\beta\right)-H(w,\alpha,\beta)
$$

and therefore

$$
\boxed{C=(1-\beta)\bigl[1-\log_2(1-\beta)\bigr]+w\log_2w+\alpha\log_2\alpha.}
$$

The usual zero-times-log convention includes $\beta=1$, when $C=0$. If $w=\alpha$, the rows coincide and every input achieves zero [mutual information](../../../../../mutual-information.md); otherwise the uniform input is the unique maximizing input.

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
