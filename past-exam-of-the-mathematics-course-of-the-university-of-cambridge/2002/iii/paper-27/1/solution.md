<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the exponent convention $\mathbb E e^{iuX_t}=e^{t\psi(u)}$. A real [Lévy process](../../../../../levy-process.md) starts at $0$, has [stationary increments](../../../../../stationary-increments.md) and [independent increments](../../../../../independent-increments.md), is [stochastically continuous](../../../../../stochastic-continuity.md), and is taken in its [càdlàg](../../../../../cadlag.md) version. Its [characteristic exponent of a Lévy process](../../../../../characteristic-exponent-of-a-levy-process.md) satisfies $\psi(0)=0$ and is continuous. This convention has the opposite sign from the alternative $e^{-t\Psi(u)}$, so $\psi=-\Psi$.

For real $u$, the [exponential martingale of a Lévy process](../../../../../exponential-martingale-of-a-levy-process.md) is integrable because $|M_t^u|=e^{-t\operatorname{Re}\psi(u)}$ is deterministic and finite. For $s\le t$, its [conditional expectation](../../../../../conditional-expectation.md) with respect to the natural [filtration](../../../../../filtration-probability-theory.md) is

$$
\mathbb E[M_t^u\mid\mathcal F_s]
=e^{iuX_s-t\psi(u)}\mathbb E e^{iu(X_t-X_s)}
=e^{iuX_s-t\psi(u)}e^{(t-s)\psi(u)}=M_s^u.
$$

The second equality uses both [independent increments](../../../../../independent-increments.md) and [stationary increments](../../../../../stationary-increments.md). Thus this is a complex [martingale](../../../../../martingale-split.md), meaning that its real and imaginary parts are [martingales](../../../../../martingale-split.md).

A [probability distribution](../../../../../probability-distribution.md) is an [infinitely divisible distribution](../../../../../infinite-divisibility-probability.md) when, for every positive integer $n$, it is the distribution of a sum of $n$ [independent and identically distributed](../../../../../independent-and-identically-distributed-random-variables.md) [random variables](../../../../../random-variable-split.md). Their common distribution is allowed to depend on $n$. For a [Lévy process](../../../../../levy-process.md),

$$
X_1=\sum_{j=1}^n\bigl(X_{j/n}-X_{(j-1)/n}\bigr),
$$

and these summands are [independent](../../../../../independent-random-variables.md) with the common law of $X_{1/n}$. This proves the required [infinite divisibility](../../../../../infinite-divisibility-probability.md) directly.

The [Lévy–Khintchine theorem](../../../../../levy-khintchine-formula.md) states that a real [infinitely divisible distribution](../../../../../infinite-divisibility-probability.md) has [characteristic function](../../../../../characteristic-function.md) $e^{\psi(u)}$, where, for a unique triplet with the following fixed truncation,

$$
\boxed{\psi(u)=ibu-\frac a2u^2+\int_{\mathbb R\setminus\{0\}}
\bigl(e^{iuy}-1-iuy\mathbf1_{\{|y|<1\}}\bigr)K(dy),}
$$

with $b\in\mathbb R$, $a\ge0$, $K$ a positive measure, $K(\{0\})=0$, and $\int(1\wedge y^2)K(dy)<\infty$. Conversely every such triplet gives an [infinitely divisible distribution](../../../../../infinite-divisibility-probability.md) and a [Lévy process](../../../../../levy-process.md), unique in law, whose time-$t$ [characteristic function](../../../../../characteristic-function.md) is $e^{t\psi(u)}$. The [Lévy measure](../../../../../levy-measure.md) $K$ need not be finite near zero. [Taylor expansion](../../../../../taylor-expansion.md) makes the compensated integrand $O(y^2)$ there, while the measure is finite away from zero, so the integral is well defined. The drift parameter depends on the truncation: using $|y|\le1$ instead can alter $b$ by the contribution of atoms at $\pm1$. Here $a$ denotes [Gaussian](../../../../../normal-distribution.md) [variance](../../../../../variance-split.md), not drift.

We now prove that continuity forces $K=0$, using the suggested truncation rather than merely quoting a path classification. For $\varepsilon>0$, $\lambda_\varepsilon=K(|y|\ge\varepsilon)$ is finite. The truncated exponent is that of the [Compound Poisson process](../../../../../compound-poisson-process.md)

$$
Y_t^\varepsilon=\sum_{j=1}^{N_t}J_j-t\int_{\varepsilon\le|y|<1}yK(dy),
$$

where $N$ has rate $\lambda_\varepsilon$ and the marks have law $K(dy)\mathbf1_{\{|y|\ge\varepsilon\}}/\lambda_\varepsilon$ when the rate is positive. The remaining exponent $\psi-\psi_\varepsilon$ also has an admissible [Lévy–Khintchine formula](../../../../../levy-khintchine-formula.md) triplet. Hence construct independently a [Lévy process](../../../../../levy-process.md) $Z^\varepsilon$ with that exponent. The sum $Y^\varepsilon+Z^\varepsilon$ has the same [finite-dimensional distributions](../../../../../finite-dimensional-distribution.md) as $X$, and hence the same law on [càdlàg](../../../../../cadlag.md) path space. Continuity is therefore an almost-sure property of the sum if it is one of $X$.

But [independent compound Poisson jumps cannot cancel](../../../../../independent-compound-poisson-jumps-cannot-cancel.md): conditional on the path of $Z^\varepsilon$, its jump times are [countable](../../../../../countable-set.md); the [independent](../../../../../independent-random-variables.md) Poisson jump times have continuous distributions and avoid them almost surely. At each jump of $Y^\varepsilon$, the sum has the same nonzero jump, of size at least $\varepsilon$. If $\lambda_\varepsilon>0$, there is positive probability of such a jump on any fixed positive-length time interval, contradicting almost-sure continuity. Thus $K(|y|\ge\varepsilon)=0$ for every $\varepsilon>0$, and taking $\varepsilon=1/n$ gives $K=0$.

The [characteristic function](../../../../../characteristic-function.md) is now $\exp[t(ibu-au^2/2)]$. If $a>0$, the process $B_t=(X_t-bt)/\sqrt a$ has continuous paths and [independent](../../../../../independent-random-variables.md) centered [normal](../../../../../normal-distribution.md) increments of [variance](../../../../../variance-split.md) $t-s$, so it is standard [Brownian motion](../../../../../brownian-motion-split.md) on the original probability space. If $a=0$, the increments are deterministic, and continuity together with equality at all rational times gives $X_t=bt$ simultaneously for all $t$ almost surely. A [Brownian motion](../../../../../brownian-motion-split.md) on an enlarged space can be used in the zero-variance representation if necessary. Therefore

$$
\boxed{X_t=bt+\sqrt a\,B_t,\qquad a\ge0.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
