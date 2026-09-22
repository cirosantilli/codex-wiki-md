<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Only active routes, those with $n_r>0$, enter the [proportional fairness](../../../../../proportional-fairness.md) inequality and the [weighted logarithmic utility](../../../../../weighted-logarithmic-utility.md). Their rates must be positive; inactive routes have no per-flow rate to determine and may be assigned zero. This convention removes otherwise meaningless terms $0\log0$ and $0/0$.

For positive active rates, [concavity of the logarithm](../../../../../concavity-of-the-logarithm.md) gives, for any positive feasible competitor $y$,

$$
\sum_r n_r(\log y_r-\log x_r)\leq\sum_r n_r\frac{y_r-x_r}{x_r}.
$$

Thus the [proportional fairness](../../../../../proportional-fairness.md) inequality proves that $x$ maximizes the log-utility objective. A competitor with an active zero rate has utility $-\infty$ and cannot improve it. Conversely, if $x$ maximizes utility, the right [directional derivative](../../../../../directional-derivative.md) along $x+\varepsilon(y-x)$ at $\varepsilon=0$ is nonpositive, giving exactly that inequality. Positive resource capacities and finitely many active routes allow a feasible allocation with every active rate positive, so an optimizer cannot have an active zero rate. [Strict concavity](../../../../../strict-concavity.md) gives uniqueness of the active rates. Hence **proportional fairness is equivalent to the stated log-utility maximization**.

Index the four adjacent-pair routes in cyclic order and put $z_i=n_ix_i$, the aggregate service on route $i$. The resource constraints are

$$
z_1+z_4\leq1,\quad z_1+z_2\leq1,\quad z_2+z_3\leq1,\quad z_3+z_4\leq1.
$$

They involve every odd-even route pair, so they are equivalent to

$$
p+q\leq1,\qquad p=\max(z_1,z_3),\quad q=\max(z_2,z_4).
$$

For given maxima, increasing each active odd service to $p$ and each active even service to $q$ remains feasible and improves utility. Apart from the constant $-\sum_i n_i\log n_i$, the objective therefore reduces to

$$
P\log p+Q\log q,\qquad P=n_1+n_3,\quad Q=n_2+n_4,\quad p+q\leq1.
$$

When both groups are present the constraint is tight, and differentiation gives $P/p=Q/(1-p)$. If one group is empty, the other receives unit aggregate service on each of its active routes. Thus the [opposite-route reduction for a proportionally fair four-cycle](../../../../../opposite-route-reduction-for-a-proportionally-fair-four-cycle.md) yields, with $T=P+Q>0$,

$$
\boxed{x_i=\begin{cases}P/(Tn_i),&i\in\{1,3\},\ n_i>0,\\Q/(Tn_i),&i\in\{2,4\},\ n_i>0.\end{cases}}
$$

Inactive rates can be set to zero, including every rate in the empty state. In particular $n_{\{1,2\}}x_{\{1,2\}}=(n_{\{1,2\}}+n_{\{3,4\}})/\sum_rn_r$ whenever that route is active. This proves the required formula even when other routes are empty.

For the [flow-level network model](../../../../../flow-level-network-model.md), an active document's residual size retains an [exponential distribution](../../../../../exponential-distribution.md) with parameter $\mu_i$. Receiving service at rate $x_i(n)$ gives completion intensity $\mu_ix_i(n)$, so $n_i$ independent active documents give total completion intensity $\mu_in_ix_i(n)$. Consequently the population [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md) has

$$
\boxed{q(n,n+e_i)=\nu_i,\qquad q(n,n-e_i)=\begin{cases}\mu_i P/T,&i\text{ odd},\ n_i>0,\\\mu_i Q/T,&i\text{ even},\ n_i>0,\\0,&n_i=0.\end{cases}}
$$

All death intensities are zero at $T=0$. Their total is bounded by $\sum_i\mu_i$, and the total arrival rate is constant, proving [nonexplosion](../../../../../nonexplosion-of-a-continuous-time-markov-chain.md).

