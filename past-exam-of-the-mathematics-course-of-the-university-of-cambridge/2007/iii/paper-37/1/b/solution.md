<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Scale the [SIRS Markov chain](../../../../../../sirs-markov-chain.md) by population size: $U_n=Z_n/n=(s_n,i_n,r_n)$. Suppose $U_n(0)\to u_0$ in probability, where $u_0$ is a deterministic point in the probability [standard simplex](../../../../../../standard-simplex.md). The required [fluid limit of the SIRS Markov chain](../../../../../../fluid-limit-of-the-sirs-markov-chain.md) is

$$
\boxed{\dot s=-\lambda si+\nu r,\qquad
\dot i=\lambda si-\gamma i,\qquad
\dot r=\gamma i-\nu r,\qquad u(0)=u_0.}
$$

We prove uniform convergence in probability on every fixed interval $[0,T]$, rather than merely replace random products by products of their [expectations](../../../../../../expected-value.md).

Introduce the jump vectors and scaled rate functions

$$
v_1=(-1,1,0),\quad v_2=(0,-1,1),\quad v_3=(1,0,-1),\qquad
\beta_1(u)=\lambda si,\quad\beta_2(u)=\gamma i,\quad\beta_3(u)=\nu r.
$$

At state $U_n=u$, an event of type $j$ has rate $n\beta_j(u)$ and jump $v_j/n$. Let $N_1,N_2,N_3$ be independent unit-rate [Poisson processes](../../../../../../poisson-process.md). The [Poisson time-change representation of a Markov chain](../../../../../../poisson-time-change-representation-of-a-markov-chain.md) gives

$$
U_n(t)=U_n(0)+\frac1n\sum_{j=1}^3v_jN_j\left(n\int_0^t\beta_j(U_n(a))\,da\right).
$$

This representation follows by giving each event type an independent exponential clock in its accumulated hazard. Conditional on the current state its firing rate is $n\beta_j$, hence it has exactly the transition rates from part (a). The finite state space and bounded rates rule out explosion. Values at the jump times do not affect the time integrals.

With $\widetilde N_j(v)=N_j(v)-v$, this becomes

$$
U_n(t)=U_n(0)+\int_0^tF(U_n(a))\,da+E_n(t),\qquad
F(u)=\sum_jv_j\beta_j(u),
$$

where

$$
E_n(t)=\frac1n\sum_jv_j\widetilde N_j\left(n\int_0^t\beta_j(U_n(a))\,da\right).
$$

The displayed $F$ is precisely the boxed drift. On the simplex, $\beta_j\le b_j$ with $b_1=\lambda$, $b_2=\gamma$, $b_3=\nu$. Thus every Poisson clock used before $T$ is at most $nb_jT$. For any fixed $\eta>0$, the permitted Poisson maximal bound, applied with time horizon $nb_jT$ and relative tolerance $\eta/(b_jT)$, gives

$$
\mathbb P\left(\frac1n\sup_{0\le v\le nb_jT}|\widetilde N_j(v)|\ge\eta\right)
\le2\exp\left[-nb_jT\,h\left(\frac\eta{b_jT}\right)\right]\longrightarrow0.
$$

A channel with $b_j=0$ contributes nothing and is simply omitted. Since $h(a)>0$ for $a>0$, these probabilities even decrease exponentially in $n$. Each $v_j$ has $\ell^1$ norm two. The [union bound](../../../../../../boole-s-inequality.md) consequently gives $\sup_{t\le T}\|E_n(t)\|_1\to0$ in probability. Notice that the clock is random, but its deterministic upper bound makes the Poisson maximal estimate directly applicable.

The drift $F$ is [Lipschitz](../../../../../../lipschitz-continuity.md) on the simplex. Indeed $|si-s'i'|\le|s-s'|+|i-i'|$ there, and one may take $L=2(\lambda+\gamma+\nu)$ for its $\ell^1$ [Lipschitz constant](../../../../../../lipschitz-constant.md). The [Picard-Lindelöf theorem](../../../../../../picard-lindelof-theorem.md) gives a unique local solution, which remains in the simplex: the sum of the derivatives is zero, while on the faces $s=0$, $i=0$, and $r=0$ the corresponding derivatives are respectively $\nu r$, $0$, and $\gamma i$, all nonnegative. More explicitly, $i(t)=i(0)\exp(\int_0^t(\lambda s(a)-\gamma)\,da)$ is nonnegative, and the linear equations for $r$ and $s$ have nonnegative forcing terms; their integrating-factor formulas keep both nonnegative. Conservation then bounds every coordinate by one, so the local solution extends globally.

Subtract its integral equation from that of $U_n$. The [Gronwall inequality](../../../../../../gronwall-inequality.md) yields

$$
\sup_{t\le T}\|U_n(t)-u(t)\|_1
\le e^{LT}\left(\|U_n(0)-u_0\|_1+\sup_{t\le T}\|E_n(t)\|_1\right)
\xrightarrow{\mathbb P}0.
$$

This proves the [Poisson concentration proof of a density-dependent fluid limit](../../../../../../poisson-concentration-proof-of-a-density-dependent-fluid-limit.md) for this model, including the initial-condition requirement and uniform finite-time approximation. In terms of population counts, the associated deterministic approximation is $\dot S=-\lambda SI/n+\nu R$, $\dot I=\lambda SI/n-\gamma I$, $\dot R=\gamma I-\nu R$. The limit concerns macroscopic initial proportions and fixed times; a single initial infective has limiting fraction zero, so early stochastic invasion on a growing time scale is not described by this finite-time limit alone.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
