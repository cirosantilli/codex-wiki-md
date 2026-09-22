# Optimal bounded influence function for normal location

↑ **Parent:** [Huber score](huber-score.md)

For standard [normal distribution](normal-distribution.md) location estimation, an [influence function](influence-function.md) $h$ obeys $\mathbb E[Zh(Z)]=1$. Under $|h|\le C$, minimize $\mathbb E h^2$ by projecting $ax$ onto $[-C,C]$, choosing $a$ to meet that identity. For $C>\sqrt{\pi/2}$ this gives the displayed [Huber score](huber-score.md) normalized by $2\Phi(K)-1$, with $C=K/(2\Phi(K)-1)$. Pointwise minimality of $h^2-2axh$ proves global optimality after integration. At $C=\sqrt{\pi/2}$ the only feasible normalized function is $C\operatorname{sgn}(x)$ almost everywhere, the [influence function of the sample median](influence-function-of-the-sample-median.md). The endpoint is a limit of rescaled clipped scores, not the identically zero score obtained by substituting $K=0$ literally.

## ↑ Ancestors (8)

1. [Huber score](huber-score.md)
2. [Huber location estimator](huber-location-estimator.md)
3. [Robust statistics](robust-statistics.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32/4/solution.md)
