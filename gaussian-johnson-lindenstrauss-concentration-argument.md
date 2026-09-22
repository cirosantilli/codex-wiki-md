<h1 id="gaussian-johnson-lindenstrauss-concentration-argument">Gaussian Johnson–Lindenstrauss concentration argument</h1>

↑ **Parent:** [Gaussian Johnson–Lindenstrauss transform](gaussian-johnson-lindenstrauss-transform.md)

A short [concentration inequality](concentration-inequality.md) argument explains the bound. For a fixed nonzero [vector](vector.md) $u$, the normalized row products $\langle G_a,u\rangle/\|u\|_2$ are [independent random variables](independent-random-variables.md) with the [standard normal distribution](standard-normal-distribution.md), so

$$
R_u=\frac{\|Tu\|_2^2}{\|u\|_2^2}\ \sim\ \frac{\chi_k^2}{k},
\qquad\mathbb E R_u=1,\qquad\operatorname{Var}(R_u)=\frac2k.
$$

Use the [moment-generating function of a chi-squared distribution](moment-generating-function-of-a-chi-squared-distribution.md) and the [Chernoff bound](chernoff-bound.md) to obtain

$$
\begin{aligned}
\mathbb P(R_u\geq1+\varepsilon)
&\leq\exp\!\left[-\frac k2\bigl(\varepsilon-\log(1+\varepsilon)\bigr)\right],\\
\mathbb P(R_u\leq1-\varepsilon)
&\leq\exp\!\left[-\frac k2\bigl(-\varepsilon-\log(1-\varepsilon)\bigr)\right].
\end{aligned}
$$

For $0<\varepsilon<1$, elementary [logarithm](logarithm.md) inequalities bound their sum by $2e^{-kc(\varepsilon)}$. Apply the [union bound](boole-s-inequality.md) to the $\binom n2$ nonzero pair differences to get failure [probability](probability.md) at most $n(n-1)e^{-kc(\varepsilon)}\leq\delta$. Independence of different pairs is unnecessary; they use the same map. This combines fixed-[vector](vector.md) concentration with a finite-set [union bound](boole-s-inequality.md). [Lecture notes on metric embeddings, §2.1, pp. 20–21, and proof of Lemma 2.3.1, pp. 25–26: fixed-vector concentration and union bound over pair differences](lecture-notes-on-metric-embeddings-by-jiri-matousek.md)

## ↑ Ancestors (8)

1. [Gaussian Johnson–Lindenstrauss transform](gaussian-johnson-lindenstrauss-transform.md)
2. [Johnson–Lindenstrauss lemma](johnson-lindenstrauss-lemma.md)
3. [Metric embedding](metric-embedding.md)
4. [Functional analysis](functional-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
