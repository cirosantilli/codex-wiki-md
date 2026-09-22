<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the unheaded existence request, use the [probabilistic method](../../../../../probabilistic-method.md). Choose every value $f(x,y)$ independently and uniformly from $\{-1,1\}$. For a rectangle with $x\ne x'$ and $y\ne y'$, its four entries are distinct, so independence and the zero mean of each sign give expectation zero for their product. If $x=x'$ or $y=y'$, the product is identically one. The number of ordered rectangles in this union of diagonal cases is

$$
mn^2+m^2n-mn.
$$

Therefore the [random sign rectangle fourth moment](../../../../../random-sign-rectangle-fourth-moment.md) has expectation

$$
\mathbb E Q(f)=\frac1m+\frac1n-\frac1{mn}.
$$

Some sign function has $Q(f)$ at most this expectation. Applying the bound in part (a) to that same function gives the simultaneous choices

$$
\boxed{c_1=\frac1m+\frac1n-\frac1{mn},\qquad c_2=\left(\frac1m+\frac1n-\frac1{mn}\right)^{1/4}.}
$$

Both constants tend to zero whenever both dimensions tend to infinity, without any assumption on their relative rates of growth.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
