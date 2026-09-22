<h1 id="c8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each alignment column, ignore gaps, form the [empirical distribution](../../../../../type-information-theory.md) of its [amino acids](../../../../../amino-acid.md), and calculate its [Shannon entropy](../../../../../information-entropy-split.md) in bits. The requested [alignment column information content](../../../../../alignment-column-information-content.md) is

$$
\boxed{R_i=\log_2(20)-H_i
=\sum_{a:p_{ia}>0}p_{ia}\log_2(20p_{ia}).}
$$

Thus it is the [relative entropy](../../../../../kullback-leibler-divergence.md) from the column distribution to the uniform distribution on twenty [amino acids](../../../../../amino-acid.md), not the ordinary [Shannon entropy](../../../../../information-entropy-split.md) itself. A column containing one residue type has the maximum value $\log_2(20)=4.321928$ bits.

```
information = []
for j in range(A.shape[1]):
    counts, n = emission_counts(A[:, j])
    p = np.array(list(counts.values()), dtype=float) / n
    H = -np.sum(p * np.log2(p))
    information.append(float(np.log2(20) - H))
print(np.round(information, 4))
```

**The values for all 79 alignment columns are as follows**, in bits. Each line lists its one-based column interval followed by the corresponding values in order:

```
01–10: 1.9025, 1.5964, 1.9025, 3.8187, 1.9025, 1.5964, 1.9025, 3.5577, 1.9025, 1.9025
11–20: 2.4420, 3.3355, 1.5964, 4.3219, 3.8187, 1.6803, 3.0975, 3.3355, 3.0975, 2.4420
21–30: 2.5692, 2.8219, 3.5106, 3.3219, 4.3219, 4.3219, 2.8000, 2.0703, 2.6574, 1.8003
31–40: 2.1938, 1.9163, 3.7784, 3.2606, 1.6803, 1.6803, 2.6642, 2.5692, 2.8753, 2.2631
41–50: 2.8753, 3.3355, 1.6803, 2.9703, 3.3355, 2.7914, 2.2086, 2.5692, 4.3219, 1.3742
51–60: 2.2631, 4.3219, 4.3219, 3.8187, 4.3219, 3.5577, 2.8753, 1.9025, 2.7914, 2.0409
61–70: 3.3355, 2.7370, 2.4309, 2.4309, 2.5692, 2.0409, 2.5692, 3.3355, 2.9298, 3.5577
71–79: 1.9025, 1.8187, 4.3219, 2.2631, 3.8187, 2.4309, 1.9025, 1.9025, 1.9025
```

A high score indicates conservation among the observed nongap letters, but does not itself imply low [gap fraction](../../../../../gap-fraction.md). For example, an insertion column represented by only one observed nongap residue has maximal information by this calculation; its tiny sample size still makes that estimate uncertain.

## ↑ Ancestors (13)

1. [C](../c.md)
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
