<h1 id="section-c/c11/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Start with the fundamental relation at fixed material amount, $dU=T\,dS-p\,dV$, and expand [entropy](../../../../../../entropy-split.md) in independent variables $T,V$:

$$
dS=\left(\frac{\partial S}{\partial T}\right)_VdT
+\left(\frac{\partial S}{\partial V}\right)_TdV
=\frac{C_V}{T}dT+\left(\frac{\partial p}{\partial T}\right)_VdV.
$$

The last equality uses the supplied [Maxwell relation](../../../../../../maxwell-relations.md). Consequently

$$
dU=C_V\,dT+\left[T\left(\frac{\partial p}{\partial T}\right)_V-p\right]dV.
$$

For the [excluded-volume ideal gas](../../../../../../excluded-volume-ideal-gas.md), $(\partial p/\partial T)_V=R/(V-b)=p/T$, so the bracket vanishes:

$$
\boxed{\left(\frac{\partial U}{\partial V}\right)_T=0,
\qquad U=U(T),\qquad dU=C_V\,dT.}
$$

Once $U$ depends only on [temperature](../../../../../../temperature-split.md), $C_V=dU/dT$ cannot depend on [volume](../../../../../../volume-thermodynamics.md) either. Its stipulated [temperature](../../../../../../temperature-split.md) independence therefore makes it a constant, giving $U=C_VT+U_*$ with arbitrary [energy](../../../../../../energy-split.md) reference $U_*$. [Excluded volume](../../../../../../excluded-volume.md) changes the [pressure](../../../../../../pressure-split.md) without adding the volume-dependent attractive [internal energy](../../../../../../internal-energy-split.md) that a more general interacting-gas model might have.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [C11](../../c11.md)
3. [Section C](../../../section-c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
