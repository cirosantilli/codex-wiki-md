<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By [Euclidean division](../../../../../euclidean-division.md), write $a=qn+r$ and $b=sn+t$, with [integers](../../../../../integer-split.md) $q,s$ and $0\leq r,t<n$. The hypothesis is $a\equiv b\pmod n$. Apply the addition rule from part (b)(i) with $-qn\equiv-sn\equiv0\pmod n$ to obtain

$$
r=a-qn\equiv b-sn=t\pmod n.
$$

Therefore $n\mid r-t$. But $-n<r-t<n$, and the only multiple of $n$ in that interval is zero. Hence

$$
\boxed{r=t,}
$$

so the two [remainders](../../../../../remainder.md) agree.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
