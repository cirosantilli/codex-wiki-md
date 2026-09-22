<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose interface $z=0$, source $(0,-h)$ in medium 1 and transmitted medium 2 at $z>0$. Write $\mu_j=\rho_j\beta_j^2$, take $p$ to be signed tangential slowness, and define

$$
q_j=\sqrt{\beta_j^{-2}-p^2}>0,\qquad
\sin\theta_j=\beta_jp,\quad\cos\theta_j=\beta_jq_j.
$$

The propagating range is $|p|<1/\max(\beta_1,\beta_2)$; the absolute value is needed if both azimuthal directions are included. [Snell law for elastic waves](../../../../../../snell-law-for-elastic-waves.md) preserves $p$. The incident ray reaches the interface after time $t_1$ at horizontal position $x_I$, with

$$
\boxed{t_1(p)=\frac{h}{\beta_1^2q_1},\qquad x_I(p)=\frac{hp}{q_1}}.
$$

In the transmitted medium its velocity is $\beta_2(\sin\theta_2,\cos\theta_2)=(\beta_2^2p,\beta_2^2q_2)$. Therefore the [refraction of a cylindrical SH wavefront](../../../../../../refraction-of-a-cylindrical-sh-wavefront.md) gives

$$
\boxed{x(t,p)=\frac{hp}{q_1}+\beta_2^2p[t-t_1(p)],\qquad
z(t,p)=\beta_2^2q_2[t-t_1(p)],\quad t\ge t_1(p)}.
$$

Time is measured from source emission. For a later emission add its time to the clock. These straight transmitted rays and their common-time endpoints determine the refracted [wavefront](../../../../../../wavefront.md); critical incidence and an evanescent transmitted field are excluded by the strict slowness bound.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
