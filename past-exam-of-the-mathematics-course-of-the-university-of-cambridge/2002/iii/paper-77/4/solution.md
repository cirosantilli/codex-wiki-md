<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Work deterministically with nonnegative arrivals. Write $S_x(t)=\sum_{k=1}^t x_{-k}$ for integer $t\geq1$, and $S_x(0)=0$. The relevant metric is

$$
d(x,y)=\|x-y\|
=\sup_{t\geq1}\frac{|S_x(t)-S_y(t)|}{t}.
$$

This is the [weighted cumulative-input topology for a slotted queue](../../../../../weighted-cumulative-input-topology-for-a-slotted-queue.md). It is a genuine [norm](../../../../../norm.md) on the ambient space of sequences with finite value: zero cumulative differences force every individual difference to vanish, since $x_{-k}=S_x(k)-S_x(k-1)$. Every input in the specified set $A$ has finite [norm](../../../../../norm.md), because its long prefixes are bounded by $\lambda t$ and there are only finitely many earlier prefixes.

Use the conventional net-input slot boundary [finite-buffer workload map](../../../../../finite-buffer-workload-map.md), whose recursion is the clipped [Lindley recursion](../../../../../lindley-recursion.md)

$$
q_{t+1}=F_B(q_t,x_t),\qquad
F_B(q,a)=\min\{B,\max(0,q+a-C)\}.
$$

Arriving work in a slot is available to that slot's service, and the observed queue state is after service and upper clipping. This fixes the slot convention explicitly. The queue size $Q_B(x)$ is obtained by starting in the distant past and taking the present workload. We first prove that, under the stated strict drift condition, this is uniquely defined independently of the initial state.

Fix $x\in A$ and write $d_0=C-\lambda>0$. Choose a finite integer $T$ so large that

$$
S_x(T)\leq\lambda T,\qquad T>\frac{2B}{d_0}.
$$

Then $S_x(T)-CT<-B$. Start at time $-T$ with a full buffer $q_{-T}=B$. The trajectory must hit zero by time zero. Otherwise lower clipping is never used, so for nonnegative lost-work amounts $\ell_t$ the total recursion would give

$$
q_0=B+S_x(T)-CT-\sum_{t=-T}^{-1}\ell_t
\leq B+S_x(T)-CT<0,
$$

contradicting nonnegativity. If zero is attained even at the last update the desired conclusion still holds.

The update $F_B$ is [monotone](../../../../../monotonic-function.md) in the initial workload. Couple all starting values in $[0,B]$ using the same arrivals. When the trajectory starting at $B$ reaches zero, all smaller trajectories must also be zero, and they remain identical thereafter. Thus the present queue depends only on the last $T$ slots, not on any earlier state or arrivals. This is [finite-memory continuity of a finite-buffer queue](../../../../../finite-memory-continuity-of-a-finite-buffer-queue.md). In particular it proves the existence and uniqueness of $Q_B(x)$ without assuming a random stationary law.

The same memory horizon works in a neighborhood of $x$. If $\delta=\|x-y\|<d_0/2$, then

$$
S_y(T)-CT
\leq S_x(T)+\delta T-CT
\leq-(d_0-\delta)T
<-\frac{d_0T}{2}<-B.
$$

The full-buffer trajectory for $y$ therefore also reaches zero within this horizon. Both $Q_B(x)$ and $Q_B(y)$ can consequently be calculated from initial workload zero at time $-T$, even though their respective reset times need not coincide.

Clipping to $[0,B]$ is [Lipschitz continuous](../../../../../lipschitz-continuity.md) with constant one, so

$$
|F_B(q,a)-F_B(\tilde q,\tilde a)|
\leq |q-\tilde q|+|a-\tilde a|.
$$

Iterating from the common initial value zero gives

$$
|Q_B(x)-Q_B(y)|\leq\sum_{k=1}^T|x_{-k}-y_{-k}|.
$$

The cumulative-input [norm](../../../../../norm.md) bounds each summand:

$$
|x_{-k}-y_{-k}|
\leq |S_x(k)-S_y(k)|+|S_x(k-1)-S_y(k-1)|
\leq(2k-1)\delta.
$$

Summing proves the explicit local estimate

$$
\boxed{|Q_B(x)-Q_B(y)|\leq T^2\|x-y\|,
\qquad\|x-y\|<\frac{C-\lambda}{2}.}
$$

Given $\varepsilon>0$, choose $\|x-y\|<\min\{(C-\lambda)/2,\varepsilon/T^2\}$. Then the workload difference is less than $\varepsilon$. Since $x\in A$ was arbitrary, **the queue size function is [continuous](../../../../../continuous-function.md) on $(A,\|\cdot\|)$**.

The argument also handles the alternative slot ordering that clips arrivals to the buffer before serving them: its update is a composition of monotone one-Lipschitz clipping and service maps, and negative total net input forces a reset. Measuring immediately after arrivals instead adds one finite-coordinate update, which is likewise [continuous](../../../../../continuous-function.md) in this [norm](../../../../../norm.md). The essential point is strict subcritical drift and loss of dependence on the remote past, rather than incorrectly replacing a finite-buffer history by the minimum of $B$ and an infinite-buffer workload.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
