<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The printed split uses $n$ while naming the current length $m=j-i$. For the intended [stooge sort](../../../../../stooge-sort.md), read that split as $k=\lfloor m/3\rfloor$ at every recursive call. Keeping one fixed original $n$ instead is not the standard algorithm and does not generally sort correctly.

The three recursive calls then each have length $m-\lfloor m/3\rfloor=\lceil2m/3\rceil$, and all other work is constant. Thus

$$
\boxed{T(m)=3T(\lceil2m/3\rceil)+\Theta(1)\quad(m>2),\qquad T(m)=\Theta(1)\quad(m\leq2).}
$$

A version of the [master theorem](../../../../../master-theorem.md) sufficient here states: if $T(n)=aT(\lceil n/b\rceil)+f(n)$ with constants $a\geq1,b>1$, fixed-size base cases and $f(n)=O(n^{\log_b a-\epsilon})$ for some $\epsilon>0$, then $T(n)=\Theta(n^{\log_b a})$, provided the recursive sizes shrink above the base threshold. Apply it with $a=3,b=3/2,f=\Theta(1)$ to obtain

$$
\boxed{T(n)=\Theta\!\left(n^{\log_{3/2}3}\right),\qquad \log_{3/2}3\approx2.7095.}
$$

The rounded size is important for correctness; it does not change this asymptotic exponent.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
