<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $J$ be a finite collection of resources with positive integer capacities $C_j$, and let $R$ be a finite collection of nonempty routes. In the standard unit-resource [loss network](../../../../../loss-network.md), a call on route $r$ needs one unit simultaneously at each resource in $r$; [fixed routing](../../../../../fixed-routing.md) means that these requirements do not change when a request is rejected. Suppose route $r$ has an independent [Poisson process](../../../../../poisson-process.md) of arrivals of rate $\nu_r$ and independent holding times of mean $1/\mu_r$. Its [offered traffic](../../../../../offered-traffic.md) is $\alpha_r=\nu_r/\mu_r$. The [Erlang fixed point approximation](../../../../../erlang-fixed-point-approximation.md) approximates resource blocking events as independent, rather than claiming this [independence](../../../../../independent-random-variables.md) for the exact [loss network](../../../../../loss-network.md).

Write $b_j$ for the approximate blocking probability at resource $j$. The [reduced-load approximation](../../../../../reduced-load-approximation.md) screens a call by every other resource that it needs, so the [offered traffic](../../../../../offered-traffic.md) seen by resource $j$ is

$$
a_j(b)=\sum_{r:j\in r}\alpha_r\prod_{k\in r\setminus\{j\}}(1-b_k).
$$

For a single resource with [offered traffic](../../../../../offered-traffic.md) $a$ and capacity $C$, the [Erlang loss formula](../../../../../erlang-loss-formula.md) is

$$
E(a,C)=\frac{a^C/C!}{\sum_{k=0}^{C}a^k/k!}.
$$

Thus the [Erlang fixed point approximation](../../../../../erlang-fixed-point-approximation.md) is the system

$$
\boxed{b_j=E(a_j(b),C_j),\qquad j\in J.}
$$

The resulting route acceptance probability is $\prod_{j\in r}(1-b_j)$. In particular, the screening product for $a_j$ excludes $j$ itself; including it would describe a different approximation.

For existence, define $T_j(b)=E(a_j(b),C_j)$ on $[0,1]^J$. Each $a_j$ is a continuous polynomial, and the denominator of the [Erlang loss formula](../../../../../erlang-loss-formula.md) is at least one. Consequently $T$ is continuous and maps this nonempty compact [convex set](../../../../../convex-set.md) into itself. The [Brouwer fixed-point theorem](../../../../../brouwer-fixed-point-theorem.md) supplies a [fixed point](../../../../../fixed-point.md). At any such point $b_j<1$, since finite [offered traffic](../../../../../offered-traffic.md) and positive capacity give $E(a,C)<1$.

For uniqueness, we construct a [strictly convex function](../../../../../strictly-convex-function.md) whose minimizer is equivalent to an [Erlang fixed point](../../../../../erlang-fixed-point-approximation.md). Put $y_j=-\log(1-b_j)$. First establish the single-resource facts needed for this change of coordinates. For $a>0$, the inverse blocking probability has the expression

$$
E(a,C)^{-1}=\sum_{k=0}^{C}\frac{C!}{k!}a^{k-C}.
$$

The terms with $k<C$ decrease strictly with $a$, so $E(a,C)$ increases strictly from zero to one. Let $a_C(y)$ be its inverse parametrization defined by $E(a_C(y),C)=1-e^{-y}$, with $a_C(0)=0$. If $K$ has the truncated [Poisson distribution](../../../../../poisson-distribution.md) with weights proportional to $a^k/k!$, then shifting the sum gives its mean, the [carried load of an Erlang loss resource](../../../../../carried-load-of-an-erlang-loss-resource.md), as

$$
m_C(a)=\mathbb E_aK=a[1-E(a,C)].
$$

Differentiating the normalized weights shows

$$
\frac{d}{da}\mathbb E_aK=\frac{\operatorname{Var}_a(K)}a>0.
$$

The [variance](../../../../../variance-split.md) is positive because both $K=0$ and $K=1$ have positive probability. Moreover, $m_C(a)\to C$ as $a\to\infty$, since the largest term in the truncated [Poisson distribution](../../../../../poisson-distribution.md) dominates. Hence

