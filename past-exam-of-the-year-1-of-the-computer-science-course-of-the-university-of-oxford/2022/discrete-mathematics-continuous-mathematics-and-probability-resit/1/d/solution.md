<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Pad every [integer](../../../../../integer-split.md) from $0$ through $999999$ with leading zeros to obtain a unique six-digit decimal string. If its digits sum to $5$, each digit is automatically at most $5$, so the usual digit [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md) $9$ adds no restriction. We therefore count the nonnegative [integer](../../../../../integer-split.md) solutions of

$$
d_1+d_2+\cdots+d_6=5.
$$

By [stars and bars](../../../../../stars-and-bars-combinatorics.md), there are $\binom{5+6-1}{6-1}=\binom{10}{5}$. The all-zero string is not counted because its [digit sum](../../../../../digit-sum.md) is zero, so every counted [integer](../../../../../integer-split.md) is positive. Thus the answer is **$252$**.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Discrete mathematics, continuous mathematics and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
