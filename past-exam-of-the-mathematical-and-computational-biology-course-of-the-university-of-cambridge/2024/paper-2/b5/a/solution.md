<h1 id="b5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Generate independent [Bernoulli random variables](../../../../../bernoulli-distribution.md) above the diagonal and set everything else to zero. Taking the strict upper triangle of a random square array gives each allowed entry probability $1/2$ of being one:

```
import numpy as np
rng = np.random.default_rng(2024)


def rand_triu(n):
    return np.triu(rng.integers(0, 2, size=(n, n)), k=1)


example = rand_triu(10)
print(example)
```

One reproducible [strictly upper triangular matrix](../../../../../strictly-upper-triangular-matrix.md) is:

```
0 1 0 0 0 0 1 1 1 1
0 0 1 0 0 0 1 0 0 0
0 0 0 1 1 0 0 1 1 0
0 0 0 0 1 1 1 1 0 0
0 0 0 0 0 0 1 1 1 0
0 0 0 0 0 0 0 0 0 0
0 0 0 0 0 0 0 0 0 1
0 0 0 0 0 0 0 0 0 0
0 0 0 0 0 0 0 0 0 0
0 0 0 0 0 0 0 0 0 0
```

Every matrix returned in this way is a [nilpotent matrix](../../../../../nilpotent-matrix.md); randomness affects its [nilpotency index](../../../../../nilpotency-index.md), not the fact of the nilpotent property.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [B5](../../b5.md)
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
