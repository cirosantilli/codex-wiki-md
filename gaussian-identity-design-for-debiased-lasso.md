# Gaussian identity design for debiased Lasso

↑ **Parent:** [Debiased-Lasso asymptotic normality](debiased-lasso-asymptotic-normality.md)

In the [normal linear model](normal-linear-model.md), assume $\varepsilon\sim N_n(0,\sigma^2I)$ is independent of $X$. Independent rows of $X$ with [multivariate normal distribution](multivariate-normal-distribution.md) $N_p(0,I_p)$ give a simple random design for [Debiased Lasso](debiased-lasso.md). Let $p\to\infty$, $\log p=o(n)$ and $s\log p=o(\sqrt n)$, with fixed positive noise scale. Choose the [Lasso](lasso.md) penalty and all [Nodewise Lasso](nodewise-lasso.md) penalties as sufficiently large constant multiples of $\sqrt{\log p/n}$, including the noise scale in the former. Uniform sample cross-correlations are bounded by this scale, so zero is the nodewise solution with [probability](probability.md) tending to one. Column squared [norms](norm.md) divided by $n$ converge uniformly to one. To check the [Compatibility condition for the Lasso](compatibility-condition-for-the-lasso.md) directly, put $\widehat\Sigma=X^TX/n$ and $\eta=\max_{j,k}|\widehat\Sigma_{jk}-\mathbf1_{\{j=k\}}|$. On the [Lasso cone condition](lasso-cone-condition.md), $\|\delta\|_1\le4\|\delta_S\|_1$, and the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives

$$
\delta^T\widehat\Sigma\delta\ge\|\delta\|_2^2-\eta\|\delta\|_1^2\ge(1/s-16\eta)\|\delta_S\|_1^2.
$$

For $s\ge1$, [entrywise concentration of a Gaussian Gram matrix](entrywise-concentration-of-a-gaussian-gram-matrix.md) gives $\eta\le D_0\sqrt{\log p/n}$ with [probability](probability.md) tending to one for sufficiently large fixed $D_0$. The stated sparsity condition implies $s\eta\to0$ on this event, so one can take $\phi^2\ge1/2$ eventually. The conditional [Gaussian tail bound](gaussian-tail-bound.md) for the noise score and the [Basic inequality for the Lasso](basic-inequality-for-the-lasso.md) then give $\|\widehat\beta-\beta^0\|_1\le C s\sqrt{\log p/n}$ with [probability](probability.md) tending to one. Consequently the [debiased-Lasso remainder bound](debiased-lasso-remainder-bound.md) is at most $A s\log p/\sqrt n$ with [probability](probability.md) tending to one, for a fixed constant $A$. These assumptions allow both $p$ and $s$ to grow, for example $p=n^2$, $s=\lfloor n^{1/4}\rfloor$.

## ↑ Ancestors (7)

1. [Debiased-Lasso asymptotic normality](debiased-lasso-asymptotic-normality.md)
2. [Debiased Lasso](debiased-lasso.md)
3. [Lasso](lasso.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205/6/solution.md)
