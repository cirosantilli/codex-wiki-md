<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [de Rham cohomology](../../../../../../de-rham-cohomology.md) of $X$ is

$$
H^r_{\mathrm{dR}}(X)
=\frac{\ker(d:\Omega^r(X)\to\Omega^{r+1}(X))}
{\operatorname{im}(d:\Omega^{r-1}(X)\to\Omega^r(X))}.
$$

Because pullback commutes with $d$, it sends [closed forms](../../../../../../closed-differential-form.md) to closed forms and [exact forms](../../../../../../exact-differential-form.md) to exact forms. Thus a smooth map induces

$$
F^*:H^r_{\mathrm{dR}}(Y)\longrightarrow H^r_{\mathrm{dR}}(X).
$$

Let $H:X\times I\to Y$ be a smooth homotopy and write $H_t(x)=H(x,t)$. If $V=\partial_t$, [Cartan's magic formula](../../../../../../cartan-s-magic-formula.md) gives

$$
\frac d{dt}H_t^*\omega
=H_t^*(\mathcal L_V\omega)
=d\,H_t^*(\iota_V\omega)+H_t^*(\iota_Vd\omega).
$$

Integrating defines a degree-minus-one operator $K$ satisfying

$$
H_1^*-H_0^*=dK+Kd.
$$

For closed $\omega$, the difference is exact, so smoothly homotopic maps induce the same map on de Rham cohomology.

If $F:X\to Y$ is a [homotopy equivalence](../../../../../../homotopy-equivalence.md) with inverse up to homotopy $G$, functoriality and homotopy invariance give

$$
G^*F^*=\operatorname{id},\qquad F^*G^*=\operatorname{id}.
$$

**Hence $F^*$ is an isomorphism.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
