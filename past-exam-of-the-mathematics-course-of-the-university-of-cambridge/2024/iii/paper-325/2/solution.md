<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the [spin singlet state](../../../../../spin-singlet-state.md), measurements along the same axis are perfectly anticorrelated. By measuring either spin component of particle $B$, one can therefore predict with certainty the corresponding result for distant particle $A$. The [Einstein–Podolsky–Rosen criterion of reality](../../../../../einstein-podolsky-rosen-criterion-of-reality.md) then says that every such spin component of $A$ is an element of physical reality, because the choice at $B$ can be made without disturbing $A$. Since the quantum state assigns no simultaneous sharp values to noncommuting spin components, the EPR argument concludes that the wavefunction is not a complete description, provided this locality premise is accepted.

Let $\lambda$ denote a proposed complete hidden state, and let $a,b$ be the chosen axes.

- [Outcome determinism](../../../../../outcome-determinism.md) says that, given $\lambda$ and the settings, each outcome is fixed rather than merely probabilistic: $A,B\in\{-1,1\}$ are definite response functions.
- [Parameter independence](../../../../../parameter-independence.md) says that the conditional distribution of one local outcome is independent of the distant setting. Together with outcome determinism, it gives $A=A(a,\lambda)$ and $B=B(b,\lambda)$.
- [Measurement independence](../../../../../measurement-independence.md) says that the preparation variable is statistically independent of the later settings: $\rho(\lambda|a,b)=\rho(\lambda)$.

For two axes on each side, every $\lambda$ obeys

$$
\begin{aligned}
S(\lambda)
&=A(a_0,\lambda)[B(b_0,\lambda)+B(b_1,\lambda)]\\
&\quad+A(a_1,\lambda)[B(b_0,\lambda)-B(b_1,\lambda)]
\in\{-2,2\}.
\end{aligned}
$$

[Measurement independence](../../../../../measurement-independence.md) permits averaging the same distribution of $\lambda$ for all four setting pairs, producing the [CHSH inequality](../../../../../chsh-inequality.md)

$$
|E_{00}+E_{01}+E_{10}-E_{11}|\leq2.
$$

The singlet prediction is

$$
E(a,b)=-\mathbf a\mathbin\cdot\mathbf b.
$$

Choose coplanar unit vectors

$$
\mathbf a_0=\mathbf z,
\qquad
\mathbf a_1=\mathbf x,
\qquad
\mathbf b_0=\frac{\mathbf z+\mathbf x}{\sqrt2},
\qquad
\mathbf b_1=\frac{\mathbf z-\mathbf x}{\sqrt2}.
$$

Then

$$
E_{00}=E_{01}=E_{10}=-\frac1{\sqrt2},
\qquad
E_{11}=\frac1{\sqrt2},
$$

and therefore

$$
\boxed{|E_{00}+E_{01}+E_{10}-E_{11}|=2\sqrt2>2}.
$$

Thus the predictions of quantum theory violate the conjunction of outcome determinism, parameter independence, and measurement independence. This is [Bell theorem](../../../../../bell-theorem.md); the calculation alone does not select which premise a deeper theory must abandon.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 325](../../paper-325-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
