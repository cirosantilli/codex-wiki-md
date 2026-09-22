<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

By the assumed [spherical symmetry](../../../../../../../spherical-symmetry.md) of the [electric potential](../../../../../../../electric-potential.md), the [electric field](../../../../../../../electric-field-split.md) is radial: $\mathbf E=E_r(r)\mathbf e_r$ for $r>0$. On a [sphere](../../../../../../../sphere.md) of radius $r$, [Gauss's law](../../../../../../../gauss-s-law.md) therefore reads

$$
4\pi r^2E_r(r)=\frac{Q(r)}{\epsilon_0},\qquad
Q(r)=4\pi\int_0^r\rho(s)s^2\,ds.
$$

Put $R=a(1+\delta)$. For $r<a$, the enclosed [electric charge](../../../../../../../electric-charge-split.md) is $4\pi\rho_0r^3/3$. In the [spherical shell](../../../../../../../spherical-shell.md), the factor $s^2$ in the [volume element](../../../../../../../volume-element.md) cancels $s^{-2}$ in the [charge density](../../../../../../../charge-density.md), so

$$
\begin{aligned}
Q(r)&=\frac{4\pi\rho_0a^3}{3}
+\frac{4\pi\rho_0a^2}{\delta}\int_a^rh'(s/a)\,ds\\
&=4\pi\rho_0a^3\left[\frac13+\frac{h(r/a)-h(1)}{\delta}\right].
\end{aligned}
$$

It follows that

$$
\boxed{\mathbf E(\mathbf r)=\begin{cases}
\dfrac{\rho_0}{3\epsilon_0}\mathbf r,&0\leq r<a,\\
\dfrac{\rho_0a^3}{\epsilon_0r^2}\left[\dfrac13+\dfrac{h(r/a)-h(1)}{\delta}\right]\mathbf e_r,&a\leq r<R,\\
\dfrac{\rho_0a^3}{\epsilon_0r^2}\left[\dfrac13+\dfrac{h(1+\delta)-h(1)}{\delta}\right]\mathbf e_r,&r\geq R.
\end{cases}}
$$

At the origin the first formula gives $\mathbf E=\mathbf0$ without needing a radial [unit vector](../../../../../../../unit-vector.md). At both shell interfaces the adjacent formulas agree: for every fixed $\delta>0$, there is no [surface charge](../../../../../../../surface-charge.md) concentrated on either [sphere](../../../../../../../sphere.md), and the [electric field](../../../../../../../electric-field-split.md) is continuous there. No sign restriction on $h'$ has been assumed, so the shell [charge density](../../../../../../../charge-density.md) and the radial [electric field](../../../../../../../electric-field-split.md) can be negative.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
