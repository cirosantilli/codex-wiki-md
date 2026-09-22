<h1 id="b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the system as $U_x+A(U)U_y=0$ with $U=(u,v)^T$ and

$$
A=\begin{pmatrix}v&u\\1&v\end{pmatrix},\qquad\det(A-\lambda I)=(v-\lambda)^2-u.
$$

Its two [characteristic speeds](../../../../../characteristic-speed.md) are $\lambda_\pm=v\pm\sqrt u$, so it is **strictly hyperbolic precisely when $u>0$**. At $u=0$ they coincide and the matrix is not diagonalizable; for $u<0$ the speeds are nonreal.

For $u>0$ define $R_\pm=v\pm2\sqrt u$ and $D_\pm=\partial_x+(v\pm\sqrt u)\partial_y$. Substitution from the two differential equations gives

$$
\begin{aligned}
D_\pm R_\pm
&=v_x+(v\pm\sqrt u)v_y
\ \pm u^{-1/2}[u_x+(v\pm\sqrt u)u_y]\\
&=(-u_y\pm\sqrt u\,v_y)\pm u^{-1/2}(\pm\sqrt u\,u_y-uv_y)=0.
\end{aligned}
$$

Therefore

$$
\boxed{v\pm2\sqrt u\text{ is constant on curves }\frac{dy}{dx}=v\pm\sqrt u.}
$$

These are the two [Riemann invariants](../../../../../riemann-invariant.md); their constancy applies within smooth regions, not across a [shock](../../../../../shock-wave.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
