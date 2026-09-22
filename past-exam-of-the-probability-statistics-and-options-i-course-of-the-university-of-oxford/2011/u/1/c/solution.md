<h1 id="u/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At the left endpoint $f(-1)=36>0$. If $b=2$, the endpoint is exactly a root and the function above immediately returns $2$. For $2<b\leq4$, $f(b)<0$, so the first midpoint is $m=(b-1)/2$.

If $2<b<3$, then $1/2<m<1$ and $f(m)<0$. The first retained bracket is $[-1,m]$, containing only the root zero, so the iterates converge to zero. If $b=3$, the first midpoint is exactly the root one and is returned. If $3<b\leq4$, then $1<m\leq3/2$ and $f(m)>0$. The retained bracket is $[m,b]$, containing only the root two, so the iterates converge to two. Hence

$$
\boxed{\text{returned root}=\begin{cases}
2,&b=2,\\0,&2<b<3,\\1,&b=3,\\2,&3<b\leq4.
\end{cases}}
$$

This illustrates [root selection by bisection with multiple roots in the initial bracket](../../../../../root-selection-by-bisection-with-multiple-roots-in-the-initial-bracket.md): bisection guarantees a root, but which root it chooses depends discontinuously on the starting endpoint.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [U](../../../u.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
