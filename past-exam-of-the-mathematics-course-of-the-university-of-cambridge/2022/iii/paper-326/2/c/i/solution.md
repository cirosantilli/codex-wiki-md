<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The objective separates by coordinates, so minimize

$$
h_i(z)=\frac12(z-x_i)^2+\lambda|z|.
$$

The [subgradient optimality condition](../../../../../../../subgradient-optimality-condition.md) is

$$
0\in z-x_i+\lambda\,\partial|z|.
$$

For $z>0$ this gives $z=x_i-\lambda$, valid when $x_i>\lambda$; for $z<0$ it gives $z=x_i+\lambda$, valid when $x_i<-\lambda$. At $z=0$, the condition is $x_i\in[-\lambda,\lambda]$. Therefore the shrinkage operator is the [soft-thresholding operator](../../../../../../../soft-thresholding.md)

$$
[\psi_\lambda(x)]_i
=\begin{cases}
x_i-\lambda,&x_i>\lambda,\\
0,&-\lambda\leq x_i\leq\lambda,\\
x_i+\lambda,&x_i<-\lambda.
\end{cases}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
