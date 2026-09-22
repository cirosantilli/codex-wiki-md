<h1 id="7b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Inspection gives $y_1=x$ in the degree-one [Legendre differential equation](../../../../../../legendre-differential-equation.md). After division by $1-x^2$, $p=-2x/(1-x^2)$ and $e^{-\int p}=1/(1-x^2)$. On either side of zero, [reduction of order](../../../../../../reduction-of-order.md) therefore gives

$$
v'=\frac1{x^2(1-x^2)}=\frac1{x^2}+\frac1{1-x^2},\qquad v=-\frac1x+\operatorname{arctanh}x.
$$

A second solution is $y_2=x\operatorname{arctanh}x-1$. Although $v$ is singular at zero, the product $vy_1$ has a smooth continuation throughout $(-1,1)$. This illustrates [reduction of order across a zero of the known solution](../../../../../../reduction-of-order-across-a-zero-of-the-known-solution.md). Since $y_1(0)=0$, $y_1'(0)=1$, $y_2(0)=-1$ and $y_2'(0)=0$, the required coefficients are $1,-1$. Hence

$$
\boxed{y(x)=1+x-x\operatorname{arctanh}x=1+x-\frac x2\log\frac{1+x}{1-x},\qquad -1<x<1.}
$$

The [ordinary differential equation](../../../../../../ordinary-differential-equation.md) has regular coefficients near zero, so the resulting initial-value solution is unique and the removable singularity in the intermediate representation causes no ambiguity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7B](../../7b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
