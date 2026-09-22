<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

The closure table is

$$
\begin{array}{c|ccc}
&\text{union}&\text{intersection}&\text{complement}\\ \hline
\text{regular}&\text{Yes}&\text{Yes}&\text{Yes}\\
\text{context-free}&\text{Yes}&\text{No}&\text{No}\\
\text{computable}&\text{Yes}&\text{Yes}&\text{Yes}\\
\text{computably enumerable}&\text{Yes}&\text{Yes}&\text{No}
\end{array}
$$

For the context-free intersection failure, take

$$
L_1=\{a^nb^nc^k:n,k\geq0\},\qquad L_2=\{a^kb^nc^n:n,k\geq0\}.
$$

Both are context-free, but $L_1\cap L_2=\{a^nb^nc^n:n\geq0\}$ is not. If context-free languages were also closed under complement, their closure under union and De Morgan's law would imply closure under intersection, so complement closure also fails. Finally, the halting set is computably enumerable but its complement is not, disproving complement closure for computably enumerable languages.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
