<h1 id="19c/solution">Solution</h1>

↑ **Parent:** [19C](../19c.md)

Put $h_0=1$ and $h_r=0$. The [Markov property](../../../../../markov-property.md) and first-step conditioning give $h_i=\sum_jP_{ij}h_j$. Consider a finite history ending at state $i$ and having positive conditional probability given $A$. The chance of eventual absorption at zero after that history is $h_i$: the future depends only on the present state, and if zero has already been reached, absorption keeps the chain there. If the next state is $j$, this chance is $h_j$. Bayes' rule therefore gives

$$
\mathbb P(X_{n+1}=j\mid X_0,\ldots,X_n=i,A)
=\frac{P_{ij}h_j}{h_i}.
$$

This depends on the history only through $i$, proving the conditional [Markov property](../../../../../markov-property.md). **The conditional [transition matrix](../../../../../stochastic-matrix.md) is**

$$
\boxed{Q_{ij}=P_{ij}\frac{h_j}{h_i}\quad(0\leq i<r).}
$$

Its row sums are one by harmonicity of $h$, and $Q_{ir}=0$. State $r$ is never visited under the conditioning and is naturally removed; any row assigned there on an enlarged formal state space is immaterial, since conditioning starting at $r$ is undefined. State zero stays absorbing. For a random initial law $\nu$, its conditional law is $\nu_i h_i/\sum_j\nu_jh_j$. This is the [Doob h-transform](../../../../../doob-h-transform.md) with the absorption probability as harmonic function.

For the simple symmetric walk, $h_i=(r-i)/r$ solves the linear harmonic recurrence and its boundary values. Thus

$$
Q_{i,i-1}=\frac{r-i+1}{2(r-i)},\qquad
Q_{i,i+1}=\frac{r-i-1}{2(r-i)},\qquad 1\leq i<r.
$$

In particular, the conditioned chain moves downward with probability one from $r-1$.

Let $\tau$ be the first hit of $\{0,r\}$ in the original walk and let $g_i=\mathbb E_i[\tau\mathbf1_A]$. Its absorption time has finite expectation: from any transient state a run of at most $r$ downward steps hits zero with probability at least $2^{-r}$, giving a geometric tail bound by blocks. First-step conditioning then gives

$$
g_0=g_r=0,\qquad g_i=h_i+\frac12(g_{i-1}+g_{i+1}).
$$

Equivalently, $g_{i+1}-2g_i+g_{i-1}=-2(r-i)/r$. The cubic [polynomial](../../../../../polynomial-split.md)

$$
g_i=\frac{i(r-i)(2r-i)}{3r}
$$

has exactly these second differences and boundary values. It is the unique solution, since the difference of any two solutions is a linear sequence vanishing at both endpoints. Conditional on $A$, $\tau$ is the first time in zero, so division by $h_i$ proves

$$
\boxed{\mathbb E_i[\tau_0\mid A]=\frac{g_i}{h_i}=\frac{i(2r-i)}3.}
$$

This is the [duration of gambler's ruin conditioned on a chosen boundary](../../../../../duration-of-gambler-s-ruin-conditioned-on-a-chosen-boundary.md).

## ↑ Ancestors (10)

1. [19C](../19c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
