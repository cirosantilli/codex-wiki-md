<h1 id="section-b/b2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mathbf a=d\mathbf u/dt$ denote coordinate [acceleration](../../../../../acceleration.md) and use $A^\mu$ for [four-acceleration](../../../../../four-acceleration.md), to distinguish these two objects. Applying the [chain rule](../../../../../chain-rule.md) to the [Lorentz factor](../../../../../lorentz-factor.md) gives

$$
\frac{d\gamma_u}{dt}
=-\frac12\left(1-\frac{\mathbf u\cdot\mathbf u}{c^2}\right)^{-3/2}
\left(-\frac{2\mathbf u\cdot\mathbf a}{c^2}\right)
=\boxed{\frac{\gamma_u^3\mathbf u\cdot\mathbf a}{c^2}}.
$$

Since $dt/d\tau=\gamma_u$, differentiation of the [four-velocity](../../../../../four-velocity.md) $U^\mu=\gamma_u(c,\mathbf u)$ with respect to [proper time](../../../../../proper-time.md) yields

$$
A^\mu=\gamma_u\frac{d}{dt}\big[\gamma_u(c,\mathbf u)\big]
=\boxed{\left(\frac{\gamma_u^4\mathbf u\cdot\mathbf a}{c},\
\gamma_u^2\mathbf a+\frac{\gamma_u^4(\mathbf u\cdot\mathbf a)\mathbf u}{c^2}\right)}.
$$

This is also $\gamma_u^2[\gamma_u^2(\mathbf u\cdot\mathbf a)/c,\ \mathbf a+\gamma_u^2(\mathbf u\cdot\mathbf a)\mathbf u/c^2]$, as required.

The invariant [Minkowski norm](../../../../../minkowski-norm.md) of the [four-velocity](../../../../../four-velocity.md) is $U^\mu U_\mu=c^2$. Differentiating this identity gives $U^\mu A_\mu=0$. In the instantaneous [rest frame](../../../../../rest-frame.md), $U^\mu=(c,\mathbf0)$, so $A^0=0$ and the spatial components equal the physically experienced [proper acceleration](../../../../../proper-acceleration.md) $\boldsymbol\alpha$. Therefore $\alpha^2=-A^\mu A_\mu$ in the $+---$ [metric signature](../../../../../metric-signature.md).

For a direct calculation, put $q=\mathbf u\cdot\mathbf a$ and expand the temporal and spatial squares:

$$
\begin{aligned}
\alpha^2
&=\left|\gamma_u^2\mathbf a+\frac{\gamma_u^4q\mathbf u}{c^2}\right|^2
-\frac{\gamma_u^8q^2}{c^2}\\
&=\gamma_u^4a^2+\frac{2\gamma_u^6q^2}{c^2}
+\frac{\gamma_u^8q^2}{c^2}\left(\frac{u^2}{c^2}-1\right)\\
&=\boxed{\gamma_u^4\mathbf a\cdot\mathbf a+\frac{\gamma_u^6(\mathbf u\cdot\mathbf a)^2}{c^2}}.
\end{aligned}
$$

The last step uses $1-u^2/c^2=\gamma_u^{-2}$. This [proper acceleration from coordinate velocity and acceleration](../../../../../proper-acceleration-from-coordinate-velocity-and-acceleration.md) also reads $\alpha^2=\gamma_u^6a_\parallel^2+\gamma_u^4a_\perp^2$, providing the familiar one-dimensional limit $\alpha=\gamma_u^3|a_\parallel|$. Each expression has units $\mathrm{m^2\,s^{-4}}$.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [B2](../../b2.md)
3. [Section B](../../../section-b.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the relativity course of the University of Cambridge](../../../../split.md)
6. [Relativity course of the University of Cambridge](../../../../../relativity-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
