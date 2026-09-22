<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**TODO: Complete the data-specific numerical results and diagnostics when the original `Iris_data.csv` is available.**

The identity

$$
\sum_i(x_i-\mu)^2=\sum_i(x_i-\bar x)^2+n(\mu-\bar x)^2
$$

shows that the [likelihood function](../../../../../../likelihood-function.md) is a bell-shaped curve in $\mu$, maximized at the [sample mean](../../../../../../sample-mean.md), with width $1/\sqrt n$. Its actual vertical scale also depends on the within-sample sum of squares.

Continue the R script with:

```
sse <- sum((x - xbar)^2)
loglik <- function(mu) {
  -n/2 * log(2*pi) - 0.5 * (sse + n * (mu - xbar)^2)
}
grid <- seq(3, 6, length.out = 2001L)
ell <- loglik(grid)
png("q2-likelihood.png", width = 900, height = 600)
par(mar = c(4.5, 4.5, 4, 1))
if (max(ell) > log(.Machine$double.xmin)) {
  plot(grid, exp(ell), type = "l", xlab = expression(mu),
       ylab = expression(L(mu)), main = "Likelihood on [3,6]")
} else {
  # Explicitly label a proportional likelihood if the true scale underflows.
  plot(grid, exp(ell - max(ell)), type = "l", xlab = expression(mu),
       ylab = "Likelihood relative to maximum on plotted grid",
       main = "Likelihood on [3,6] (rescaled)")
}
abline(v = xbar, col = "steelblue", lty = 2)
dev.off()
```

Working first with the [log-likelihood](../../../../../../log-likelihood.md) avoids premature numerical underflow. The fallback preserves the shape on the requested interval and labels the altered scale. **A data-specific plot requires the missing CSV file**; no fabricated observation set is used here.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the systems biology course of the University of Cambridge](../../../../../split.md)
7. [Systems Biology course of the University of Cambridge](../../../../../../systems-biology-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
