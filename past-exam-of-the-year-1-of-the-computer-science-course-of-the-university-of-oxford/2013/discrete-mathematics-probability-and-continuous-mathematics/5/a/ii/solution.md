<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a [partial fraction decomposition](../../../../../../partial-fraction-decomposition.md), write

$$
\frac4{(x-1)^2(x+1)}=\frac A{x-1}+\frac B{(x-1)^2}+\frac C{x+1}.
$$

Multiplying by $(x-1)^2(x+1)$ gives $4=A(x^2-1)+B(x+1)+C(x-1)^2$. Setting $x=1,-1$ gives $B=2,C=1$, and comparing the coefficient of $x^2$ gives $A=-1$. Thus

$$
f(x)=-\frac1{x-1}+\frac2{(x-1)^2}+\frac1{x+1}.
$$

Integrating each term gives the [antiderivative](../../../../../../antiderivative.md)

$$
\boxed{\int f(x)\,dx=\log\left|\frac{x+1}{x-1}\right|-\frac2{x-1}+C.}
$$

The [constant of integration](../../../../../../constant-of-integration.md) can be chosen independently on each interval separated by $-1$ and $1$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
