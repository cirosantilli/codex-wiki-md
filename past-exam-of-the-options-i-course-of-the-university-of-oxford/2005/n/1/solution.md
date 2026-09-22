<h1 id="n/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

States $i,j$ communicate when each is accessible from the other: $(P^m)_{ij}>0$ and $(P^n)_{ji}>0$ for some nonnegative integers $m,n$. The communicating classes are

$$
\boxed{\{1,4\}\text{ closed},\qquad\{2,3,5\}\text{ open},\qquad\{6\}\text{ closed}.}
$$

Indeed $1$ and $4$ move only between themselves; $2\to5\to3\to2$ links the second class, but it has exits to $1,4,6$ and no return from the closed classes; state 6 is absorbing.

Let $h_i$ be the [probability](../../../../probability.md) of ever reaching 6 from state $i$. Then $h_1=h_4=0$, $h_6=1$, and first-step conditioning gives

$$
h_2=\frac34h_5,\qquad h_3=\frac12h_2+\frac12h_3,\qquad h_5=\frac14h_3+\frac14h_4+\frac14h_5+\frac14.
$$

Thus $h_3=h_2=3h_5/4$ and $3h_5=h_3+1$, giving $h_5=4/9$. Therefore

$$
\boxed{\mathbb P_3(\text{eventual absorption in }6)=\frac13.}
$$

## ↑ Ancestors (12)

1. [1](../1.md)
2. [N](../../n.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
