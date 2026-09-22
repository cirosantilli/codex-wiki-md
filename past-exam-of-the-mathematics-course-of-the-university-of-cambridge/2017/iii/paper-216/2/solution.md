<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $\mathcal E$ for the directed edges from parent to child and $x_v(i)$ for the state at site $i$. The [global Markov property for an undirected graph](../../../../../global-markov-property-for-an-undirected-graph.md) on this [tree](../../../../../tree-graph-theory.md), together with the specified parent transitions, gives the complete-data [likelihood function](../../../../../likelihood-function.md)

$$
p_K(x)=4^{-k}\prod_{(v,w)\in\mathcal E}\prod_{i=1}^kK(x_v(i),x_w(i)).
$$

One can obtain the factorization by successively removing terminal subtrees: after conditioning on their parent, each subtree is independent of the rest. The root factor and transition products also show that different sites are independent. Only ancestral states are [latent variables](../../../../../latent-variable.md).

At the current [Markov kernel](../../../../../markov-kernel.md) $K^{(o)}$, define expected transition counts

$$
N_{ab}=\sum_{i=1}^k\sum_{(v,w)\in\mathcal E}
\Pr_{K^{(o)}}(X_v(i)=a,X_w(i)=b\mid\text{observed leaves}).
$$

The E-step of the [expectation-maximization algorithm](../../../../../expectation-maximization-algorithm.md) is

$$
Q(K\mid K^{(o)})=\text{constant}+\sum_{a,b}N_{ab}\log K(a,b).
$$

Maximize separately for each row under $K(a,b)\geq0$ and $\sum_bK(a,b)=1$. For $N_a=\sum_bN_{ab}>0$, the [Lagrange multiplier](../../../../../lagrange-multiplier.md) equation is $N_{ab}/K(a,b)=N_a$, with zero-count entries set to zero at a boundary maximum. Thus the [EM transition-count update on a tree](../../../../../em-transition-count-update-on-a-tree.md) is

$$
\boxed{K^{\mathrm{new}}(a,b)=\frac{N_{ab}}{\sum_cN_{ac}}.}
$$

If $N_a=0$, that row does not occur in $Q$; any row [probability distribution](../../../../../probability-distribution.md), including its previous value, maximizes the objective.

The expected counts can be computed exactly by the [Felsenstein pruning algorithm](../../../../../felsenstein-pruning-algorithm.md) and an outward [belief propagation](../../../../../belief-propagation.md) pass. For one site, let $L_v(a)$ be the [conditional probability](../../../../../conditional-probability.md) of observations in the subtree below $v$, given state $a$. For a leaf $v$ with observed state $d_v$, $L_v(a)=\mathbf1_{\{a=d_v\}}$. For an internal vertex,

$$
L_v(a)=\prod_{w\text{ child of }v}\sum_bK^{(o)}(a,b)L_w(b),\qquad
Z_i=\frac14\sum_a L_{v_0}(a).
$$

Define $A_v(a)$ as the joint mass of state $a$ at $v$ and all observations outside its subtree. The root has $A_{v_0}(a)=1/4$. For a child $w$ of $v$, put

$$
S_{vw}(a)=\prod_{u\text{ child of }v,\ u\ne w}\sum_cK^{(o)}(a,c)L_u(c),\qquad
A_w(b)=\sum_a A_v(a)S_{vw}(a)K^{(o)}(a,b).
$$

The edge [posterior probability](../../../../../posterior-probability.md) required above is

$$
\xi_{vw}^{(i)}(a,b)=\frac{A_v(a)S_{vw}(a)K^{(o)}(a,b)L_w(b)}{Z_i}.
$$

Multiply the inside and outside factors to obtain the joint mass of the observations and endpoint states; division by the site [likelihood function](../../../../../likelihood-function.md) proves this expression. Sum $\xi$ over edges and sites to form $N_{ab}$. The two passes take $O(k|\mathcal E|4^2)=O(kn)$ operations on a binary [tree](../../../../../tree-graph-theory.md). Scaling messages or computing them logarithmically avoids underflow.

A strictly positive initial [Markov kernel](../../../../../markov-kernel.md) ensures $Z_i>0$ for every observed leaf pattern, so every E-step is defined. At a later boundary iterate, require positive likelihood for the actual data and restrict the [conditional distribution](../../../../../conditional-distribution.md) to its support. [EM likelihood monotonicity](../../../../../em-likelihood-monotonicity.md) proves that the update cannot decrease observed-data [likelihood function](../../../../../likelihood-function.md). It is a maximum-likelihood iteration, not a guarantee of finding the global [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md); different initial kernels may lead to different stationary points.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 216](../../paper-216-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
