<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For [discrete random variables](../../../../../discrete-random-variable.md), write $p(u,v)$ for the joint [probability mass function](../../../../../probability-mass-function.md) and $p_U(u)$ for its marginal. The [conditional entropy](../../../../../conditional-entropy.md) is the average of the entropies of the conditional distributions:

$$
h(V\mid U)=-\sum_{u:p_U(u)>0}\sum_vp(u,v)\log p(v\mid u),
\qquad p(v\mid u)=\frac{p(u,v)}{p_U(u)}.
$$

Conditional distributions at zero-probability values of $u$ can be chosen arbitrarily; they contribute nothing. Here $h$ denotes [Shannon entropy](../../../../../information-entropy.md), with one common [logarithm](../../../../../logarithm.md) base and $0\log0=0$.

For $p(u,v)>0$, use $\log p(u,v)=\log p_U(u)+\log p(v\mid u)$ and sum with weight $-p(u,v)$. Summing out $v$ in the first term gives

$$
\boxed{h(U,V)=h(U)+h(V\mid U)}.
$$

For countable alphabets, the entropy contributions are nonnegative, so the equality remains valid with extended values by summing nonnegative terms. Applying this identity successively to the prefix $(X_1,\ldots,X_{i-1})$ and $X_i$ proves the [chain rule for information entropy](../../../../../chain-rule-for-information-entropy.md):

$$
\boxed{h(X_1,\ldots,X_n)=\sum_{i=1}^n h(X_i\mid X_1,\ldots,X_{i-1})}.
$$

For $i=1$, the conditioning tuple is empty and the term is $h(X_1)$.

For the subset inequalities, first suppose the marginal entropies are finite, so all [joint entropies](../../../../../joint-entropy.md) below are finite by the chain rule and the assumed [conditioning reduces entropy](../../../../../conditioning-reduces-entropy.md) property. Put $H=h(X_1,\ldots,X_n)$, and let $H_{-i}$ be the [joint entropy](../../../../../joint-entropy.md) with coordinate $i$ omitted. Apply the two-variable chain rule in the order $(X_{[n]\setminus\{i\}},X_i)$ to get

$$
H-H_{-i}=h(X_i\mid X_{[n]\setminus\{i\}})
\leq h(X_i\mid X_1,\ldots,X_{i-1}).
$$

The inequality holds because the prefix conditioning set is contained in the set of all other coordinates. Summing over $i$ and using the chain rule gives

$$
nH-\sum_{i=1}^nH_{-i}\leq H,
\qquad\text{so}\qquad
\sum_{i=1}^nH_{-i}\geq(n-1)H.
$$

This proves [Han's entropy inequality](../../../../../han-s-entropy-inequality.md). In terms of the [normalized subset entropy](../../../../../normalized-subset-entropy.md), $h_n^{(n)}=H/n$ and $h_{n-1}^{(n)}=\sum_iH_{-i}/[n(n-1)]$, hence $\boxed{h_n^{(n)}\leq h_{n-1}^{(n)}}$ for $n\geq2$.

Apply the same result to each $k$-element coordinate set $S$. It gives

$$
(k-1)h(X_S)\leq\sum_{i\in S}h(X_{S\setminus\{i\}}).
$$

When this is summed over all $k$-subsets, each fixed $(k-1)$-subset $T$ occurs once for each possible added coordinate, namely $n-k+1$ times. Therefore

$$
(k-1)\sum_{|S|=k}h(X_S)
\leq(n-k+1)\sum_{|T|=k-1}h(X_T).
$$

Substitute $\sum_{|S|=k}h(X_S)=k\binom nk h_k^{(n)}$ and the analogous identity at $k-1$. The [binomial coefficient](../../../../../binomial-coefficient.md) identity $k\binom nk=(n-k+1)\binom n{k-1}$ cancels the common positive factor and gives

$$
\boxed{h_k^{(n)}\leq h_{k-1}^{(n)}\quad(2\leq k\leq n)}.
$$

This is the [monotonicity of normalized subset entropies](../../../../../monotonicity-of-normalized-subset-entropies.md), obtained from the local $k$-coordinate inequality by explicit counting.

If some marginal entropy is infinite, each subset average contains at least one subset including that coordinate. The entropy of such a subset is at least that marginal entropy, by the nonnegative conditional-entropy chain rule, so every $h_k^{(n)}$ is infinite. The inequalities then hold in the extended sense. Otherwise the finite-entropy proof applies. For [independent random variables](../../../../../independent-random-variables.md) the averages are all $n^{-1}\sum_i h(X_i)$; repeated copies of one variable instead give $h_k^{(n)}=h(X_1)/k$, illustrating the entropy reduction caused by redundancy.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