Put $\rho_i=\nu_i/\mu_i$. The required stationary weight uses a [binomial coefficient](../../../../../binomial-coefficient.md), as printed in the PDF; the converted TeX incorrectly rendered it as an ordinary fraction. Define

$$
w(n)=\binom{T}{P}\prod_{i=1}^4\rho_i^{n_i},\qquad w(0)=1.
$$

For an odd route, the neighboring [binomial coefficient](../../../../../binomial-coefficient.md) ratio is

$$
\frac{w(n+e_i)}{w(n)}=\rho_i\frac{T+1}{P+1},
$$

while its death intensity at the neighboring state is $\mu_i(P+1)/(T+1)$. Their product is $\nu_i$, so $w(n)q(n,n+e_i)=w(n+e_i)q(n+e_i,n)$. For an even route, replace $P$ by $Q$ in the same calculation. This proves [detailed balance](../../../../../detailed-balance.md) and the [stationary law of a proportionally fair four-cycle](../../../../../stationary-law-of-a-proportionally-fair-four-cycle.md):

$$
\boxed{\pi(n)=B^{-1}\binom{\sum_i n_i}{n_1+n_3}\prod_{i=1}^4\left(\frac{\nu_i}{\mu_i}\right)^{n_i},\qquad B=\sum_{n\in\mathbb Z_+^4}w(n).}
$$

A finite $B$ is essential for this expression to be a [probability distribution](../../../../../probability-distribution.md). We determine its exact convergence condition rather than asserting stationarity for arbitrary arrival rates. Let

$$
h_p(a,c)=\sum_{i=0}^pa^ic^{p-i},\qquad a=\rho_1,\ c=\rho_3,\ b=\rho_2,\ d=\rho_4.
$$

Grouping the states by odd and even population gives

$$
B=\sum_{p,q\geq0}\binom{p+q}{p}h_p(a,c)h_q(b,d).
$$

With $A=\max(a,c)$ and $E=\max(b,d)$, the bounds $A^p\leq h_p(a,c)\leq(p+1)A^p$ and $E^q\leq h_q(b,d)\leq(q+1)E^q$ show that convergence holds exactly when $A+E<1$. For necessity, the lower bound sums to $\sum_{k\geq0}(A+E)^k$, which diverges at or above one. For sufficiency, choose slightly larger $A',E'$ with $A'+E'<1$; the polynomial factors are absorbed into constants times $(A')^p(E')^q$, giving a convergent geometric generating series. Thus the [stability region for the reversible four-cycle flow network](../../../../../stability-region-for-the-reversible-four-cycle-flow-network.md) is

$$
\boxed{\max(\rho_1,\rho_3)+\max(\rho_2,\rho_4)<1.}
$$

Equivalently, the offered load on each resource, $\rho_1+\rho_4$, $\rho_1+\rho_2$, $\rho_2+\rho_3$, or $\rho_3+\rho_4$, is strictly below its unit capacity. For positive arrival rates this finite [normalizing constant](../../../../../normalizing-constant.md) gives the unique [stationary distribution](../../../../../stationary-distribution.md) of the [irreducible](../../../../../irreducible-representation.md) process. At or beyond the boundary, the displayed invariant weights are not summable and do not define a stationary probability law.

If an explicit [normalizing constant](../../../../../normalizing-constant.md) is desired, $h_p(a,c)=(a^{p+1}-c^{p+1})/(a-c)$ for $a\ne c$, and $\sum_{p,q}\binom{p+q}{p}u^pv^q=(1-u-v)^{-1}$. Hence for $a\ne c$, $b\ne d$ in the stable region,

$$
B=\frac1{(a-c)(b-d)}\left(\frac{ab}{1-a-b}-\frac{ad}{1-a-d}-\frac{cb}{1-c-b}+\frac{cd}{1-c-d}\right).
$$

Equal-parameter cases are obtained by continuity or directly from the positive series. In particular the empty-traffic limit is $B=1$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
