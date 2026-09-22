<h1 id="d11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

One simulation contributes its largest observed infected population and its last recorded time. Repeating this operation produces one row per realization:

```
def sir_sim_stats(n_sim,t_max,X0,beta,gamma,rng=None):
    result=np.empty((n_sim,2))
    for run in range(n_sim):
        t,s=sir_sim(t_max,X0,beta,gamma,rng)
        result[run]=s[:,1].max(),t[-1]
    return result
```

The maximum must be taken over the infected column, `states[:,1]`, rather than across all compartments. With the implementation in part (a), the final time is the [epidemic extinction](../../../../../epidemic-extinction.md) time if extinction occurs first, and otherwise the specified horizon; an outbreak still active at that horizon has a censored extinction time.

## ↑ Ancestors (13)

1. [B](../b.md)
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
