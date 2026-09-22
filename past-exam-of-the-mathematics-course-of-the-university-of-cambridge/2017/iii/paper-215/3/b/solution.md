<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a finite [irreducible Markov chain](../../../../../../irreducible-markov-chain.md) satisfying [detailed balance](../../../../../../detailed-balance.md), define the directed-edge capacity $Q(u,v)=\pi(u)P(u,v)$. For every ordered pair $(x,y)$ choose a [path](../../../../../../continuous-path.md) $\eta_{xy}$ from $x$ to $y$ using only positive-capacity [edges](../../../../../../edge-of-a-graph.md); take the empty [path](../../../../../../continuous-path.md) for $x=y$. Let $N_e(\eta)$ count occurrences of the directed [edge](../../../../../../edge-of-a-graph.md) $e$. The [canonical paths Poincare bound](../../../../../../canonical-paths-poincare-bound.md) says that

$$
\rho=\max_{e:Q(e)>0}\frac{1}{Q(e)}\sum_{x,y}\pi(x)\pi(y)|\eta_{xy}|N_e(\eta_{xy})
$$

is a valid [Poincare inequality for a reversible Markov chain](../../../../../../poincare-inequality-for-a-reversible-markov-chain.md) constant. Simple [paths](../../../../../../continuous-path.md) give $N_e\in\{0,1\}$; allowing repetitions requires the multiplicities shown.

To prove the theorem, expand the [variance](../../../../../../variance-split.md) using two independent samples from $\pi$:

$$
\operatorname{Var}_\pi(f)=\frac12\sum_{x,y}\pi(x)\pi(y)(f(x)-f(y))^2.
$$

Telescoping along $\eta_{xy}$ and applying the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
(f(x)-f(y))^2\leq|\eta_{xy}|\sum_eN_e(\eta_{xy})(f(e^-)-f(e^+))^2.
$$

Interchange the finite sums, then use the definition of $\rho$:

$$
\begin{aligned}
\operatorname{Var}_\pi(f)&\leq\frac12\sum_e(f(e^-)-f(e^+))^2\sum_{x,y}\pi(x)\pi(y)|\eta_{xy}|N_e(\eta_{xy})\\
&\leq\frac\rho2\sum_eQ(e)(f(e^-)-f(e^+))^2=\rho\mathcal E(f,f).
\end{aligned}
$$

Consequently $\boxed{\operatorname{Var}_\pi(f)\leq\rho\mathcal E(f,f),\quad\gamma\geq1/\rho}$. All [edges](../../../../../../edge-of-a-graph.md) here are directed, so the $1/2$ in the [Dirichlet form of a Markov chain](../../../../../../dirichlet-form-of-a-markov-chain.md) is retained consistently.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
