<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the intrinsic definition of a [Lévy process](../../../../../../levy-process.md): $X_0=0$ [almost surely](../../../../../../almost-sure-convergence.md), its increments over disjoint time intervals are independent, their [probability distributions](../../../../../../probability-distribution.md) depend only on interval length, and $X$ has [stochastic continuity](../../../../../../stochastic-continuity.md). In symbols,

$$
X_{s+t}-X_s\overset d=X_t,\qquad X_{t+h}\longrightarrow X_t\text{ in probability as }h\to0
$$

with times restricted to the half-line. Such a [stochastic process](../../../../../../stochastic-process-split.md) has a [càdlàg modification](../../../../../../cadlag-modification.md), and is usually represented by that version. Requiring [càdlàg](../../../../../../cadlag.md) paths in the definition is a common equivalent convention at the level of modifications; it is important to distinguish this from a claim about the paths of an arbitrary supplied version.

For the [characteristic function](../../../../../../characteristic-function.md), write

$$
\boxed{\mathbb E e^{i\theta X_t}=e^{t\psi(\theta)}=e^{-t\Psi(\theta)},\qquad\Psi=-\psi.}
$$

Here $\psi(0)=0$ and $\psi$ is the positive-time-sign [characteristic exponent of a Lévy process](../../../../../../characteristic-exponent-of-a-levy-process.md). The [independent increments](../../../../../../independent-increments.md) and [stationary increments](../../../../../../stationary-increments.md) give $\phi_{s+t}(\theta)=\phi_s(\theta)\phi_t(\theta)$; [stochastic continuity](../../../../../../stochastic-continuity.md) gives continuity in time and $\phi_0=1$. This continuous multiplicative [semigroup](../../../../../../semigroup.md) has the stated exponential form. Its exponent has the [Lévy–Khintchine formula](../../../../../../levy-khintchine-formula.md)

$$
\psi(\theta)=ib\theta-\frac{\sigma^2\theta^2}{2}+\int_{\mathbb R\setminus\{0\}}\left(e^{i\theta y}-1-i\theta y\mathbf1_{\{|y|\leq1\}}\right)\nu(dy),
$$

where $b\in\mathbb R$, $\sigma^2\geq0$, and the [Lévy measure](../../../../../../levy-measure.md) $\nu$ satisfies $\int(1\wedge y^2)\nu(dy)<\infty$. The truncation convention fixes the [drift coefficient](../../../../../../drift-coefficient.md) $b$; the displayed sign convention agrees with $\Psi=-\psi$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
