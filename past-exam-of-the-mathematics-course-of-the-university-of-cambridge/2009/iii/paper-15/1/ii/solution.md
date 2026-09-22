<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [incoming-edge coupling of site and bond percolation](../../../../../../incoming-edge-coupling-of-site-and-bond-percolation.md). Start with [independent random variables](../../../../../../independent-random-variables.md) indicating open bonds, each with [probability](../../../../../../probability.md) $q$. For a vertex $v$ of incoming degree $d_v$, let $J_v$ indicate that at least one incoming bond is open. Then

$$
\mathbb P(J_v=1)=1-(1-q)^{d_v}\le r:=1-(1-q)^{\Delta_{\rm in}}.
$$

The indicators $J_v$ are independent: the sets of bonds entering different vertices are disjoint. Using an additional independent coin at each vertex, turn some zeros into ones so that the resulting indicators $S_v$ are independent with common [probability](../../../../../../probability.md) $r$. Explicitly, when $J_v=0$, set $S_v=1$ with conditional [probability](../../../../../../probability.md) $(r-\mathbb P(J_v=1))/(1-\mathbb P(J_v=1))$.

Every vertex other than $x$ in an open [bond percolation](../../../../../../bond-percolation-split.md) out-cluster has an open incoming bond, and is consequently an open site. On $\{S_x=1\}$, the whole bond out-cluster is therefore contained in the [site percolation](../../../../../../site-percolation-split.md) out-cluster. The event of infinite bond reachability does not depend on bonds entering $x$: delete cycles from any finite open [directed path](../../../../../../directed-path.md) starting at $x$. It is thus independent of $S_x$, including its additional coin. Hence

$$
\theta_s(r)\ge r\theta_b(q).
$$

For every $q>p_H^b$ below $1$, monotonicity and the definition of the survival threshold give $\theta_b(q)>0$. Letting $q\downarrow p_H^b$ yields the **quantitative bound**

$$
\boxed{p_H^s(\vec\Lambda;x)\le 1-(1-p_H^b(\vec\Lambda;x))^{\Delta_{\rm in}}.}
$$

In particular, if $p_H^b<1$, the right-hand side is strictly less than $1$. If $p_H^b=1$, no separation from $1$ is implied or generally possible.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
