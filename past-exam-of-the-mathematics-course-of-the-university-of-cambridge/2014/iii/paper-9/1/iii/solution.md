<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Apply the [Ramsey theorem for r-sets](../../../../../../ramsey-s-theorem.md), proved in part (i), with $r=4$ to the even positive integers. Colour the four-set $\{a,b,c,d\}$ with $a<b<c<d$ by $\chi(a+b+2c+2d)$. This gives increasing even integers $u_1<u_2<\cdots$ such that every such four-index expression has one colour $\gamma$.

For the [simultaneous coefficient patterns from a homogeneous four-set colouring](../../../../../../simultaneous-coefficient-patterns-from-a-homogeneous-four-set-colouring.md), set

$$
\boxed{x_i=u_{2i-1}+u_{2i},\qquad y_i=\frac{u_1+u_2}{2}+2u_{i+2}.}
$$

Both sequences consist of positive integers and are strictly increasing. The evenness ensures that the shared half-prefix in $y_i$ is integral. For $i<j$, the two types of sum are

$$
x_i+2x_j=u_{2i-1}+u_{2i}+2u_{2j-1}+2u_{2j},
$$

and

$$
y_i+y_j=u_1+u_2+2u_{i+2}+2u_{j+2}.
$$

In both expressions the four indices are strictly ordered, so their colour is $\gamma$. Therefore **the union of the two families is monochromatic**. The common half-prefix is what permits the second family to use the same coefficient pattern despite having different generating variables.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
