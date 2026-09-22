<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

If $L<1$, set $\varepsilon=(1-L)/2>0$. The definition of [limit of a sequence](../../../../../../../limit-of-a-sequence.md) gives $a_n<L+\varepsilon=(1+L)/2<1$ for all sufficiently large $n$, contradicting $a_n\geq1$. Hence $\boxed{L\geq1}$.

Factor the difference of cubes. Since both [cube roots](../../../../../../../cube-root.md) are at least one,

$$
\left|a_n^{1/3}-L^{1/3}\right|
=\frac{|a_n-L|}{a_n^{2/3}+a_n^{1/3}L^{1/3}+L^{2/3}}
\leq\frac{|a_n-L|}{3}.
$$

Given $\varepsilon>0$, the definition of [limit of a sequence](../../../../../../../limit-of-a-sequence.md) supplies $N$ with $|a_n-L|<3\varepsilon$ for $n\geq N$. The displayed [inequality](../../../../../../../inequality-mathematics.md) then gives $|a_n^{1/3}-L^{1/3}|<\varepsilon$, proving directly that $\boxed{a_n^{1/3}\to L^{1/3}}$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
