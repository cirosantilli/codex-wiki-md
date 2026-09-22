<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [decision tree](../../../../../../decision-tree.md) queries individual input bits, chooses subsequent queries from previous answers and labels each leaf with an output. Its [decision-tree depth](../../../../../../decision-tree-depth.md) is the largest number of queries on any root-to-leaf path; $D(f)$ is the least such depth over trees computing $f$. An [evasive Boolean function](../../../../../../evasive-boolean-function.md) on $n$ bits has $D(f)=n$.

Remove repeated queries along any path, since their answers are already known. A leaf at depth $r\leq d<n$ fixes $r$ bits and leaves at least one bit free. The inputs reaching it form a subcube on which $f$ is constant, say $b$. Its contribution to the alternating sum is

$$
b(-1)^{\sum\text{fixed bits}}\prod_{\text{free bits}}(1-1)=0.
$$

Here $\operatorname{wt}(x)$ is the [Hamming weight](../../../../../../hamming-weight.md). The leaf subcubes partition the input cube, so adding their contributions proves

$$
\boxed{D(f)<n\Longrightarrow\sum_{x\in\{0,1\}^n}(-1)^{\operatorname{wt}(x)}f(x)=0}.
$$

The contrapositive is the [alternating-sum criterion for decision-tree evasiveness](../../../../../../alternating-sum-criterion-for-decision-tree-evasiveness.md): a nonzero alternating sum forces all $n$ bits to be necessary in the worst case.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
