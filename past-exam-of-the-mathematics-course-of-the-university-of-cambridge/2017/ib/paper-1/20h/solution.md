<h1 id="20h/solution">Solution</h1>

↑ **Parent:** [20H](../20h.md)

Assume the intended initial fortune satisfies $n\ge2$ and put $X_0=n$. Conditional on current fortune $i>1$, the next gift is uniform on $\{1,\ldots,i-1\}$ and independent of the previous choices. The remaining fortune is therefore uniform on that same set. At fortune $1$ the process stays there. Consequently the future conditional distribution depends only on the current fortune, proving the [Markov property](../../../../../markov-property.md), and the [transition matrix](../../../../../stochastic-matrix.md) on $\{1,\ldots,n\}$ is

$$
\boxed{P_{ij}=\begin{cases}1,&i=j=1,\\1/(i-1),&i>1,\ 1\le j<i,\\0,&\text{otherwise}.\end{cases}}
$$

The [uniform decreasing Markov chain](../../../../../uniform-decreasing-markov-chain.md) has state $1$ as an [absorbing state](../../../../../absorbing-state.md), and until absorption the fortune strictly decreases, so the [hitting time](../../../../../first-passage-time.md) is at most $n-1$.

Let $e_i$ be the expected number of additional transitions to hit $1$, taking $e_1=0$. [First-step analysis](../../../../../first-step-analysis.md) gives

$$
e_i=1+\frac1{i-1}\sum_{j=1}^{i-1}e_j\quad(i\ge2).
$$

In particular $e_2=1$. For $i\ge3$, multiplying this recurrence by $i-1$ and the recurrence for $i-1$ by $i-2$, then subtracting, gives $(i-1)e_i=(i-1)e_{i-1}+1$. Hence $e_i-e_{i-1}=1/(i-1)$ for every $i\ge2$, and telescoping yields

$$
\boxed{\mathbb E_n\tau=e_n=\sum_{j=1}^{n-1}\frac1j=H_{n-1}}.
$$

The PDF defines $\tau$ using times $i\ge1$. If $n=1$ were included, that definition would give $\tau=1$ although the displayed empty sum is zero; the initial instruction to choose an integer between $1$ and $n-1$ also requires $n\ge2$. The result above uses that intended assumption. A hitting time allowing time zero would have expectation zero from state $1$, but that is a different definition.

## ↑ Ancestors (10)

1. [20H](../20h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
