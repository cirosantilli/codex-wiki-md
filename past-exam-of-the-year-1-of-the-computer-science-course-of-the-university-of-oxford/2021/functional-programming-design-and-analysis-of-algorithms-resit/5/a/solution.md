<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

There are three unnumbered cases inside this leaf.

For the nine-child recurrence, a [recursion](../../../../../recursion-computer-science.md) tree has $9^j$ subproblems of size about $n/3^j$. There are $\Theta(n^2)$ constant-size leaves, and the total unit work over earlier levels is a geometric sum of the same order. Hence **$T(n)=\Theta(n^2)$**. This is also the first case of the [master theorem](../../../../../master-theorem.md), since $\log_3 9=2$ and the additive work is constant.

For the decrementing recurrence, summing from the supplied base at three gives

$$
T(n)=1+\sum_{j=4}^{n}j=\frac{n(n+1)}2-5\quad(n\geq3),
$$

so **$T(n)=\Theta(n^2)$** here as well. Values at the smaller base indices remain one as specified.

For the recurrence that squares its recursive result, [set](../../../../../set-split.md) $S(n)=\log_2 T(n)$. Then $S(n)=1+2S(\lfloor n/2\rfloor)$ above the base range. Let

$$
d(n)=\min\{j\geq0:\lfloor n/2^j\rfloor\leq3\}=\max(0,\lfloor\log_2 n\rfloor-1)\quad(n\geq1).
$$

After $d$ expansions, $S(n)=1+2+\cdots+2^{d-1}=2^d-1$, giving the exact answer

$$
\boxed{T(n)=2^{\,2^{d(n)}-1}.}
$$

For powers of two $n\geq4$ this is $2^{n/2-1}$. For arbitrary [positive integer](../../../../../positive-integer.md) $n$, the exact values form plateaux: $T(4)=\cdots=T(7)=2$, while $T(8)=\cdots=T(15)=8$. In general **$T(n)=2^{\Theta(n)}$**. It is not $\Theta(2^{n/2})$ uniformly over [integer](../../../../../integer-split.md) $n$: near the top of a plateau the exponent is closer to $n/4$. Keeping the [integer](../../../../../integer-split.md) halving is essential; the ordinary linear [master theorem](../../../../../master-theorem.md) does not apply to squaring $T$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
