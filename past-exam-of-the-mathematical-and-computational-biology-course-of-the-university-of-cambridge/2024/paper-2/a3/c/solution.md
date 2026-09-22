<h1 id="a3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use reproducible random starts and retain the best successful result:


```
rng = np.random.default_rng(2024)
starts = rng.uniform(-4, 4, size=100)
results = [opt.minimize(lambda z: f(z[0]), x0=[x0]) for x0 in starts]
successful = [result for result in results if result.success]
best = min(successful, key=lambda result: result.fun)
print(best.x[0], best.fun)
```
The estimate is **$x_{\min}\simeq-0.309213$, $f_{\min}\simeq0.0192409$**. This [random-restart optimization](../../../../../random-restart-optimization.md) improves coverage of the different attraction regions, but their number alone does not guarantee global optimality.

Here an analytic check is possible. For $|x|\geq\pi/5$, the envelope gives $f(x)\geq1-e^{-\pi^2/125}\simeq0.0759$, above the candidate. On $[0,\pi/5]$, $f\geq1$. In the remaining interval $[-\pi/5,0]$, the [derivative](../../../../../derivative.md) condition is equivalent, with $z=-x$, to $\cot(5z)=0.08z$. The left side decreases strictly from $+\infty$ to $-\infty$ while the right side increases, giving one minimum. This certifies the selected well as global rather than relying only on the restart experiment.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [A3](../../a3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
