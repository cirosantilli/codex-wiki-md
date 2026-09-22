<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The printed hitting-time formula is false for the stated transition probabilities.** For example, take $N=2$ and $q=3/4$, put $p=1-q$, and write $m_i=\mathbb E_iT$. A first step gives

$$
m_1=1+pm_2,\qquad m_2=1+m_1,
$$

so $m_2=2/q=8/3$. The printed expression gives $3$, not $8/3$. This discrepancy is present in the original PDF, not just in its converted text. The quantifier mentioning every positive integer must also be restricted to positive starting states $1,\ldots,N$; states larger than $N$ are not in $S$.

Here is the exact solution for the chain as specified. Until $T$, only $\{1,\ldots,N\}$ is visited. From any such state, a sequence of downward steps reaches zero within $N$ steps with probability at least $q^N>0$; the forced step at $N$ only increases that probability. The [Markov property](../../../../../../markov-property.md) therefore gives

$$
\mathbb P_i(T>kN)\leq(1-q^N)^k.
$$

Thus $T$ is finite [almost surely](../../../../../../almost-sure-convergence.md) and has finite [expectation](../../../../../../expected-value.md), without needing the supplied transience assumption. Set $m_0=0$. The [first-step analysis](../../../../../../first-step-analysis.md) gives

$$
m_i=1+qm_{i-1}+pm_{i+1}\quad(1\leq i<N),\qquad m_N=1+m_{N-1}.
$$

Put $d=q-p=2q-1>0$, $r=p/q$, and $D_i=m_i-m_{i-1}$. The equations become

$$
qD_i-pD_{i+1}=1,\qquad D_N=1.
$$

Backward iteration, or substitution into this recursion, gives

$$
D_i=\frac1d-\frac{2p}{d}r^{N-i}.
$$

Summing from $1$ to $i$ gives the corrected [hitting time of a downward-biased walk reflected at an upper barrier](../../../../../../hitting-time-of-a-downward-biased-walk-reflected-at-an-upper-barrier.md):

$$
\boxed{m_i=\frac{i}{d}-\frac{2pq}{d^2}r^{N-i}(1-r^i),\quad 0\leq i\leq N,}
$$

and in particular

$$
\boxed{\mathbb E_NT=\frac N{2q-1}
-\frac{2q(1-q)}{(2q-1)^2}\left[1-\left(\frac{1-q}{q}\right)^N\right].}
$$

These values also supply the appropriate test function for part (b): $f(i)=m_i$, $f(0)=0$, and $Pf=f-1$ at every state before absorption. The finite-state stopped argument is applied on $\{0,\ldots,N\}$, with zero made absorbing.

For $N\geq3$, the printed hint cannot produce constant drift by choosing its single constant $c$. With $f(i)=i$ for $i<N$ and $f(N)=N+c$, the expected downward drift is $d$ at ordinary interior states, $d-pc$ at $N-1$, and $1+c$ at $N$. Making the top drift $d$ requires $c=-2p$, but then the drift at $N-1$ is $d+2p^2$, not $d$. For $N=2$ there is no ordinary interior state; a different constant drift can be arranged, but still gives $2/q$ rather than the printed formula. This identifies precisely the missing correction at the neighboring state for the intended drift $d$; the geometric term in the correct test function repairs it throughout the interval.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
