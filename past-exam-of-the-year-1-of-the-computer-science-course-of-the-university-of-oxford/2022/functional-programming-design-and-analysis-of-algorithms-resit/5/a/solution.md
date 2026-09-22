<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the first [recurrence relation](../../../../../recurrence-relation.md), the [master theorem](../../../../../master-theorem.md) compares $n^2$ with $n^{\log_2 6}$. Since $2<\log_2 6$, the recursive leaves dominate and the answer is **$\Theta(n^{\log_2 6})$**. More explicitly, the work at depth $j$ is $n^2(6/4)^j$, a growing [geometric series](../../../../../geometric-series.md) that stops at depth $\log_2 n-O(1)$, where its sum has that order.

For the second [recurrence relation](../../../../../recurrence-relation.md), each step subtracts two and adds one until reaching a base case. For integral $n>4$ there are $\lceil(n-4)/2\rceil$ steps, so $T(n)=1+\lceil(n-4)/2\rceil$ and the answer is **$\Theta(n)$**.

The third set of printed requirements is inconsistent. The specified base values and its [recurrence relation](../../../../../recurrence-relation.md) give $T(n)=1$ identically, as [strong induction](../../../../../strong-induction.md) immediately verifies: $4\cdot1-4\cdot1+1=1$. In particular $T(8)=1$, while the extra condition demands $T(8)>2T(4)=2$. Thus **no [function](../../../../../function-split.md) satisfies all the printed conditions**. Dropping that extra inequality gives **$\Theta(1)$**.

The likely intended growth calculation can nevertheless be made precise, without treating it as a solution of the contradictory data. On dyadic arguments put $U_j=T(2^j)$. Its equation has the general form

$$
U_j=1+(A+Bj)2^j,
$$

because $U_j-1$ has characteristic equation $(r-2)^2=0$. The printed values $U_1=U_2=1$ force $A=B=0$. With suitably different initial values, the condition $U_j>2U_{j-1}$ for arbitrarily large $j$ instead requires $B2^j-1>0$, hence $B>0$ and $U_j=\Theta(j2^j)$, or $T(n)=\Theta(n\log n)$. That last order describes corrected initial data, not the paper as printed. All three bullets belong to this single marked part.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
