<h1 id="6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [administrative censoring with uniform entry](../../../../../../../administrative-censoring-with-uniform-entry.md), let entry time $A\sim\operatorname{Uniform}(\tau_a,\tau_b)$. Then $C=\tau_c-A$ has the [uniform distribution](../../../../../../../continuous-uniform-distribution.md) on $[\ell,r]$, where $\ell=\tau_c-\tau_b$, $r=\tau_c-\tau_a$, and $d=r-\ell=\tau_b-\tau_a$. **Its density and survivor function** are

$$
\boxed{g_C(t)=\begin{cases}1/d,&\ell<t<r,\\0,&\text{otherwise},\end{cases}\qquad G(t)=\begin{cases}1,&0\le t<\ell,\\(r-t)/d,&\ell\le t<r,\\0,&t\ge r.\end{cases}}
$$

Dividing density by survival and integrating gives **the censoring hazard and integrated hazard**:

$$
\boxed{h_C(t)=\begin{cases}0,&0\le t<\ell,\\1/(r-t),&\ell\le t<r,\end{cases}\qquad H_C(t)=\begin{cases}0,&0\le t<\ell,\\\log\frac{d}{r-t},&\ell\le t<r,\\+\infty,&t\ge r.\end{cases}}
$$

The [hazard function](../../../../../../../hazard-function.md) is undefined once no uncensored individuals remain. As $t\uparrow r$, it diverges like $1/(r-t)$ and the [cumulative hazard function](../../../../../../../cumulative-hazard-function.md) diverges logarithmically. This reflects the certainty of administrative censoring by the longest possible follow-up time, not dependence of censoring on the event process.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
