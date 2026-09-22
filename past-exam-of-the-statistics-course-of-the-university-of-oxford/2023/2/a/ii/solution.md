<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) states that a test which rejects where the joint [likelihood ratio](../../../../../likelihood-ratio.md) $L_1/L_0$ is largest is a [most powerful test](../../../../../most-powerful-test.md) of its size: its power is at least that of any test with no larger size. More precisely, choose a threshold $k$ and reject if $L_1/L_0>k$, accept if it is smaller, and if necessary randomize on equality to attain the specified size.

For an independent and identically distributed [statistical sample](../../../../../statistical-sample.md), take

$$
Y_i=\log\frac{f_0(X_i)}{f_1(X_i)}.
$$

The $Y_i$ are [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) under either simple hypothesis, and the log joint ratio is their sum. Thus the nonrandomized threshold form can be written

$$
\boxed{\sum_{i=1}^nY_i\leq c}
$$

with $c=-\log k$, using either strict or non-strict inequality when the boundary has probability zero. The usual finite-log expression assumes positive common support; zero densities can instead be handled by the extended likelihood ratio on the relevant supports. Continuous observations alone do not ensure a continuous likelihood-ratio statistic: ties may require the boundary randomization in the lemma. This qualification preserves the exact-size formulation.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
