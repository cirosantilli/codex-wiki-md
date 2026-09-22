<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $X$ be a coarse-grained configuration, with restricted partition function $Z_X$ and [free energy](../../../../../../thermodynamic-free-energy.md) $F(X)=-k_BT\log Z_X$. Its [Boltzmann distribution](../../../../../../boltzmann-distribution.md) is $\pi(X)\propto e^{-\beta F(X)}$. [Microscopic reversibility](../../../../../../microscopic-reversibility.md) pairs every equilibrium microscopic history with a history read backwards, including reversal of all time-odd variables. Summing this identity over the microscopic histories representing a given coarse-grained path preserves it; a Markov assumption is not needed for this argument.

Write $\mathbb P_F$ for the probability density of a specified history conditional on its starting configuration $X_1$, and $\mathbb P_B$ for its physically reversed history conditional on starting at $\Theta X_2$, where $\Theta$ reverses time-odd variables. Equilibrium [time-reversal symmetry](../../../../../../t-symmetry.md) gives

$$
\pi(X_1)\mathbb P_F=\pi(\Theta X_2)\mathbb P_B.
$$

Since $F(\Theta X)=F(X)$, the desired conditional path relation is

$$
\boxed{\frac{\mathbb P_F}{\mathbb P_B}=\frac{\pi(X_2)}{\pi(X_1)}=e^{-\beta(F_2-F_1)}.}
$$

For a reversible [Markov chain](../../../../../../markov-chain.md), this also follows by multiplying [detailed balance](../../../../../../detailed-balance.md) ratios $P_{ij}/P_{ji}=\pi_j/\pi_i$ along the history: the intermediate equilibrium weights telescope.

The conditioning is essential. If the starting equilibrium weights are included in the path probabilities, the forward and reversed probabilities are equal, rather than differing by the displayed exponential. For example, a two-state [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) with $F_1=0$, $F_2=\Delta>0$, rates $k_{12}=e^{-\beta\Delta}$ and $k_{21}=1$ has equal equilibrium-weighted probabilities for the two reversed single-jump histories. Their conditional rate ratio is instead $e^{-\beta\Delta}$. Normalized bridges conditioned on both endpoints also have a different normalization from the path weights used above. The PDF prints $\mathbb F_B$ in the denominator while its explanatory text defines $\mathbb P_B$; the latter is the intended notation. For the scalar [order parameter](../../../../../../order-parameter.md) used subsequently, $\Theta\phi=\phi$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
