<h1 id="a/2/b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the complex $L^2$ [inner product](../../../../../../inner-product-split.md) $\langle f,g\rangle=\int_0^\pi\overline f g$, linear in its second argument. Exchanging the order of integration gives

$$
\langle f,Lg\rangle=\int_0^\pi\left[\int_0^\pi\overline{f(x)}k(x,t)\,dx\right]g(t)\,dt.
$$

Since the [kernel](../../../../../../kernel-of-a-linear-map-split.md) is real, the [adjoint operator](../../../../../../adjoint-operator.md) is therefore

$$
\boxed{L^*f(t)=\int_0^\pi k(x,t)f(x)\,dx,}
$$

or, renaming variables, $L^*f(x)=\int_0^\pi k(t,x)f(t)\,dt$. [Continuity](../../../../../../continuous-function.md) of the [kernel](../../../../../../kernel-of-a-linear-map-split.md) on the compact integration square justifies these integrals and the exchange.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the differential equations and applications course of the University of Oxford](../../../../../split.md)
7. [Differential equations and applications course of the University of Oxford](../../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
