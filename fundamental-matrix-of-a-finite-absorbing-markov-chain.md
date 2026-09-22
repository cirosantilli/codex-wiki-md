# Fundamental matrix of a finite absorbing Markov chain

↑ **Parent:** [Absorbing state](absorbing-state.md)

For a [finite Markov chain](finite-markov-chain.md) in which an [absorbing state](absorbing-state.md) is accessible from every state, order the nonabsorbing states first and write

$$
P=\begin{pmatrix}Q&R\\0&I\end{pmatrix},\qquad
N=(I-Q)^{-1}=\sum_{n\geq0}Q^n.
$$

Here $I$ is the [identity matrix](identity-matrix.md) and $N$ is the [matrix inverse](matrix-inverse-split.md) of $I-Q$. With $T$ the first [hitting time](first-passage-time.md) of the absorbing set,

$$
N_{ij}=\mathbb E_i\sum_{n=0}^{T-1}\mathbf1_{\{X_n=j\}},\qquad
B=NR,\qquad t=N\mathbf1.
$$

Thus $N$ gives the [expected occupation count before absorption](expected-occupation-count-before-absorption.md), including the initial visit; $B_{ia}$ is the [absorption probability](splitting-probability.md) of state $a$; and $t_i$ is the [expected hitting time](expected-hitting-time.md) of the absorbing set. The [vector](vector.md) $\mathbf1$ has every entry one. See [Grinstead and Snell, section 11.2, theorems 11.4-11.6](https://math.dartmouth.edu/~prob/prob/prob.pdf#page=425).

For the toy routine in [absorbing state](absorbing-state.md), direct [matrix multiplication](matrix-multiplication.md) gives

$$
N=\begin{pmatrix}12/5&4/5\\4/5&8/5\end{pmatrix},\qquad
B=\begin{pmatrix}3/5&2/5\\1/5&4/5\end{pmatrix},\qquad
t=\begin{pmatrix}16/5\\12/5\end{pmatrix}.
$$

The first row of $N$ says that starting at $u$ gives $2.4$ visits to $u$ and $0.8$ to $v$ before termination. Their sum is the mean duration $3.2$. The identities $(I-Q)N=I$, $B=QB+R$, and $t=\mathbf1+Qt$ independently verify the inverse, outcome, and duration calculations. The absorbing set must be reachable from every state for these finite formulas: applying them to all nonabsorbing states in the closed-cycle example would leave a persistent cycle in $Q$ and make $I-Q$ singular.

## ↑ Ancestors (8)

1. [Absorbing state](absorbing-state.md)
2. [Markov chain](markov-chain-split.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Absorbing state](absorbing-state.md)
