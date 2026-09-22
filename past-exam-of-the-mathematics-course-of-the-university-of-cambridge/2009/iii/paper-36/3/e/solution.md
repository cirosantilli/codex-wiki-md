<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Delete the plate [random effects](../../../../../../random-effect.md) from the [linear predictor](../../../../../../linear-predictor.md) and remove their stochastic nodes and the unused scale/precision nodes. The observation layer then remains a [Poisson distribution](../../../../../../poisson-distribution.md) with

$$
\boxed{\log\mu_{ij}=\alpha+\beta\log(x_i+10)+\gamma x_i.}
$$

For example the essential [WinBUGS](../../../../../../winbugs.md) observation block can be written as
```
for (i in 1:doses) {
for (j in 1:plates) {
y[i,j] ~ dpois(mu[i,j])
log(mu[i,j]) <- alpha + beta*log(x[i]+10) + gamma*x[i]
}
}
```
Retain the coefficient priors. This is the $\tau=0$ sampling model implemented directly; attempting to keep `1/(tau*tau)` while fixing `tau` to zero would divide by zero.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
