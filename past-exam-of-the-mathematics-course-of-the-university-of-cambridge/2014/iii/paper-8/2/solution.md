<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [weak topology of probability measures](../../../../../weak-topology-of-probability-measures.md) is the smallest topology making every map $\mu\mapsto\int h\,d\mu$ continuous for bounded continuous real $h$ on $X$. Define the [bounded-Lipschitz metric](../../../../../bounded-lipschitz-metric.md) by

$$
\boxed{\beta(\mu,\nu)=\sup_{\|h\|_\infty+\operatorname{Lip}_d(h)\le1}
\left|\int h\,d\mu-\int h\,d\nu\right|.}
$$

Using the maximum of the two bounds instead of their sum changes the [metric](../../../../../metric.md) by at most a factor of two and gives the same topology. Symmetry and the triangle inequality follow from the supremum formula. Bounded Lipschitz [functions](../../../../../function-split.md) distinguish [probability measures](../../../../../probability-measure.md) by the open-set approximations below, so $\beta$ is a [metric](../../../../../metric.md). **On a separable [metric](../../../../../metric.md) space, $\beta$ induces the weak topology.**

Here are the essential details. If $\beta(\mu_n,\mu)\to0$, integrals of every bounded Lipschitz [function](../../../../../function-split.md) converge after rescaling its Lipschitz bound. For an [open set](../../../../../open-set.md) $A\ne X$, the [functions](../../../../../function-split.md)

$$
h_m(x)=\min\{1,m\,d(x,X\setminus A)\}
$$

increase to $1_A$; for $A=X$ take $h_m=1$. Thus $\mu(A)=\sup_m\int h_m\,d\mu$. It follows both that $\mu\mapsto\mu(A)$ is [lower semicontinuous](../../../../../lower-semicontinuity.md) for the weak topology, as a supremum of continuous maps, and that beta convergence implies

$$
\boxed{\liminf_n\mu_n(A)\ge\mu(A)\quad\text{for every open }A.}
$$

This is the open-set [Portmanteau criterion](../../../../../portmanteau-theorem.md). Its closed-set equivalent, by complements, is

$$
\boxed{\limsup_n\mu_n(F)\le\mu(F)\quad\text{for every closed }F.}
$$

