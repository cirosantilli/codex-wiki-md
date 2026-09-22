<h1 id="9/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $S_0>0$ and scale by the initial susceptible count:

$$
\boxed{u=\frac S{S_0},\quad v=\frac I{S_0},\quad w=\frac R{S_0},\quad\tau=\gamma t,\quad
v_0=\frac{I_0}{S_0},\quad\mathcal R_0=\frac{\beta S_0}{\gamma}.}
$$

Substitution into the [SIR model equations](../../../../../sir-model-equations.md) gives

$$
\frac{du}{d\tau}=-\mathcal R_0uv,\qquad
\frac{dv}{d\tau}=(\mathcal R_0u-1)v,\qquad
\frac{dw}{d\tau}=v.
$$

The initial data become $u(0)=1$, $v(0)=v_0$, $w(0)=0$. The conserved total is $u+v+w=1+v_0$, since the scaling is by $S_0$, not by $S_0+I_0$. With this normalization, $\mathcal R_0$ is the reproduction ratio at the initial susceptible level.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
