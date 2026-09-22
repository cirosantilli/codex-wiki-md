<h1 id="b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $v\leq t$, the two stock paths agree, so their geometric averages agree. For $v>t$, the future log-price is

$$
\log\widetilde S_u=\log S_t+(r-\sigma^2/2)(u-t)+\sigma(W_u-W_t).
$$

Split the average's log-integral into $[0,t]$ and $[t,v]$. The first part is $t\log A_t$, while integration of the displayed formula gives

$$
v\log\widetilde A_v=t\log A_t+(v-t)\log S_t+\tfrac12(r-\sigma^2/2)(v-t)^2
+\sigma\int_t^v(W_u-W_t)du.
$$

Dividing by $v$ and exponentiating proves

$$
\boxed{\widetilde A_v=A_t^{t/v}S_t^{(v-t)/v}
\exp\left[\left(r-\frac{\sigma^2}{2}\right)\frac{(v-t)^2}{2v}
+\frac\sigma v\int_t^v(W_u-W_t)du\right]\quad(v>t).}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
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
