# Maximum-subarray segment summary

↑ **Parent:** [Maximum subarray problem](maximum-subarray-problem.md)

For a segment, store its total sum $S$, maximum possibly-empty prefix sum $P$, maximum possibly-empty suffix sum $Q$ and maximum possibly-empty internal contiguous sum $B$. Adjacent segment summaries combine by

$$
(S,P,Q,B)=\left(S_L+S_R,\ \max(P_L,S_L+P_R),\ \max(Q_R,S_R+Q_L),\ \max(B_L,B_R,Q_L+P_R)\right).
$$

A prefix either stays on the left or includes the whole left segment and a right prefix. A suffix has the symmetric decomposition. An internal segment either stays in one child or crosses the boundary as a left suffix followed by a right prefix. These cases prove the formulas, including empty candidates. Store the corresponding endpoints to recover a winning segment. This constant-size summary gives a [linear time](linear-time.md) [divide-and-conquer algorithm](divide-and-conquer-algorithm.md) for the empty-allowed [maximum subarray problem](maximum-subarray-problem.md).

## ↑ Ancestors (4)

1. [Maximum subarray problem](maximum-subarray-problem.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/5/c/solution.md)
