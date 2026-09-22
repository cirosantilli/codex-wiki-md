<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $R_t=|W_t|$. First verify that the origin is not reached, so that differentiating the radius is legitimate. On $\mathbb R^3\setminus\{0\}$ the function $F(w)=|w|^{-1}$ is harmonic. For $T_\varepsilon=\inf\{t:R_t=\varepsilon\}$ with $0<\varepsilon<1$, the [Itô formula](../../../../../../ito-s-lemma.md) makes $F(W_{t\wedge T_\varepsilon})$ a [martingale](../../../../../../martingale-split.md) on each finite horizon: its stochastic integrand has norm at most $\varepsilon^{-2}$. Since $F(W_0)=1$,

$$
\frac1\varepsilon\mathbb P(T_\varepsilon\leq t)\leq\mathbb E\frac1{R_{t\wedge T_\varepsilon}}=1.
$$

Let $t\to\infty$, then $\varepsilon\downarrow0$. Any path hitting zero must first hit every positive $\varepsilon$, so $\mathbb P(\exists t:R_t=0)=0$.

For $r(w)=|w|$, $\partial_i r=w_i/r$ and $\Delta r=2/r$ in three dimensions. Itô's formula, initially localized away from zero, yields

$$
dR_t=\sum_{i=1}^3\frac{W_t^i}{R_t}dW_t^i+\frac1{R_t}dt.
$$

The [continuous local martingale](../../../../../../continuous-local-martingale.md) $\gamma_t=\sum_i\int_0^t(W_s^i/R_s)dW_s^i$ has bracket $[\gamma]_t=\int_0^t\sum_i(W_s^i/R_s)^2ds=t$ and starts at zero. By the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md), $\gamma$ is [Brownian motion](../../../../../../brownian-motion-split.md). Thus

$$
\boxed{R_t=1+\gamma_t+\int_0^t\frac1{R_s}ds.}
$$

This proves that the radial process is a [three-dimensional Bessel process](../../../../../../three-dimensional-bessel-process.md) solving the same equation as $X$ in part (b). The permitted uniqueness in distribution identifies their laws as processes.

The strong law in part (a) gives $Y_s\to\infty$, and the inverse clock satisfies $J_t\to\infty$. Hence $X_t=Y_{J_t}\to\infty$. Equality of process laws transfers this almost sure path property to $R$.

For the further logarithmic rate, fix $0<\eta<1/2$. Almost surely, for all sufficiently large $s$, $|B_s|\leq\eta s$. With a finite random lower cutoff $S$, for $u>S$,

$$
\int_S^u e^{(1-2\eta)s}ds\leq H_u\leq H_S+\int_S^u e^{(1+2\eta)s}ds.
$$

Taking logarithms and dividing by $u$ gives lower and upper asymptotic bounds $1-2\eta$ and $1+2\eta$. Letting $\eta\downarrow0$ along a countable sequence proves the [logarithmic growth of an exponential Brownian clock with positive drift](../../../../../../logarithmic-growth-of-an-exponential-brownian-clock-with-positive-drift.md), $\log H_u/u\to1$. Also $\log Y_u/u=B_u/u+1/2\to1/2$. Since $t=H_{J_t}$,

$$
\frac{\log X_t}{\log t}=\frac{\log Y_{J_t}/J_t}{\log H_{J_t}/J_t}\longrightarrow\frac12.
$$

Again transfer the full path event by uniqueness in distribution. We obtain the [logarithmic escape rate of three-dimensional Brownian motion](../../../../../../logarithmic-escape-rate-of-three-dimensional-brownian-motion.md)

$$
\boxed{|W_t|\longrightarrow\infty,\qquad\frac{\log|W_t|}{\log t}\longrightarrow\frac12\quad\text{almost surely}.}
$$

For an independent way to identify the value once existence of the almost sure limit is granted, use [Brownian scaling](../../../../../../brownian-scaling.md). At each fixed $t$, $W_t/\sqrt t$ has the law of $G+(1/\sqrt t,0,0)$, where $G$ is standard three-dimensional Gaussian. Its norm converges in distribution to the strictly positive finite variable $|G|$, so $\log(|W_t|/\sqrt t)$ is tight. Therefore

$$
\frac{\log|W_t|}{\log t}=\frac12+\frac{\log(|W_t|/\sqrt t)}{\log t}\longrightarrow\frac12\quad\text{in probability}.
$$

An existing almost sure limit must agree with this probability limit. This guesses and identifies the value through scaling, while the inverse-clock argument proves that the almost sure limit actually exists.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
