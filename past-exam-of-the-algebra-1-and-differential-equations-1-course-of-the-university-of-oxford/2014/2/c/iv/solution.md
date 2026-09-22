<h1 id="2/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The fixed points of reciprocal root pairing are $1$ and $-1$, so part (iii) alone does not establish their parity. Use the polynomial identity itself.

Write $P(x)=(x-1)^rA(x)$, where $A(1)\ne0$ and allow $r=0$ if one is not a root. After substituting in $P(x)=x^{2m}P(1/x)$ and canceling $(x-1)^r$ away from $x=1$, obtain

$$
A(x)=(-1)^r x^{2m-r}A(1/x).
$$

Letting $x\to1$ yields $A(1)=(-1)^rA(1)$, so $r$ is even.

Similarly write $P(x)=(x+1)^sB(x)$ with $B(-1)\ne0$. This time cancellation gives $B(x)=x^{2m-s}B(1/x)$. Letting $x\to-1$ yields $B(-1)=(-1)^{2m-s}B(-1)$, so $s$ is even. Thus

$$
\boxed{\text{Both }1\text{ and }-1\text{ have even algebraic multiplicity.}}
$$

The conclusion includes multiplicity zero. It is a consequence of the reciprocal identity in even degree, which is stronger at these fixed points than just pairing the roots.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
