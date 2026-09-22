<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Integrating the exact Galerkin energy identity gives

$$
\frac12|u_m(t)|^2
+\nu\int_0^t\|u_m(\tau)\|^2\,d\tau
=\frac12|P_mu_0|^2
\leq\frac12|u_0|^2.
$$

Thus one may take

$$
\boxed{
K_0(T)=|u_0|,
\qquad
K_1(T)=\frac{|u_0|}{\sqrt{2\nu}}}
$$

for the first two requested bounds; these constants happen not to grow with $T$.

The Galerkin equation and contractivity of $P_m$ on $V'$ give

$$
\left\|\frac{du_m}{dt}\right\|_{V'}
\leq\nu\|Au_m\|_{V'}
+\|B(P_Nu_m,u_m)\|_{V'}.
$$

Since $\|Au_m\|_{V'}=\|u_m\|$, part a gives

$$
\left\|\frac{du_m}{dt}\right\|_{V'}
\leq
\left(\nu+c\lambda_N^{1/4}|u_m|\right)\|u_m\|
\leq
\left(\nu+c\lambda_N^{1/4}|u_0|\right)\|u_m\|.
$$

Consequently

$$
\boxed{
\left\|\frac{du_m}{dt}\right\|_{L^2(0,T;V')}
\leq
K_0'(T)
:=
\left(\nu+c\lambda_N^{1/4}|u_0|\right)
\frac{|u_0|}{\sqrt{2\nu}}}.
$$

All three constants are independent of $m$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 359](../../../../paper-359-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
