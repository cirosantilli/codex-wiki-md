<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use $f(x)=(2\pi)^{-1}\int_{\mathbb R}\widetilde f(k)e^{ikx}dk$. [Jordan's lemma](../../../../jordan-s-lemma.md) says that for $x>0$, if a function $h$ has maximum modulus $M_R\to0$ on upper semicircles, then $\int_{C_R}h(k)e^{ikx}dk\to0$; a bound is $\pi M_R/x$. For $x<0$ use lower semicircles instead. The rational factors here meet this decay condition, so the [residue theorem](../../../../residue-theorem.md) evaluates their inverse transforms.

For $1/(a+ik)$, only the upper half-plane contains a pole, at $k=ia$. Its [residue](../../../../residue.md) after multiplication by $e^{ikx}$ is $-ie^{-ax}$. The lower contour encloses no pole. Therefore

$$
\boxed{\mathcal F^{-1}\left[\frac1{a+ik}\right](x)=e^{-ax}H(x).}
$$

Here $H$ is the [Heaviside step function](../../../../heaviside-step-function.md), with midpoint value $H(0)=1/2$ for symmetric Fourier inversion.

For $1/(a^2+k^2)$, the upper-pole [residue](../../../../residue.md) is $e^{-ax}/(2ia)$ when $x>0$, while the clockwise lower contour gives the matching expression for $x<0$. Thus

$$
\boxed{\mathcal F^{-1}\left[\frac1{a^2+k^2}\right](x)=\frac{e^{-a|x|}}{2a}.}
$$

The final rational factor has double poles at $\pm ia$. At the upper pole,

$$
\operatorname{Res}_{k=ia}\frac{e^{ikx}(a^2-k^2)}{(a^2+k^2)^2}
=\left.\frac d{dk}\frac{e^{ikx}(a^2-k^2)}{(k+ia)^2}\right|_{k=ia}
=-\frac{ix}2e^{-ax}.
$$

The upper inverse integral is $i$ times that [residue](../../../../residue.md). The lower contour for negative $x$ supplies $-x e^{ax}/2$, and the value at zero is zero. Consequently

$$
\boxed{\mathcal F^{-1}\left[\frac{a^2-k^2}{(a^2+k^2)^2}\right](x)=\frac{|x|}2e^{-a|x|}.}
$$

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [2008](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
