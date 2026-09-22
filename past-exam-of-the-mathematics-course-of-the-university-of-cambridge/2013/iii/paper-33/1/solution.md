<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $Ph=\mathbb Eh(X)$ and $P_nh=n^{-1}\sum_{i=1}^nh(X_i)$. A [function bracket](../../../../../bracketing-of-a-function-class.md) $[\ell,u]$ contains the measurable functions $h$ satisfying $\ell(z)\le h(z)\le u(z)$ for every $z\in T$. Require its endpoints to be integrable and call $P(u-\ell)$ its $L^1(P)$ width. A sufficient condition is that, for every $\varepsilon>0$, finitely many brackets of width at most $\varepsilon$ cover the whole class $\mathcal H$. Under this condition the [uniform strong law from finite L1 bracketing](../../../../../uniform-strong-law-from-finite-l1-bracketing.md) states

$$
\boxed{\sup_{h\in\mathcal H}|P_nh-Ph|\longrightarrow0\quad\text{almost surely}.}
$$

The conclusion holds outside a common measurable null set. If the supremum is not initially known to be measurable, this formulation means pathwise convergence on a measurable probability-one event; a [pointwise separable function class](../../../../../pointwise-separable-function-class.md), including the application below, has a measurable supremum. Pointwise brackets also ensure the sample inequalities hold simultaneously over the class.

To prove the result, choose a finite $\varepsilon$-cover $[\ell_r,u_r]$, $1\le r\le N$. If $h$ belongs to bracket $r$, monotonicity of the [empirical measure](../../../../../empirical-measure.md) and of expectation gives

$$
P_nh-Ph\le P_nu_r-Pu_r+P(u_r-h)\le |P_nu_r-Pu_r|+\varepsilon,
$$

and

$$
Ph-P_nh\le P(h-\ell_r)+P\ell_r-P_n\ell_r\le\varepsilon+|P_n\ell_r-P\ell_r|.
$$

Consequently

$$
\sup_{h\in\mathcal H}|P_nh-Ph|\le\varepsilon+\max_{r\le N}\max\{|P_nu_r-Pu_r|,|P_n\ell_r-P\ell_r|\}.
$$

Apply the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) to these finitely many integrable endpoints. On a probability-one event, the maximum tends to zero. Repeat with $\varepsilon=1/q$, $q\in\mathbb N$, and intersect the countably many probability-one events. The limiting supremum is bounded by $1/q$ for every $q$, hence is zero. This proves the [uniform law of large numbers](../../../../../uniform-law-of-large-numbers.md) without a boundedness assumption on the class itself.

For the [moment-generating function](../../../../../moment-generating-function.md), use the [empirical measure](../../../../../empirical-measure.md) estimator

$$
\boxed{\widehat m_n(s)=\frac1n\sum_{i=1}^n e^{sX_i},\qquad 0\le s\le t.}
$$

If $t=0$, this estimator and $m$ are both identically one. Otherwise, $X\ge0$ makes $e^{sX}$ increasing in $s$, and $e^{sX}\le e^{tX}$ provides an integrable envelope. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) shows that $m$ is continuous on $[0,t]$, hence uniformly continuous.

For any $\varepsilon>0$, choose a partition $0=s_0<s_1<\cdots<s_N=t$ so that $m(s_r)-m(s_{r-1})\le\varepsilon$ for every $r$. If $s\in[s_{r-1},s_r]$, then $e^{s_{r-1}z}\le e^{sz}\le e^{s_rz}$ for every $z\ge0$. These endpoint functions form finitely many integrable [function brackets](../../../../../bracketing-of-a-function-class.md) with the required $L^1(P)$ widths. The just-proved [uniform law of large numbers](../../../../../uniform-law-of-large-numbers.md) therefore gives

$$
\boxed{\sup_{s\in[0,t]}|\widehat m_n(s)-m(s)|\longrightarrow0\quad\text{almost surely}.}
$$

Both functions of $s$ are continuous; their supremum equals the supremum over a countable dense subset, so it is measurable. This proves [uniform consistency of an empirical moment-generating function](../../../../../uniform-consistency-of-an-empirical-moment-generating-function.md) using only the observed sample.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