Either family of inequalities is necessary and sufficient for [weak convergence of probability measures](../../../../../weak-convergence-of-probability-measures.md). For sufficiency of the open inequalities, apply the layer-cake formula and [Fatou's lemma](../../../../../fatou-s-lemma.md) to the open superlevel sets of a continuous [function](../../../../../function-split.md) $0\le h\le1$, obtaining $\liminf\int h\,d\mu_n\ge\int h\,d\mu$. Applying the same argument to $1-h$ gives the reverse bound. Scaling handles every bounded continuous [function](../../../../../function-split.md).

Conversely, weak convergence implies beta convergence. Choose a [compact set](../../../../../compact-space.md) $K$ of arbitrarily large $\mu$-mass, using [tightness of a probability measure](../../../../../tightness-of-a-probability-measure.md) on a Polish space. The unit bounded-Lipschitz class is uniformly bounded and equicontinuous on $K$, so finitely many of its members approximate all others uniformly there. On the open $\delta$-neighborhood $K^\delta$, approximation errors increase by at most $2\delta$. The open-set inequality makes $\mu_n(K^\delta)$ large for all sufficiently large $n$. Weak convergence for the finitely many selected [functions](../../../../../function-split.md), combined with these approximation errors and the small mass outside $K^\delta$, bounds the supremum defining $\beta$ by an arbitrarily small number. The same finite-test and open-mass bounds define weak neighborhoods, so the argument gives equality of the topologies, not only their convergent sequences. It does not first assume uniform tightness of the entire sequence.

The map $j=i_*$ is injective and continuous: for $h\in C(\widetilde X)$, $h\circ i$ is bounded continuous on $X$, and $\int h\,dj(\mu)=\int h\circ i\,d\mu$. To prove inverse continuity on its image, suppose $j(\mu_n)\to j(\mu)$. For every open $A\subset X$, there is an open $U\subset\widetilde X$ with $i(A)=U\cap i(X)$. Hence $\mu_n(A)=j(\mu_n)(U)$ and $\mu(A)=j(\mu)(U)$. The open-set criterion on $\widetilde X$ now gives the criterion on $X$, so $\mu_n\to\mu$. Both spaces are metrizable, and this sequential argument proves

$$
\boxed{j:P(X)\longrightarrow j(P(X))\text{ is a homeomorphism}.}
$$

This is the [probability pushforward embedding theorem](../../../../../probability-pushforward-embedding-theorem.md). The printed claim needs the words “onto its image”: it is generally not onto all $P(\widetilde X)$, since a Dirac mass at a point outside $i(X)$ is not in its image. By Question 1, the completely metrizable subspace $i(X)$ is a Borel [G-delta set](../../../../../g-delta-set.md), and

$$
j(P(X))=\{\lambda\in P(\widetilde X):\lambda(i(X))=1\}.
$$

Now let $S$ be weakly closed and [uniformly tight](../../../../../uniform-tightness.md). Take any sequence $(\mu_n)$ in $S$. The space $P(\widetilde X)$ is compact for the weak topology. For completeness, this compactness follows by choosing a countable uniformly dense family in $C(\widetilde X)$, extracting a diagonal subsequence of its bounded integrals, and extending the limits to a positive normalized functional on $C(\widetilde X)$; the [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md) gives the limiting [probability measure](../../../../../probability-measure.md). Thus, along a subsequence, $j(\mu_n)\to\lambda$.

For every $m$, choose compact $K_m\subset X$ with $\mu(K_m)\ge1-2^{-m}$ for every $\mu\in S$. The set $i(K_m)$ is compact and closed in $\widetilde X$, so the closed-set criterion gives

$$
\lambda(i(K_m))\ge\limsup_n j(\mu_n)(i(K_m))\ge1-2^{-m}.
$$

Therefore $\lambda(i(X))=1$, and $\lambda=j(\mu)$ for some $\mu\in P(X)$. Inverse continuity gives $\mu_n\to\mu$, and closedness puts $\mu\in S$. Hence $S$ is sequentially compact, and metrizability makes it compact. This proves the required [closed uniformly tight compactness criterion](../../../../../closed-uniformly-tight-compactness-criterion.md), rather than assuming it from [Prokhorov's theorem](../../../../../prokhorov-s-theorem.md).

Such a compact metrizable extension is always available: for a countable dense set $(x_k)$, the coordinates $d(x,x_k)/(1+d(x,x_k))$ embed $X$ homeomorphically into $[0,1]^{\mathbb N}$. Injectivity and inverse continuity follow by choosing $x_k$ close to a specified point and using the triangle inequality. The closure of the image gives $\widetilde X$.

To show separability of $P(X)$, use finite sums of Dirac [measures](../../../../../measure.md) on a countable dense subset of $X$ with nonnegative rational weights summing to one. This is a countable family. Given $\mu$, cover a large-mass [compact set](../../../../../compact-space.md) by finitely many small balls centered in that subset, move the mass in each piece to its center, and move the remaining small mass to one fixed center. The bounded-Lipschitz error is at most the ball radius plus twice the exceptional mass. Approximate the resulting weights by rational weights. Thus these atomic [measures](../../../../../measure.md) are beta-dense.

Finally use a complete compatible [metric](../../../../../metric.md) $d$ on the Polish space $X$, as required for the granted total-boundedness-to-tightness assertion. A beta-[Cauchy sequence](../../../../../cauchy-sequence.md) is beta-totally bounded, and so is its closure in $P(X)$. By the allowed assertion this closure is uniformly tight; it is weakly closed because the weak and beta topologies agree. The compactness result just proved gives a convergent subsequence, and the Cauchy property forces the whole sequence to converge in beta. Consequently beta is complete for this choice of $d$, and

$$
\boxed{(P(X),w)\text{ is a Polish space}.}
$$

If the originally displayed compatible [metric](../../../../../metric.md) is incomplete, replace it by a complete compatible [metric](../../../../../metric.md) for this last argument; the weak topology itself is unchanged.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
