<h1 id="section-b/b2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\Gamma_a(v)=(1-v^2/a^2)^{-1/2}$. The first proposed [Lorentz transformation](../../../../../lorentz-transformation.md) is

$$
x'=\Gamma_a(v)(x-vt),\qquad
t'=\Gamma_a(v)\left(t-\frac{vx}{a^2}\right).
$$

For the next transformation, write $\Gamma_b(u)=(1-u^2/b^2)^{-1/2}$ and substitute the first pair into $x''=\Gamma_b(u)(x'-ut')$ and $t''=\Gamma_b(u)(t'-ux'/b^2)$. The result is

$$
\begin{aligned}
x''&=\Gamma_a(v)\Gamma_b(u)
\left[\left(1+\frac{uv}{a^2}\right)x-(u+v)t\right],\\
t''&=\Gamma_a(v)\Gamma_b(u)
\left[\left(1+\frac{uv}{b^2}\right)t
-\left(\frac{v}{a^2}+\frac{u}{b^2}\right)x\right].
\end{aligned}
$$

The direct transformation between $S$ and $S''$ must belong to the same standard boost family with the same calibration of space and time units. Such a transformation has one common factor multiplying the coefficient of $x$ in $x''$ and that of $t$ in $t''$. Equality of these coefficients for generic $uv\ne0$ requires

$$
1+\frac{uv}{a^2}=1+\frac{uv}{b^2},\qquad
\boxed{a^2=b^2.}
$$

The case $uv=0$ alone cannot constrain the scales, but a transformation law must work for arbitrary successive boosts. Once the scales agree, their composed [velocity](../../../../../velocity.md) is $V=(u+v)/(1+uv/a^2)$ and the common factor is $\Gamma_a(V)$. This establishes the [universality of an invariant speed under boost composition](../../../../../universality-of-an-invariant-speed-under-boost-composition.md) within the proposed family.

**Finiteness needs physical input.** Sending $a^2$ to infinity gives the consistent [Galilean transformation](../../../../../galilean-transformation.md) $x'=x-vt$, $t'=t$. Its boosts compose with $V=u+v$ and satisfy a relativity principle. Thus the composition calculation itself does _not_ prove that $a^2$ cannot be infinite. The finite propagation speed of light in vacuum and its invariance, supplied by the second of the [postulates of special relativity](../../../../../postulates-of-special-relativity.md), rule out this limit for physical spacetime. Under a [Galilean transformation](../../../../../galilean-transformation.md), a ray with laboratory speed $c$ would have speed $c-v$ in the moving frame, in conflict with that postulate.

Finally, the common invariant scale must be identified with the physical [speed of light](../../../../../speed-of-light.md), rather than an arbitrary speed measured in one frame. Requiring a ray $x=ct$ also to obey $x'=ct'$ gives

$$
\frac{c-v}{1-vc/a^2}=c
\quad\Longrightarrow\quad a^2=c^2\qquad(v\ne0).
$$

Hence **the physical scale is $a=c$**, taking the positive speed. The postulate about light identifies and requires a finite invariant scale; closure alone only establishes its universality. This distinction is necessary for a logically valid answer to the question's request to exclude infinity.

## ↑ Ancestors (14)

1. [B](../b.md)
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
