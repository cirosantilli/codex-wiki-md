<h1 id="c9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Initialize all **eight** leaves, not seven: every observed base contributes a one-hot vector in the order A, C, G, T. The reference to $L-1$ leaf rows in the prose is inconsistent with its eight-leaf tree.

```
def initialise_prob(leafList):
    alphabet = {base: j for j, base in enumerate("ACGT")}
    result = np.zeros((2*len(leafList)-1, 4), dtype=float)
    for i, base in enumerate(leafList):
        result[i, alphabet[base]] = 1.
    return result

leaves = ["G", "A", "T", "G", "G", "G", "C", "G"]
prob = initialise_prob(leaves)
print(prob[:len(leaves)])
```

The initialized leaf rows are:

```
0 0 1 0
1 0 0 0
0 0 0 1
0 0 1 0
0 0 1 0
0 0 1 0
0 1 0 0
0 0 1 0
```

The remaining seven internal-node rows initially contain zeros. Their eventual entries are conditional [likelihoods](../../../../../likelihood-function.md) of descendant observations given the ancestral base, rather than normalized [posterior probabilities](../../../../../posterior-probability.md) of that ancestral base.

## ↑ Ancestors (13)

1. [B](../b.md)
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
