<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $\sigma_0=0$. Equating the cylindrical tether area $2\pi rL$ to $A\Delta\alpha$ gives

$$
\log\left(1+\frac{\sigma A}{\pi^2k_c}\right)
=\frac{16\pi^2k_crL}{Ak_BT},
$$

or

$$
\sigma=\frac{\pi^2k_c}{A}
\left[\exp\left(\frac{16\pi^2k_crL}{Ak_BT}\right)-1\right].
$$

Because a cylinder has $2H=1/r$, the energy becomes

$$
E(r,L)=\frac{\pi k_cL}{r}
+\frac{\pi k_BT}{8}\left[
e^{16\pi^2k_crL/(Ak_BT)}-1\right]-FL.
$$

The two stationarity equations imply

$$
\boxed{F=\frac{2\pi k_c}{r},
\qquad
e^{16\pi^2k_crL/(Ak_BT)}=\frac{A}{2\pi^2r^2}.}
$$

Eliminating $r$ gives the implicit [entropic membrane-tether force--extension relation](../../../../../../entropic-membrane-tether-force-extension-relation.md)

$$
\boxed{L=\frac{Ak_BTF}{32\pi^3k_c^2}
\log\left(\frac{AF^2}{8\pi^4k_c^2}\right).}
$$

As tether length grows, fluctuation area is depleted, tension rises, the tether narrows, and the required force increases.

For a membrane connected to a reservoir at fixed tension, its energy per length is $\pi k_c/r+2\pi\sigma r-F$. Minimization instead gives

$$
\boxed{r=\sqrt{\frac{k_c}{2\sigma}},
\qquad F=2\pi\sqrt{2k_c\sigma}.}
$$

The reservoir supplies area without changing $\sigma$, so the force is independent of extension; the finite vesicle has an entropic, strain-stiffening response.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 355](../../../paper-355-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