$$
U_C(y)=e^{-y}a_C(y)=m_C(a_C(y))
$$

is continuous, strictly increasing from zero to $C$.

Now minimize the following [convex potential for the Erlang fixed point](../../../../../convex-potential-for-the-erlang-fixed-point.md) over the nonnegative orthant:

$$
F(y)=\sum_{r\in R}\alpha_r\exp\!\left(-\sum_{j\in r}y_j\right)+\sum_{j\in J}\int_0^{y_j}U_{C_j}(z)\,dz.
$$

Each exponential term is [convex](../../../../../convex-function.md), and each integral is a [strictly convex function](../../../../../strictly-convex-function.md) of its coordinate because its derivative $U_{C_j}$ is strictly increasing. Their sum is therefore [strictly convex](../../../../../strictly-convex-function.md). It is also a [coercive function](../../../../../coercive-function.md): once $z$ is large enough, $U_{C_j}(z)\geq C_j/2$, so each integral grows at least linearly in its coordinate, while the exponential terms are nonnegative. Thus $F$ attains exactly one minimum.

The coordinate derivative is

$$
\partial_jF(y)=U_{C_j}(y_j)-\sum_{r:j\in r}\alpha_r\exp\!\left(-\sum_{k\in r}y_k\right).
$$

At an interior coordinate of a minimizer it vanishes. At $y_j=0$, it is nonpositive, whereas the one-sided minimum condition requires it to be nonnegative; it therefore vanishes there too. Conversely, a zero [gradient](../../../../../gradient.md) is a global minimizer of this [convex function](../../../../../convex-function.md). Multiplying $\partial_jF=0$ by $e^{y_j}$ gives

$$
a_{C_j}(y_j)=\sum_{r:j\in r}\alpha_r\exp\!\left(-\sum_{k\in r\setminus\{j\}}y_k\right)=a_j(b).
$$

Applying the [Erlang loss formula](../../../../../erlang-loss-formula.md) converts this exactly to $b_j=E(a_j(b),C_j)$. The change of coordinates is one-to-one, proving **uniqueness under fixed routing**. A zero-capacity resource can instead be fixed as blocked with probability one, with all routes using it removed before applying the proof; an unused positive-capacity resource has blocking probability zero.

For [alternative routing](../../../../../alternative-routing.md), consider a symmetric three-node [loss network](../../../../../loss-network.md). Each of its three links has capacity $1000$; every node pair offers traffic $950$, tries its direct link first, and, if that link is blocked, tries the two-link path through the third node. Let all approximate link blocking probabilities equal $b$. Each link receives its direct [offered traffic](../../../../../offered-traffic.md) and the overflow from the other two node pairs. An overflow is generated with probability $b$ and reaches the link under consideration only when its other required link accepts, with probability $1-b$. The symmetric [reduced-load approximation](../../../../../reduced-load-approximation.md) therefore gives

$$
b=E(950[1+2b(1-b)],1000).
$$

For $g(b)=E(950[1+2b(1-b)],1000)-b$, evaluate the [Erlang loss formula](../../../../../erlang-loss-formula.md) by the stable recursion $E(a,0)=1$, $E(a,k)=aE(a,k-1)/(k+aE(a,k-1))$. It gives

$$
\begin{array}{c|rrrr}
b&0&0.01&0.1&0.4\\\hline
g(b)&0.00364929&-0.00092309&0.01445982&-0.10951455
\end{array}
$$

These signs can also be certified with exact rational arithmetic, since all four loads are rational. Continuity and the [intermediate value theorem](../../../../../intermediate-value-theorem.md) give three distinct roots, one in each intervening interval. Thus **the alternative-routing approximation need not be unique**. This is multiplicity of approximate [fixed points](../../../../../fixed-point.md), not multiplicity of [stationary distributions](../../../../../stationary-distribution.md) for the exact finite irreducible [Markov chain](../../../../../markov-chain.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
