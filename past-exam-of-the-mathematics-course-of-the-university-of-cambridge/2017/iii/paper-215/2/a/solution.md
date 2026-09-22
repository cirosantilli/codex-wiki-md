<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a finite [irreducible Markov chain](../../../../../../irreducible-markov-chain.md) that is an [aperiodic Markov chain](../../../../../../aperiodic-markov-chain.md), set

$$
d_n(t)=\max_x\|P_n^t(x,\cdot)-\pi_n\|_{\mathrm{TV}},\qquad
\boxed{t_{\mathrm{mix}}^{(n)}(\alpha)=\min\{t\in\mathbb Z_{\geq0}:d_n(t)\leq\alpha\}.}
$$

Here $\pi_n$ is its unique [stationary distribution](../../../../../../stationary-distribution.md), and the distance is [total variation distance](../../../../../../total-variation-distance.md). Applying a [Markov kernel](../../../../../../markov-kernel.md) contracts [total variation distance](../../../../../../total-variation-distance.md), so $d_n(t)$ is nonincreasing and the minimum is finite.

Use the [ratio definition of cutoff](../../../../../../ratio-definition-of-cutoff.md): a family has [cutoff for Markov chains](../../../../../../cutoff-for-markov-chains.md) if, for every fixed $0<\varepsilon<1/2$,

$$
\boxed{\frac{t_{\mathrm{mix}}^{(n)}(\varepsilon)}{t_{\mathrm{mix}}^{(n)}(1-\varepsilon)}\longrightarrow1,}
$$

with the denominator positive eventually. Thus the transition between any two fixed distance levels takes negligible time compared with the [mixing time](../../../../../../mixing-time-of-a-markov-chain.md) scale. By monotonicity and squeezing, this also gives $t_{\mathrm{mix}}^{(n)}(\alpha)/t_{\mathrm{mix}}^{(n)}(\beta)\to1$ for any fixed $\alpha,\beta\in(0,1)$.

Some definitions of [cutoff for Markov chains](../../../../../../cutoff-for-markov-chains.md) additionally require the [mixing time](../../../../../../mixing-time-of-a-markov-chain.md) to diverge. That extra requirement cannot be built into the definition here: the final request in part (d) explicitly asks for a bounded-time counterexample. The ratio convention is the one consistent with that request.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
