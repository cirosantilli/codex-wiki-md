<h1 id="14b/solution">Solution</h1>

↑ **Parent:** [14B](../14b.md)

Let the three orbit points be $a<b<c$. Up to reflection of the interval, their images are $F(a)=b,F(b)=c,F(c)=a$. Set $I=[a,b]$ and $J=[b,c]$. [Continuity](../../../../../continuous-function.md) and the [intermediate value theorem](../../../../../intermediate-value-theorem.md) imply the covering relations

$$
F(I)\supseteq J,\qquad F(J)\supseteq I\cup J.
$$

We first prove the needed interval-covering principle using the permitted pullback fact. If a cyclic list of closed intervals $I_0,\ldots,I_{n-1},I_n=I_0$ obeys $F(I_j)\supseteq I_{j+1}$, pull back successively from the end to obtain a closed interval $K\subseteq I_0$ with $F^n(K)=I_0$ and $F^j(K)\subseteq I_j$. Since $F^n(K)\supseteq K$, the [intermediate value theorem](../../../../../intermediate-value-theorem.md) gives a [fixed point](../../../../../fixed-point.md) of $F^n$ in $K$: choose preimages of the two endpoints of $K$, which give opposite weak signs of $F^n(x)-x$, irrespective of their order. This point realizes the cyclic itinerary.

For $n\geq2$, use the word $I J^{n-1}$. It obeys the covering relations and therefore yields a point with period dividing $n$. A point away from the shared endpoint $b$ has an unambiguous itinerary, and this word has exactly one $I$ per cycle; it cannot be a repetition of a shorter word. Its least period is consequently $n$. If an orbit touches $b$, it is the original three-cycle. That realizes the case $n=3$ itself. It cannot realize any of the other words: for $n$ not divisible by three it is not fixed by $F^n$, and for a multiple of three larger than three it visits $a\in I\setminus J$ more than once, contradicting the itinerary. Thus the construction works for every $n\geq2$. For $n=1$, $F(J)\supseteq J$ and the same fixed-point argument gives a [fixed point](../../../../../fixed-point.md). This proves [period three implies all periods](../../../../../period-three-implies-all-periods.md): **there is an orbit of every positive least period**.

For the [two five-cycles forced by a three-cycle](../../../../../two-five-cycles-forced-by-a-three-cycle.md), use the two cyclic words $I J J J J$ and $I J I J J$. Both are admissible. Their points cannot be endpoints from the three-cycle, and because five is prime and the words use both intervals, each has least period five. Their itineraries have respectively one and two visits to the interior of $I$; cyclically shifting the starting point cannot change this count. Hence they give **at least two distinct period-five orbits**.

## ↑ Ancestors (10)

1. [14B](../14b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
