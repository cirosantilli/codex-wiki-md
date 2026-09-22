<h1 id="12c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $r=|\boldsymbol r_1-\boldsymbol r_2|$ and $\widehat{\boldsymbol r}=(\boldsymbol r_1-\boldsymbol r_2)/r$. A differentiable central [potential energy](../../../../../../potential-energy.md) gives the internal [forces](../../../../../../force.md)

$$
\boldsymbol F_{12}=-\nabla_{\boldsymbol r_1}U=-U'(r)\widehat{\boldsymbol r},\qquad
\boldsymbol F_{21}=-\nabla_{\boldsymbol r_2}U=+U'(r)\widehat{\boldsymbol r}.
$$

There are no external [forces](../../../../../../force.md). Differentiating the total [kinetic energy](../../../../../../kinetic-energy.md) and using [Newton's second law](../../../../../../newton-s-second-law.md) therefore gives

$$
\begin{aligned}
\frac{dT}{dt}
&=m_1\boldsymbol v_1\cdot\dot{\boldsymbol v}_1
+m_2\boldsymbol v_2\cdot\dot{\boldsymbol v}_2\\
&=\boldsymbol F_{12}\cdot\boldsymbol v_1+
\boldsymbol F_{21}\cdot\boldsymbol v_2\\
&=-U'(r)\widehat{\boldsymbol r}\cdot(\boldsymbol v_1-\boldsymbol v_2).
\end{aligned}
$$

Since $\dot r=\widehat{\boldsymbol r}\cdot(\boldsymbol v_1-\boldsymbol v_2)$, the last expression is $-U'(r)\dot r=-dU/dt$. Thus

$$
\boxed{\frac{dT}{dt}+\frac{dU}{dt}=0,\qquad T+U=\mathrm{constant}.}
$$

This conserves total [mechanical energy](../../../../../../mechanical-energy.md), including the [kinetic energy](../../../../../../kinetic-energy.md) of centre-of-mass motion, not merely the relative [kinetic energy](../../../../../../kinetic-energy.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [12C](../../12c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
