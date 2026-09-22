<h1 id="p/p3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The difference $d=p-q$ has $d(x_i)=d'(x_i)=0$ at every node. [Rolle's theorem](../../../../../rolle-theorem.md) supplies an additional zero of $d'$ in each of the $n$ open intervals between successive nodes. Together with the $n+1$ nodal derivative zeros, these are $2n+1$ distinct zeros of $d'$, including the two endpoints. But $d'$ is a polynomial of degree at most $2n$, so it is identically zero. Since $d(x_0)=0$, $d$ is also identically zero.

Thus **the interpolation polynomial is unique**. Once $d'=0$ identically, it indeed has arbitrarily many zeros in the open interval as requested. The initial Rolle count naturally includes the endpoints, rather than initially supplying $2n+1$ open-interval zeros. Equivalently, every node is a double root of $d$, so a nonzero difference would be divisible by the degree-$2n+2$ polynomial $\prod_i(x-x_i)^2$, exceeding its allowed degree.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [P3](../../p3.md)
3. [P](../../../p.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
