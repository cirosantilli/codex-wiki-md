<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $i(G)$ be the number of [independent sets](../../../../../../independent-set-graph-theory.md) of the [biregular graph](../../../../../../biregular-graph.md) $G$. Choose one such set $I$ uniformly and write $X_v=\mathbf1_{v\in I}$. All [information entropies](../../../../../../information-entropy.md) below use logarithms to base two, so

$$
H(X_U,X_W)=\log_2 i(G).
$$

We will prove $\boxed{i(G)\leq(2^r+2^s-1)^{m/s}}$.

We state and justify the entropy facts used. For a finite-valued [random variable](../../../../../../random-variable-split.md) $Y$, $H(Y)=-\sum_y p_y\log_2p_y$ with $0\log_20=0$. Its [conditional entropy](../../../../../../conditional-entropy.md) is the mean of this quantity over the conditioning variable. Factoring the joint probabilities proves the [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md), $H(Y,Z)=H(Y)+H(Z\mid Y)$. [Conditioning reduces entropy](../../../../../../conditioning-reduces-entropy.md): $H(Y\mid Z,T)\leq H(Y\mid Z)$. To see this, condition on $Z$ and use concavity of $-x\log_2x$ to compare the mixture of the conditional distributions given $T$ with their mean entropy.

The precise [Shearer inequality](../../../../../../shearer-s-inequality.md) needed here is: if subsets $S_j$ of the indices of a finite [random vector](../../../../../../random-vector.md) $Y$ cover every index at least $d$ times, then $dH(Y)\leq\sum_jH(Y_{S_j})$. To prove it, order the indices. The [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md) expands

$$
H(Y_{S_j})=\sum_{u\in S_j}H(Y_u\mid Y_v:v\in S_j,\ v<u)
\geq\sum_{u\in S_j}H(Y_u\mid Y_v:v<u).
$$

The inequality is [conditioning reduces entropy](../../../../../../conditioning-reduces-entropy.md). Summing over $j$ counts each nonnegative conditional term at least $d$ times and proves the assertion.

For every $w\in W$, its [vertex neighbourhood](../../../../../../vertex-neighbourhood.md) $N(w)\subseteq U$ has $s$ vertices. Every $u\in U$ lies in exactly $r$ of these neighbourhoods. Hence [Shearer inequality](../../../../../../shearer-s-inequality.md) gives

$$
H(X_U)\leq\frac1r\sum_{w\in W}H(X_{N(w)}).
$$

Let $q_w=\mathbb P(X_{N(w)}=0)$, the [probability](../../../../../../probability.md) that no neighbour of $w$ is selected. Conditional on a particular selected subset of $U$, a vertex $w$ with a selected neighbour is forbidden, and all other vertices of $W$ are available. Because there are no [edges](../../../../../../edge-of-a-graph.md) within $W$, every subset of the available vertices is a valid completion. Uniform choice of $I$ makes these completions equally likely. The available coordinates are therefore independent fair binary choices, each of entropy one, and the forbidden coordinates are zero. Averaging their number gives

$$
H(X_W\mid X_U)=\sum_{w\in W}q_w.
$$

By the [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md),

$$
\log_2i(G)\leq\frac1r\sum_{w\in W}\bigl(H(X_{N(w)})+rq_w\bigr).
$$

It remains to bound each bracket. Let $Y=X_{N(w)}$, a binary vector of length $s$, with distribution $(p_y)$ on $\{0,1\}^s$, and put $Z=2^r+2^s-1$. Assign weight $w_0=2^r$ to the all-zero vector and weight $w_y=1$ to every nonzero vector. Then

$$
H(Y)+rq_w=\sum_{y:p_y>0}p_y\log_2\frac{w_y}{p_y}
\leq\log_2\left(\sum_{y:p_y>0}w_y\right)
\leq\log_2Z.
$$

The first inequality is [Jensen's inequality](../../../../../../jensen-s-inequality.md) for the concave logarithm; the weights sum to $2^r+(2^s-1)$. This explicitly handles zero probabilities and does not assume the neighbourhood indicators are independent.

There are $n$ right vertices, so combining the bounds and using $rm=sn$ gives

$$
\log_2i(G)\leq\frac nr\log_2Z=\frac ms\log_2Z.
$$

Exponentiating proves the required [independent-set bound for biregular graphs](../../../../../../independent-set-bound-for-biregular-graphs.md). The proof uses both degree constraints: $r$ supplies the neighbourhood-cover multiplicity and the conditional-completion weight, while $s$ determines the number of neighbourhood patterns.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
