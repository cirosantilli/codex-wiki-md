<h1 id="b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the time integral $I_t=\int_0^tW_sds$, [Fubini's theorem](../../../../../fubini-s-theorem.md) and $\mathbb EW_s=0$ give $\mathbb EI_t=0$. Brownian covariance is $\mathbb E[W_uW_v]=\min(u,v)$, so

$$
\operatorname{Var}(I_t)=\int_0^t\int_0^t\min(u,v)\,du\,dv
=2\int_0^t\int_0^v u\,du\,dv=\int_0^t v^2dv.
$$

Consequently

$$
\boxed{\mathbb EI_t=0,\qquad\operatorname{Var}(I_t)=t^3/3.}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
