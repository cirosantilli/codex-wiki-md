# Failure of unrestricted Big O composition

↑ **Parent:** [Big O notation](big-o-notation.md)

From $f_1=O(g_1)$ and $f_2=O(g_2)$ one cannot generally deduce $f_2\circ f_1=O(g_2\circ g_1)$. For $f_1(n)=2n$, $g_1(n)=n$ and $f_2(n)=g_2(n)=2^n$, the two premises hold, but the ratio of the compositions is $2^n$, which is unbounded. A constant scaling of an inner argument can change the growth order after an [exponential function](exponential-function.md) is applied.

## ↑ Ancestors (6)

1. [Big O notation](big-o-notation.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/discrete-mathematics-continuous-mathematics-and-probability/3/c/solution.md)
