<h1 id="b/6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Since $f(0)=0$, the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) gives $f=Tf'$, with the same oriented integral on the negative half-interval. Set $h(t)=t^2$. The adjoint calculation gives the real-valued function

$$
\boxed{g(t)=(T^*h)(t)=\begin{cases}(\pi^3-t^3)/3,&0<t\leq\pi,\\-(\pi^3+t^3)/3,&-\pi<t<0.\end{cases}}
$$

Choose any value at zero. This function is bounded and hence belongs to $L^2(-\pi,\pi]$. Since it is real, the [adjoint operator](../../../../../adjoint-operator.md) identity yields

$$
\int_{-\pi}^{\pi}t^2f(t)dt=\langle Tf',h\rangle=\langle f',T^*h\rangle=\int_{-\pi}^{\pi}g(t)f'(t)dt.
$$

One can also check this by [integration by parts](../../../../../integration-by-parts.md) separately on each half-interval: $g'=-t^2$, $g(\pm\pi)=0$, and the two possible jump terms at zero vanish because $f(0)=0$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
