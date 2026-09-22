<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Construct one infinite [binary sequence](../../../../../bitstream.md) $u$ by concatenating every binary word of length one, then every word of length two, then every word of length three, and so on, in [lexicographic order](../../../../../lexicographic-order.md) within each length. Every finite binary word occurs somewhere in $u$.

Given any target [sequence](../../../../../sequence.md) $s$ and any $\eta>0$, choose $N$ such that $2^{-N}<\eta$. The word $s_1\cdots s_N$ occurs in $u$, beginning after some $k$ symbols. Thus $\sigma^ku$ agrees with $s$ in its first $N$ positions, and the prescribed [metric](../../../../../metric.md) gives

$$
d(\sigma^ku,s)\leq\sum_{i>N}2^{-i}=2^{-N}<\eta.
$$

Every open [open ball](../../../../../open-ball.md) about every point therefore meets the [forward orbit](../../../../../forward-orbit.md) of $u$. **This [forward orbit](../../../../../forward-orbit.md) is [dense](../../../../../dense-set.md) in $\Sigma$.** The argument identifies finite-prefix [cylinder sets](../../../../../cylinder-set.md) as arbitrarily small neighborhoods in this [metric](../../../../../metric.md); no binary-expansion convention for real numbers is needed.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the nonlinear systems course of the University of Oxford](../../../../split.md)
6. [Nonlinear systems course of the University of Oxford](../../../../../nonlinear-systems-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
