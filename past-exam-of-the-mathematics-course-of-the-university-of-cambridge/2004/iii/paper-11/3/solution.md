<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Expose the independent coordinates in order and let $M_i=\mathbb E[f\mid X_1,\ldots,X_i]$, $M_0=\mathbb Ef$. This is the [Doob exposure martingale](../../../../../doob-exposure-martingale.md). For fixed earlier coordinates, write $h_i(x)=\mathbb E[f\mid X_i=x,\text{earlier coordinates}]$. The remaining coordinates have the same distribution for all $x$, and the coordinate-change hypothesis gives $|h_i(x)-h_i(y)|\leq c_i$. Thus the conditional range of $M_i-M_{i-1}$ has length at most $c_i$, and its conditional mean is zero.

Here is the [Hoeffding lemma](../../../../../hoeffding-lemma.md) needed for the sharp constant. If a mean-zero [random variable](../../../../../random-variable-split.md) $Y$ lies in an interval of length $c$, [set](../../../../../set-split.md) $\psi(s)=\log\mathbb Ee^{sY}$. Its second derivative is the [variance](../../../../../variance-split.md) under the exponentially tilted law. Under any such law, [variance](../../../../../variance-split.md) is at most $c^2/4$, by comparison with squared distance from the interval midpoint. Since $\psi(0)=\psi'(0)=0$, integration gives $\psi(s)\leq s^2c^2/8$ for all real $s$. Applying this conditionally and iterating the tower property yields

$$
\mathbb Ee^{s(f-\mathbb Ef)}\leq
\exp\left(\frac{s^2}{8}\sum_i c_i^2\right).
$$

The [exponential Markov bound](../../../../../exponential-markov-bound.md) now gives

$$
\Pr(f-\mathbb Ef\geq t)
\leq\exp\left(-st+\frac{s^2C}{8}\right),
\qquad C=\sum_i c_i^2.
$$

For $C>0$ choose $s=4t/C$. Apply the same argument to $-f$ and add the two tails, proving the [McDiarmid inequality](../../../../../mcdiarmid-s-inequality.md)

$$
\boxed{\Pr(|f-\mathbb Ef|\geq t)\leq2e^{-2t^2/C}.}
$$

For $C=0$, $f$ is constant almost surely, and every positive-deviation [probability](../../../../../probability.md) is zero.

For the neighbourhood application, the ambient points must be elements of $\mathcal P[n]$, equivalently binary strings; the printed $y\in[n]$ is a type error. An $n$-element ambient [set](../../../../../set-split.md) could not generally satisfy the stated exponential-size lower bound. Use the uniform [product probability space](../../../../../product-probability-space.md) on the [Boolean cube](../../../../../boolean-hypercube.md) and [set](../../../../../set-split.md) $F(y)=d(y,A)$. Flipping one coordinate changes this [Hamming distance](../../../../../hamming-distance.md) by at most one, so $C=n$. Put $\mu=\mathbb EF$. Since $\Pr(F=0)=|A|/2^n\geq\varepsilon$, the proved two-sided inequality gives, for $\mu>0$,

$$
\varepsilon\leq\Pr(|F-\mu|\geq\mu)
\leq2e^{-2\mu^2/n}.
$$

Consequently $\mu\leq\sqrt{(n/2)\log(2/\varepsilon)}=t/2$; the same bound is immediate if $\mu=0$. Therefore

$$
\Pr(F>t)\leq\Pr(|F-\mu|\geq t-\mu)
\leq2e^{-2(t-\mu)^2/n}\leq2e^{-t^2/(2n)}=\varepsilon.
$$

This proves the [Boolean cube expansion from bounded differences](../../../../../boolean-cube-expansion-from-bounded-differences.md):

$$
\boxed{|A_t|\geq(1-\varepsilon)2^n.}
$$

The meaningful range is $0<\varepsilon\leq1$; real radii are interpreted by the inequality on the integer-valued [Hamming distance](../../../../../hamming-distance.md). The converted TeX's final $2^{2n}$ is another corruption: the original PDF has $2^n$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
