<h1 id="d11/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

“Failed to take off” needs an operational definition; the two separated groups in the [histograms](../../../../../histogram.md) suggest a low peak or an early end. For example, classify a run as a failure if its peak is below ten infected individuals, or alternatively if its extinction time is below ten days:

```
failed_by_peak = stats[:,0] < 10
failed_by_time = stats[:,1] < 10
print(failed_by_peak.mean(), failed_by_time.mean())
```

**Both definitions give $255/1000=0.255$ in this run.** Here they also classify the same 255 realizations, although agreement is not guaranteed for other simulations or cutoffs. These are empirical failure fractions for the stated rules, not exact model constants.

The early [branching process](../../../../../branching-process.md) approximation provides a useful check: while susceptible depletion is negligible, $R_0\simeq4$ gives eventual extinction probability about $1/R_0=0.25$ from one initial infection. Allowing for the initial susceptible fraction gives a rate ratio $\gamma/(\beta\times0.99)\simeq0.253$; both approximations are compatible with this simulation, but neither defines the finite-population cutoff exactly.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [D11](../../d11.md)
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
