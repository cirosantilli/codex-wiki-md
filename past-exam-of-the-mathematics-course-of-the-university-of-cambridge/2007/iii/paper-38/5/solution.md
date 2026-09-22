<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For the [graphical representation of the contact process](../../../../../graphical-representation-of-the-contact-process.md), put independent death marks on each vertical time-line $\{x\}\times[0,\infty)$ at rate $\delta$, and independent infection arrows $x\to y$ at rate $\lambda$ for every ordered nearest-neighbour pair. A time-directed path moves vertically upward, cannot pass a death mark, and may follow an infection arrow. From an initial set $A$, the infected set $\xi_t^A$ consists of sites reachable at time $t$ from $A\times\{0\}$. Thus infected sites recover at rate $\delta$, and a healthy site with $k$ infected neighbours becomes infected at rate $k\lambda$. Rates here are per ordered [edge](../../../../../edge-of-a-graph.md), fixing the normalization of $\lambda$.

With $\delta=1$, write

$$
\theta_d(\lambda)=\mathbb P_\lambda(\xi_t^{\{0\}}\ne\varnothing\text{ for every }t\geq0),\qquad
\lambda_c(d)=\inf\{\lambda:\theta_d(\lambda)>0\}.
$$

Couple two infection rates by adding independent arrows of rate $\lambda_2-\lambda_1$ to the rate-$\lambda_1$ construction, retaining the same deaths. Every path available at the lower rate remains available at the higher rate. Hence **$\theta_d(\lambda)$ is nondecreasing**.

For the lower bound, dominate the infection population by a linear birth-death [branching process](../../../../../branching-process.md) $Z_t$, started from one particle, with per-particle birth rate $2d\lambda$ and death rate $1$. Assign one branching particle to every infection; allow an offspring at every attempted transmission, including attempts into an already infected site, and let the extra particles continue independently. Matched deaths remove their infection. This constructs $|\xi_t|\leq Z_t$. The linear birth rate is nonexplosive, so in particular the [contact process](../../../../../contact-process.md) from a finite initial set is well-defined with finite population at finite times. Its branching mean solves

$$
\frac d{dt}\mathbb E Z_t=(2d\lambda-1)\mathbb E Z_t,\qquad
\mathbb E Z_t=e^{(2d\lambda-1)t}.
$$

Consequently

$$
\theta_d(\lambda)\leq\mathbb P(\xi_t\ne\varnothing)
\leq\mathbb E|\xi_t|\leq e^{(2d\lambda-1)t}.
$$

If $2d\lambda<1$, let $t\to\infty$ to obtain $\theta_d(\lambda)=0$. This proves the [branching bound for contact-process survival](../../../../../branching-bound-for-contact-process-survival.md)

$$
\boxed{\lambda_c(d)\geq\frac1{2d}}.
$$

For the upper bound use the [dimension comparison for the contact process](../../../../../dimension-comparison-for-the-contact-process.md). Define the height $h(x)=x_1+\cdots+x_d$. Construct an auxiliary infected set $\eta_t\subseteq\mathbb Z$ together with an infected representative $r_n(t)\in\xi_t$ of height $n$ for every $n\in\eta_t$. Initially $\eta_0=\{0\}$ and $r_0=0$. Use the original graphical marks as follows.

- A death at $r_n$ removes $n$ from $\eta$ as well as removing that representative from $\xi$. Other deaths change only $\xi$.
- From $r_n$ there are exactly $d$ arrows $r_n\to r_n+e_i$ into height $n+1$ and exactly $d$ arrows into height $n-1$. When one of these arrows occurs and the target height $m$ is absent from $\eta$, infect $m$ in the auxiliary process and use the arrow's target as its representative. That target belongs to $\xi$ after the arrow, whether it was newly infected or already infected.
- Arrows from other sites and arrows into an already occupied auxiliary height produce no auxiliary change.

This rule maintains a live representative for every auxiliary infection. Conditional on the full past, each active representative has death rate $1$ and outgoing-arrow rate $d\lambda$ in each of the two height directions. Representatives at distinct heights are different sites, using distinct death clocks and distinct outgoing ordered-[edge](../../../../../edge-of-a-graph.md) clocks. Independence and memorylessness of the underlying Poisson processes give exactly the one-dimensional contact-process generator

$$
(Lf)(\eta)=\sum_{n\in\eta}\bigl[f(\eta\setminus\{n\})-f(\eta)\bigr]
+d\lambda\sum_{n\in\eta}\sum_{\substack{m=n-1,n+1\\m\notin\eta}}
\bigl[f(\eta\cup\{m\})-f(\eta)\bigr].
$$

Thus $\eta$ has the law of the one-dimensional [contact process](../../../../../contact-process.md) with infection rate $d\lambda$, even though the representatives themselves depend on the higher-dimensional history. Since $\eta_t\ne\varnothing$ implies $\xi_t\ne\varnothing$ at every time,

$$
\theta_d(\lambda)\geq\theta_1(d\lambda).
$$

Every $\lambda$ for which $d\lambda>\lambda_c(1)$ is therefore supercritical whenever the one-dimensional survival set is nonempty; if that critical value were infinite the inequality would be trivial. Taking infima gives

$$
\boxed{\lambda_c(d)\leq\frac{\lambda_c(1)}d}.
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
