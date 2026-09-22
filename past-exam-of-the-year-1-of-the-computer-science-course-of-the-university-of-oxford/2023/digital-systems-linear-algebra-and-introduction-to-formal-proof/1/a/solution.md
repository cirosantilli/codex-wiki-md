<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write an $n$-[bit](../../../../../bit.md) [binary string](../../../../../binary-string.md) as $A=a_{n-1}\cdots a_1a_0$, where each $a_i\in\{0,1\}$ and $a_{n-1}$ is most significant. Its [unsigned interpretation](../../../../../unsigned-interpretation-of-a-bit-string.md) and [two's complement](../../../../../two-s-complement.md) interpretation are

$$
\boxed{\operatorname{bin}(A)=\sum_{i=0}^{n-1}a_i2^i,\qquad
\operatorname{twoc}(A)=-a_{n-1}2^{n-1}+\sum_{i=0}^{n-2}a_i2^i.}
$$

Equivalently, $\operatorname{twoc}(A)=\operatorname{bin}(A)-a_{n-1}2^n$. The ranges are $0$ through $2^n-1$ and $-2^{n-1}$ through $2^{n-1}-1$, respectively. The same stored [bits](../../../../../bit.md) can therefore denote different [integers](../../../../../integer-split.md) depending on the chosen interpretation.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [Digital systems](../../digital-systems.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
