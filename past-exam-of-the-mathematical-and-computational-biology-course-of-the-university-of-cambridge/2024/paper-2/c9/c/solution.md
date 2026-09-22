<h1 id="c9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For node $v$ with children $l,r$, the [phylogenetic pruning algorithm](../../../../../phylogenetic-pruning-algorithm.md) combines the two conditionally independent descendant subtrees:

$$
L_v(a)=\left[\sum_b P_{ab}(t_l)L_l(b)\right]
\left[\sum_c P_{ac}(t_r)L_r(c)\right].
$$

The [likelihood function](../../../../../likelihood-function.md) is $\mathcal L(\mu)=\frac14\sum_a L_{\mathrm{root}}(a)$ under a uniform ancestral prior. In the supplied numbering, children have smaller indices than their parents, so increasing node order is a valid bottom-up traversal:

```
def felsenstein(prob, mu, L, left, right, left_time, right_time):
    # All four entries are overwritten at every internal node.
    for node in range(L, 2*L-1):
        Tl = np.array([[jukes(a,b,left_time[node],mu)
                        for b in range(4)] for a in range(4)])
        Tr = np.array([[jukes(a,b,right_time[node],mu)
                        for b in range(4)] for a in range(4)])
        prob[node] = (Tl @ prob[left[node]]) * (Tr @ prob[right[node]])
    return float(np.log(prob[-1].mean()))

print(felsenstein(prob, .5, len(leaves), left, right, left_time, right_time))
```

**At $\mu=0.5$, the log-likelihood is $-10.5052883$.** Internal rows must remain unnormalized in this implementation, because their magnitudes contribute to the tree [likelihood function](../../../../../likelihood-function.md); normalization without retaining the removed factors would lose that information. The final root normalization required for a [posterior probability](../../../../../posterior-probability.md) is a separate step in part (e).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [C9](../../c9.md)
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
