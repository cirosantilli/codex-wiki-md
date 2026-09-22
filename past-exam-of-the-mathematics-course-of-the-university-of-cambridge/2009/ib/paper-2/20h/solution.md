<h1 id="20h/solution">Solution</h1>

↑ **Parent:** [20H](../20h.md)

The modified [transition matrix](../../../../../stochastic-matrix.md) $\widetilde P$ describes the original [Markov chain](../../../../../markov-chain.md) until it hits $B$, and then keeps it at the first state hit. Each state of $B$ is therefore an [absorbing state](../../../../../absorbing-state.md), and

$$
(\widetilde P^{\,n}\mathbf1_B)_i=\mathbb P_i(\tau\le n).
$$

For a [nonnegative superharmonic function for a Markov chain](../../../../../nonnegative-superharmonic-function-for-a-markov-chain.md) $g$ satisfying the boundary condition, part (c) and positivity of the [transition matrix](../../../../../stochastic-matrix.md) give by induction $g\ge\widetilde P^{\,n}g$. Also $g\ge\mathbf1_B$. Consequently

$$
g_i\ge(\widetilde P^{\,n}g)_i\ge(\widetilde P^{\,n}\mathbf1_B)_i=\mathbb P_i(\tau\le n).
$$

Let $n\to\infty$ to obtain $g_i\ge h_i$. Since $h$ satisfies the conditions by parts (a),(b), **$h$ is their pointwise minimal solution**. This extends the [hitting probability is the minimal nonnegative harmonic extension](../../../../../hitting-probability-is-the-minimal-nonnegative-harmonic-extension.md) principle to the superharmonic inequality. Nonnegative sums justify the argument on a countable state space as well as a finite one.

Now suppose the [Markov chain](../../../../../markov-chain.md) is irreducible and recurrent, and let $g$ satisfy condition (a). In such a chain every state is hit almost surely from every other state. To see this directly, recurrence gives infinitely many visits to a starting state $i$. Irreducibility supplies a finite path from $i$ to any target $j$ with positive probability $\alpha$, chosen with no return to $i$ before reaching $j$. At each successive return to $i$, the [Strong Markov property](../../../../../strong-markov-property.md) gives another trial with conditional success probability at least $\alpha$. The chance of avoiding $j$ through $N$ such trials is at most $(1-\alpha)^N$, which tends to zero.

Apply the absorbing modification at the singleton $\{j\}$. Part (c) holds for arbitrary $g$ satisfying (a), so

$$
g_i\ge(\widetilde P^{\,n}g)_i\ge g_j\mathbb P_i(\tau_j\le n).
$$

Since $g_j\ge0$ and the probability tends to one, $g_i\ge g_j$. Interchanging $i,j$ yields equality. Thus **every nonnegative superharmonic function is constant** on an irreducible recurrent [Markov chain](../../../../../markov-chain.md).

Conversely, if an irreducible [Markov chain](../../../../../markov-chain.md) is not recurrent, choose a state $j$ with return probability $r_j=\mathbb P_j(\tau_j^+<\infty)<1$. Its [hitting probability](../../../../../hitting-probability.md) $h$ for $\{j\}$ satisfies condition (a), and $h_j=1$. The first-step formula for a return after time zero gives $(Ph)_j=r_j<1$. Therefore $h$ cannot be constant: a constant function with value one at $j$ would have $(Ph)_j=1$. This supplies a nonconstant nonnegative superharmonic solution. Hence

$$
\boxed{P\text{ is recurrent}\iff\text{every solution of (a) is constant}.}
$$

The admissible constant solutions are precisely the nonnegative constants. This is [recurrence characterized by constant nonnegative superharmonic functions](../../../../../recurrence-characterized-by-constant-nonnegative-superharmonic-functions.md).

## ↑ Ancestors (10)

1. [20H](../20h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
