<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Pad every number with leading zeros to obtain exactly $n$ decimal digits. Its digits are a solution of $d_1+\cdots+d_n=9$ in nonnegative [integers](../../../../../integer-split.md). Conversely every such solution is a valid digit string, since no individual digit can exceed $9$; its digit sum also excludes the number zero. The [stars and bars](../../../../../stars-and-bars-combinatorics.md) count therefore gives

$$
f(n)=\binom{n+8}{9}=\frac1{9!}\prod_{j=0}^8(n+j).
$$

For $n\geq1$, $n+j\leq n(j+1)$, so $f(n)\leq n^9\prod_{j=0}^8(j+1)/9!=n^9$. Thus **$f(n)=O(n^9)$**, with an explicit [Big O notation](../../../../../big-o-notation.md) constant $C=1$ and threshold $n=1$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Discrete mathematics, continuous mathematics, and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
