<h1 id="c8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each [match state](../../../../../match-state.md), count the nongap [amino acids](../../../../../amino-acid.md) and divide by the number of nongap observations in that column. A gap is not one of the twenty emitted [amino acids](../../../../../amino-acid.md); including it in the denominator would make the [emission probabilities](../../../../../emission-probability.md) sum to less than one:

```
def emission_counts(column):
    counts = Counter(str(x) for x in column if x != ".")
    n = sum(counts.values())
    if n == 0:
        raise ValueError("an all-gap column has no empirical emission distribution")
    return counts, n

match_emissions = {}
for state, j in enumerate(match_columns, 1):
    counts, n = emission_counts(A[:, j])
    match_emissions[state] = {aa: count/n for aa, count in counts.items()}
    print(state, j+1, match_emissions[state])
```

The table gives an exact compact representation of **every [emission probability](../../../../../emission-probability.md)**: divide each displayed count by the denominator $n$ in its row; all unlisted [amino acids](../../../../../amino-acid.md) have probability zero. The state number follows the order of [match states](../../../../../match-state.md), while the column refers to the original [multiple sequence alignment](../../../../../multiple-sequence-alignment.md).

| State | Alignment column | $n$ | Nongap counts |
| --- | --- | --- | --- |
| 1 | 1 | 9 | I:1, K:1, R:1, S:2, V:3, Y:1 |
| 2 | 2 | 9 | D:1, E:2, G:1, I:1, L:1, Q:2, S:1 |
| 3 | 3 | 9 | E:2, I:1, K:1, Q:1, R:3, T:1 |
| 4 | 4 | 9 | L:8, M:1 |
| 5 | 5 | 9 | E:3, G:1, L:2, N:1, Q:1, S:1 |
| 6 | 6 | 9 | A:1, D:2, G:1, K:1, N:1, S:2, T:1 |
| 7 | 7 | 9 | A:1, E:3, I:2, L:1, M:1, V:1 |
| 8 | 8 | 9 | I:2, L:7 |
| 9 | 9 | 9 | D:3, E:1, K:1, L:2, N:1, Q:1 |
| 10 | 10 | 9 | D:1, E:3, G:1, N:1, P:1, S:2 |
| 11 | 11 | 9 | A:5, D:1, G:1, P:1, T:1 |
| 12 | 12 | 9 | I:1, L:7, Y:1 |
| 13 | 13 | 9 | E:1, F:1, G:1, H:2, M:1, Q:2, T:1 |
| 14 | 14 | 9 | F:9 |
| 15 | 15 | 9 | F:1, L:8 |
| 16 | 16 | 9 | E:1, I:1, L:1, N:3, Q:1, R:1, Y:1 |
| 17 | 17 | 9 | D:6, E:2, S:1 |
| 18 | 18 | 9 | C:7, F:1, S:1 |
| 19 | 19 | 9 | K:1, N:6, R:2 |
| 20 | 20 | 9 | E:1, F:1, I:5, L:1, V:1 |
| 21 | 21 | 9 | K:3, P:1, Q:1, S:4 |
| 22 | 29 | 7 | K:4, P:1, R:1, S:1 |
| 23 | 30 | 7 | E:2, F:1, G:1, I:1, K:1, V:1 |
| 24 | 31 | 7 | D:3, E:1, G:1, K:1, S:1 |
| 25 | 32 | 8 | D:1, E:1, G:1, K:1, N:1, R:3 |
| 26 | 33 | 8 | D:7, N:1 |
| 27 | 34 | 8 | A:1, P:6, S:1 |
| 28 | 35 | 9 | C:1, H:1, I:1, K:1, M:1, R:1, T:3 |
| 29 | 36 | 9 | E:1, F:1, G:1, L:1, Q:3, W:1, Y:1 |
| 30 | 37 | 9 | I:5, L:1, T:2, Y:1 |
| 31 | 38 | 9 | A:1, G:1, P:3, S:4 |
| 32 | 39 | 9 | I:1, K:6, L:1, R:1 |
| 33 | 40 | 9 | F:1, N:1, Q:4, T:2, V:1 |
| 34 | 41 | 9 | A:1, F:1, I:1, V:6 |
| 35 | 42 | 9 | I:1, L:7, V:1 |
| 36 | 43 | 9 | A:1, C:1, E:1, N:1, R:1, S:3, V:1 |
| 37 | 44 | 9 | D:3, E:5, Q:1 |
| 38 | 45 | 9 | A:1, C:7, I:1 |
| 39 | 46 | 9 | K:2, L:3, R:4 |
| 40 | 47 | 9 | A:3, E:1, L:1, N:3, T:1 |
| 41 | 48 | 9 | I:4, L:1, T:1, V:3 |
| 42 | 49 | 9 | L:9 |
| 43 | 50 | 9 | D:1, E:1, H:1, Q:1, S:1, T:1, V:1, Y:2 |
| 44 | 51 | 9 | E:1, K:1, Q:2, R:1, V:4 |
| 45 | 52 | 9 | L:9 |
| 46 | 53 | 9 | G:9 |
| 47 | 54 | 9 | P:8, T:1 |
| 48 | 55 | 9 | W:9 |
| 49 | 56 | 9 | A:2, C:7 |
| 50 | 57 | 9 | A:6, C:1, L:1, T:1 |
| 51 | 58 | 9 | A:1, D:3, F:1, S:2, V:1, Y:1 |
| 52 | 59 | 9 | K:4, R:2, S:3 |
| 53 | 60 | 9 | A:2, F:1, I:2, L:2, V:2 |
| 54 | 61 | 9 | A:7, G:1, Y:1 |
| 55 | 62 | 9 | E:3, G:3, Q:3 |
| 56 | 63 | 9 | I:3, M:3, T:1, Y:2 |
| 57 | 64 | 9 | F:3, L:2, M:3, N:1 |
| 58 | 65 | 9 | H:1, I:3, L:1, V:4 |
| 59 | 66 | 9 | K:1, M:1, P:1, R:4, S:1, T:1 |
| 60 | 67 | 9 | D:1, E:3, Q:4, Y:1 |
| 61 | 68 | 9 | I:1, L:7, M:1 |
| 62 | 69 | 9 | D:1, E:4, Q:4 |
| 63 | 70 | 9 | K:7, R:2 |
| 64 | 71 | 9 | A:1, I:2, M:1, N:1, R:1, Y:3 |
| 65 | 72 | 9 | A:1, C:1, D:1, E:2, I:2, V:2 |
| 66 | 73 | 9 | K:9 |
| 67 | 74 | 9 | H:4, L:1, Q:2, S:1, V:1 |
| 68 | 75 | 9 | E:8, Q:1 |
| 69 | 76 | 9 | Q:3, R:1, S:2, T:3 |
| 70 | 77 | 9 | C:2, E:3, G:1, R:1, S:1, V:1 |
| 71 | 78 | 9 | A:1, D:2, E:3, I:1, K:1, Y:1 |
| 72 | 79 | 9 | I:2, L:3, M:1, N:1, Q:1, V:1 |

These are unregularized [maximum-likelihood estimates](../../../../../maximum-likelihood-estimator.md) of the [emission probabilities](../../../../../emission-probability.md). No additional artificial observations are added. Although only emissions are requested here, a full [profile hidden Markov model](../../../../../profile-hidden-markov-model.md) would also require transitions and deletion mechanisms to represent the gaps that remain in some match columns.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [C8](../../c8.md)
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
