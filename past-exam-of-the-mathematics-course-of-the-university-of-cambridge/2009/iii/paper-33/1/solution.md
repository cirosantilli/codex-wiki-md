<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $Ph=\mathbb E h(X)$ and $P_nh=n^{-1}\sum_{i=1}^nh(X_i)$ for the population and [empirical measure](../../../../../empirical-measure.md). The [empirical distribution function](../../../../../empirical-distribution-function.md) is

$$
\boxed{F_n(t)=\frac1n\sum_{i=1}^n\mathbf1_{\{X_i\le t\}}.}
$$

Fix $\varepsilon>0$ and a finite cover by [function brackets](../../../../../bracketing-of-a-function-class.md) $[l_r,u_r]$ of $L^1(P)$ width below $\varepsilon$. If $h$ belongs to the $r$th bracket, then

$$
P_nh-Ph\le(P_nu_r-Pu_r)+P(u_r-h)\le|P_nu_r-Pu_r|+\varepsilon,
$$

and, using $l_r$ instead, $Ph-P_nh\le|P_nl_r-Pl_r|+\varepsilon$. Thus

$$
\sup_{h\in\mathcal H}|P_nh-Ph|
\le\varepsilon+\max_r\max\{|P_nl_r-Pl_r|,|P_nu_r-Pu_r|\}.
$$

The [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) applies to every integrable endpoint because the sample consists of [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md). For this finite collection the maximum tends to zero on a common probability-one event. Apply the argument for $\varepsilon=1/m$, $m=1,2,\ldots$, and intersect those countably many events. On the resulting event the limsup is at most $1/m$ for every $m$, proving the [uniform strong law from finite L1 bracketing](../../../../../uniform-strong-law-from-finite-l1-bracketing.md). This pathwise argument also avoids assuming without justification that an arbitrary uncountable supremum is measurable.

For the [Glivenko-Cantelli theorem](../../../../../glivenko-cantelli-theorem.md), take $h_t(x)=\mathbf1_{\{x\le t\}}$. Here is a finite bracketing construction which also handles atoms of the distribution. Choose $0<\delta<\varepsilon$ and divide the possible values of $F(t)$ into finitely many bins $[r\delta,(r+1)\delta)$, including the final value one. For each nonempty parameter set $T_r=\{t:r\delta\le F(t)<(r+1)\delta\}$, set $l_r=\inf_{t\in T_r}h_t$ and $u_r=\sup_{t\in T_r}h_t$ pointwise. These functions are indicators of rays, possibly with an open endpoint, so they are measurable. Monotonicity of $h_t$ and monotone limits at the extreme thresholds give $Pl_r=\inf_{t\in T_r}F(t)$ and $Pu_r=\sup_{t\in T_r}F(t)$. Hence $P(u_r-l_r)\le\delta<\varepsilon$. No continuity of $F$ is required. Applying the proved uniform law gives

$$
\boxed{\sup_{t\in\mathbb R}|F_n(t)-F(t)|\longrightarrow0\quad\text{almost surely}.}
$$

For an uncountable class of [continuous functions](../../../../../continuous-function.md), use $\mathcal H=\{h_a(x)=a\sin x:0\le a\le1\}$. The functions are distinct, bounded and integrable for every probability law. Moreover $\sup_{0\le a\le1}|P_nh_a-Ph_a|=|P_n\sin-P\sin|\to0$ by the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md). This supplies the requested example without additional compactness machinery.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
