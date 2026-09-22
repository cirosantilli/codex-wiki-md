<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

There is a useful explicit reconstruction of a shorter trace from a longer one. Suppose

$$
\rho_\beta(\alpha)=\langle S_0,\ldots,S_{n-1}\rangle,
\qquad S_i=C_{\beta_i^\alpha}\cap\alpha,
$$

and fix $\xi<\alpha$. Let $j<n$ be the first index with $S_j\setminus\xi\ne\varnothing$, if it exists. Before that index, the walk to $\xi$ follows the walk to $\alpha$. At index $j$ it moves to $\delta=\min(S_j\setminus\xi)<\alpha$. Thus

$$
\rho_\beta(\xi)
=\langle S_i\cap\xi:i\leq j\rangle\mathbin{{}^\frown}\rho_\delta(\xi).
$$

When $\delta=\xi$, the appended trace is empty. If no such $j$ exists, the walk first reaches $\alpha$ and then continues toward $\xi$, giving

$$
\rho_\beta(\xi)
=\langle S_i\cap\xi:i<n\rangle\mathbin{{}^\frown}\rho_\alpha(\xi).
$$

Both formulas depend only on the displayed sequence, $\alpha,\xi$, and the fixed [club sequence](../../../../../../../club-sequence.md). Equal traces $\rho_\beta(\alpha)=\rho_\gamma(\alpha)$ consequently reconstruct the same trace at every $\xi<\alpha$. This proves the [trace coherence lemma for minimal walks](../../../../../../../trace-coherence-lemma-for-minimal-walks.md):

$$
\boxed{\rho_\beta\upharpoonright\alpha=\rho_\gamma\upharpoonright\alpha.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 24](../../../../paper-24-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
