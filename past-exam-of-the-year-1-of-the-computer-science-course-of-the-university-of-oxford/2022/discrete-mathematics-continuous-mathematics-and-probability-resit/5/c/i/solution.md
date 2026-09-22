<h1 id="5/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $q(x)=x^TAx$ and $t(x)=x^Tb$. The [product rule](../../../../../../product-rule.md) gives

$$
\boxed{\nabla h(x)=2t(x)Ax+q(x)b.}
$$

Differentiate each term. The [derivative](../../../../../../derivative.md) of $2tAx$ is $2(Ax)b^T+2tA$, while that of $qb$ is $2b(Ax)^T$. Hence

$$
\boxed{H_h(x)=2(x^Tb)A+2(Ax)b^T+2b(Ax)^T.}
$$

The last two terms are transposes of each other, so this [Hessian matrix](../../../../../../hessian-matrix.md) is symmetric, as expected.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Discrete mathematics, continuous mathematics and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
