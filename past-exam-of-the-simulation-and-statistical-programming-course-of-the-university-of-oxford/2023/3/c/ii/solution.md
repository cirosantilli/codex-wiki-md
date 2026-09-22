<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The source's function name suggests a log return value, and (c)(i) asks for $\log\alpha$, while the wording here and in (c)(iv) asks for the acceptance [probability](../../../../../probability.md). We use the literal probability-returning convention and explicitly exponentiate the result of (c)(i):

```
mylogapp <- function(x, u, v, sigma_inv) {
  d <- v - u
  log_ratio <- as.numeric(crossprod(d, sigma_inv %*% (x - (u + v) / 2)))
  log_alpha <- min(0, log_ratio)
  exp(log_alpha)
}
```

Thus `mylogapp` returns $\alpha\in[0,1]$, and (c)(iv) compares it directly with a [uniform distribution](../../../../../continuous-uniform-distribution.md) draw. Taking the minimum before exponentiating prevents overflow. The arguments $u,v$ are assumed to be valid neighbouring states. A log-returning convention would instead return `log_alpha` and compare `log(runif(1))` with it; the two conventions implement the same [Metropolis–Hastings algorithm](../../../../../metropolis-hastings-algorithm.md), provided the caller uses the matching comparison.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
