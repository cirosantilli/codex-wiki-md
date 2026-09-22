<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Complete the square in the [dispersion relation](../../../../../../dispersion-relation.md):

$$
\nu=-\frac{iR_0}{2}\pm\sqrt{k^2c_0^2-\frac{R_0^2}{4}+inkR_0U}.
$$

If the imaginary part of the square root has magnitude $b$, then

$$
b^2=\frac12\left[\sqrt{\left(k^2c_0^2-\frac{R_0^2}{4}\right)^2+n^2k^2R_0^2U^2}-\left(k^2c_0^2-\frac{R_0^2}{4}\right)\right].
$$

One root grows exactly when $b>R_0/2$. For $k\ne0$, squaring the equivalent positive inequality gives $n^2U^2>c_0^2$. Thus **positive flow is unstable whenever $\boxed{U>c_0/n}$**. This proves the entire stated range, not just a small neighborhood of threshold. Zero [wavenumber](../../../../../../wavenumber.md) has only a neutral uniform-area change and a damped [velocity](../../../../../../velocity.md) mode.

Near threshold write $nU=c_0(1+\delta)$ and follow the neutral branch as $\nu=kc_0+\delta\nu_1+O(\delta^2)$. Substitution yields

$$
(2kc_0+iR_0)\nu_1=ikR_0c_0.
$$

Taking its imaginary part gives the growth rate

$$
\boxed{\operatorname{Im}\omega=\frac{\delta R_0k^2c_0^2}{2(k^2c_0^2+R_0^2/4)}+O(\delta^2).}
$$

Area increases reduce friction, causing a [velocity](../../../../../../velocity.md) increase that feeds the area disturbance through [mass conservation](../../../../../../mass-conservation.md). The [pressure](../../../../../../pressure.md)-driven base flow supplies the energy; the positive friction coefficient does not by itself prevent instability of that maintained flow.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
