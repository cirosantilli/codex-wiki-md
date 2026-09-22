<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Track on the lifted integer line the coordinate refreshed at each step. It is a random walk $R_t$ with right-step probability $2/3$ and left-step probability $1/3$. Every visited residue modulo $n$ has had its bit replaced by an independent fair bit. Consequently the first time all residues have been visited is a [strong stationary time](../../../../../../strong-stationary-time.md) for this [shift-refresh chain on a hypercube](../../../../../../shift-refresh-chain-on-a-hypercube.md).

For the upper bound, reaching level $n$ visits every residue, so the refresh time is at most $\tau_n$. The supplied moments give

$$
\mathbb E\tau_n=3n,\qquad
\operatorname{Var}(\tau_n)=24n.
$$

For any sequence $w_n$ with $w_n/\sqrt n\to\infty$, [Chebyshev inequality](../../../../../../chebyshev-inequality.md) and the strong-stationary-time bound imply

$$
d_{\mathrm{TV}}(3n+w_n)
\leq\mathbb P(\tau_n>3n+w_n)\longrightarrow0.
$$

For the lower bound, choose integers $b_n$ such that

$$
\sqrt n\ll b_n\ll w_n,\qquad b_n=o(n),
$$

and consider $\tau_{n-2b_n}\wedge\tau_{-b_n}$. Its supplied mean is $3n-6b_n+o(1)$ and its variance is $O(n)$; after replacing $w_n$ by a sequence with $\sqrt n\ll w_n\ll n$, take for example $b_n=\lfloor\sqrt{w_n\sqrt n}\rfloor$. This satisfies the displayed scale separation, and the supplied moment bounds show

$$
\mathbb P\{\tau_{n-2b_n}\wedge\tau_{-b_n}\leq3n-w_n\}\longrightarrow0.
$$

Before that exit, the visited interval has length less than $n-b_n$, so at least $b_n$ coordinates retain their initial values.

Start the chain from the all-zero vector. Conditional on the explored path, the number of one-bits is binomial with at most $n-b_n$ trials, whereas under stationarity it is $\operatorname{Bin}(n,1/2)$. Since $b_n/\sqrt n\to\infty$, standard binomial concentration separates these two laws; for instance the event

$$
\left\{\text{number of ones}\leq\frac n2-\frac{b_n}{4}\right\}
$$

has probability tending to one for the chain and to zero under $\pi$. Therefore

$$
d_{\mathrm{TV}}(3n-w_n)\longrightarrow1.
$$

The transition from one to zero occurs in an $o(n)$ window around $3n$, proving total-variation cutoff with cutoff time $3n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
