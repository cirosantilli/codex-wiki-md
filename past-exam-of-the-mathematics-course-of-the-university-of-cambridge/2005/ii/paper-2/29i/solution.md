<h1 id="29i/solution">Solution</h1>

↑ **Parent:** [29I](../29i.md)

A time-homogeneous [Markov decision process](../../../../../markov-decision-process.md) specifies a state space, admissible actions at each state, an action-dependent [transition kernel](../../../../../markov-kernel.md) and one-step reward, with neither [kernel](../../../../../kernel-of-a-linear-map.md) nor reward depending on time. A policy chooses actions using the observed history. The positive programming case has nonnegative rewards and maximizes expected undiscounted total reward, allowing infinite values; its finite-horizon values increase to the infinite-horizon [supremum](../../../../../supremum.md) under the appropriate approximation argument.

Here let $\tau_B$ be the absorption time of the underlying [simple random walk](../../../../../simple-random-walk.md) at $0,N$. Every admissible [stopping time](../../../../../stopping-time.md) $T$ is at most $\tau_B$. The reward is bounded by $R_{\max}=\max_jr(j)$, and $E_i\tau_B=i(N-i)$, as follows by solving $h_i=1+(h_{i-1}+h_{i+1})/2$ with zero endpoint values. In particular absorption is almost surely finite. Truncating any policy at $T\wedge n$ changes its reward [expectation](../../../../../expected-value.md) by at most $2R_{\max}P_i(\tau_B>n)\leq2R_{\max}i(N-i)/n$. Since the truncated policy is allowed in the $n$-step problem,

$$
V_n(i)\leq V(i)\leq V_n(i)+2R_{\max}P_i(\tau_B>n).
$$

This proves **$V_n\to V$**, even uniformly on the finite state space.

The finite-horizon recursion starts with $V_0=r$, fixes the endpoint rewards and has

$$
V_{n+1}(i)=\max\{r(i),\tfrac12[V_n(i-1)+V_n(i+1)]\}.
$$

Taking limits shows $V\geq r$ and $2V(i)\geq V(i-1)+V(i+1)$, so $V$ is discretely concave. If $W$ is any [concave function](../../../../../concave-function.md) majorizing $r$, induction in this same recursion gives $V_n\leq W$, and hence $V\leq W$. Therefore **$V$ is the smallest [concave majorant](../../../../../concave-majorant.md) of the rewards**. At a point where $V(i)>r(i)$ the recursion forces equality with the neighboring average; the value graph is linear through each consecutive continuation region.

An optimal policy stops upon first entering the contact set $\{i:V(i)=r(i)\}$ and continues elsewhere. Before stopping the neighboring-average equality makes $V$ of the walk a bounded [martingale](../../../../../martingale-split.md); the [stopping time](../../../../../stopping-time.md) is bounded by $\tau_B$. Applying the bounded stopping identity by first truncating the time and then passing to the limit proves the expected terminal reward equals $V(i)$.

Distinct rewards do not guarantee uniqueness. With $N=2$ and $r(0)=0,r(1)=1,r(2)=2$, the reward function is already linear and $V=r$. From state one, stopping gives one, while continuing to the next step also gives expected reward $(0+2)/2=1$. Both policies are optimal. Thus **the claimed uniqueness is false** even when all rewards are distinct.

## ↑ Ancestors (10)

1. [29I](../29i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
