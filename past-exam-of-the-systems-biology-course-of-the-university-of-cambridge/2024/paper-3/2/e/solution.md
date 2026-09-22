<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**TODO: Complete the data-specific numerical results and diagnostics when the original `Iris_data.csv` is available.**

Plot all 10,001 stored states, including the initial value, and indicate the provisional [burn-in](../../../../../burn-in.md) boundary. Also display the retained chain's [autocorrelation function](../../../../../autocorrelation.md):

```
png("q2-trace.png", width = 1000, height = 700)
par(mfrow = c(2, 1), mar = c(4, 4.5, 2.5, 1))
plot(0:B, mu, type = "l", xlab = "Iteration", ylab = expression(mu),
     main = "Complete Metropolis trace")
abline(v = burn, col = "firebrick", lty = 2)
abline(h = m, col = "steelblue", lty = 3)
acf(post, main = "Autocorrelation after provisional burn-in")
dev.off()
# Check sensitivity to the chosen discard and to the retained time window.
for (discard in c(500L, 1000L, 2000L)) {
  kept <- mu[(discard + 2L):(B + 1L)]
  cat("Discard", discard, ": posterior mean", mean(kept), "\n")
}
cat("Means of retained halves:", mean(post[1:4500]),
    mean(post[4501:9000]), "\n")
```

A satisfactory [trace plot](../../../../../trace-plot.md) should show an initial transient, if any, followed by repeated exploration of one stable range with no continuing drift. Repeated values are expected because rejections are stored. If $n$ is large, the prescribed proposal standard deviation one can be much wider than the [posterior](../../../../../bayesian-posterior.md) scale $1/\sqrt n$, giving low acceptance and conspicuous plateaus. A flat-looking trace is therefore not by itself evidence of good exploration.

Compare the retained histogram with the exact [posterior density](../../../../../posterior-density.md), inspect [autocorrelation](../../../../../autocorrelation.md), compare separate retained windows, and assess sensitivity to the discarded count. Agreement supports the adequacy of this run; neither 10,000 iterations nor a chosen [burn-in](../../../../../burn-in.md) of 1,000 proves convergence. The [effective sample size of a Markov chain](../../../../../effective-sample-size-of-a-markov-chain.md) can be much smaller than the number of stored states.

**The actual trace cannot be diagnosed without `Iris_data.csv`.** The code produces the required trace when the measurements are available; the comments here specify what to examine rather than asserting an unseen chain has converged.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the systems biology course of the University of Cambridge](../../../../split.md)
6. [Systems Biology course of the University of Cambridge](../../../../../systems-biology-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
