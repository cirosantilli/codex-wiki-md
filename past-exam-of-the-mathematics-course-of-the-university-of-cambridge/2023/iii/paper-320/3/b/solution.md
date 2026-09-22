<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put

$$
q=\frac{A_s}{A_h},
\qquad
\mu_s=\frac{2\pi A_s^3}{A_h^2},
\qquad
C=2\pi GA_h,
\qquad
\mathcal L=\mathcal K\log\Lambda.
$$

Part a gives

$$
r_t=qr_o,
\qquad
M_s=\mu_s r_o^2,
$$

while the host [circular speed](../../../../../../circular-speed.md) is $v_c=\sqrt{Cr_o}$. The [Chandrasekhar dynamical friction](../../../../../../chandrasekhar-dynamical-friction.md) acceleration reduces to the radius-independent value

$$
a_{\rm df}
=-\frac{4\pi G^2M_s(A_h/r_o)\mathcal L}{v_c^2}
=-2G\mu_s\mathcal L.
$$

Assume stripped material leaves with the satellite's instantaneous specific angular momentum. The remaining orbit then obeys

$$
\frac d{dt}(r_ov_c)=r_oa_{\rm df}.
$$

Since $r_ov_c=\sqrt C,r_o^{3/2}$,

$$
\boxed{
\frac{dr_o}{dt}=-K_s\sqrt{r_o},
\qquad
K_s=\frac{4G\mu_s\mathcal L}{3\sqrt C}}.
$$

For initial radius $r_{o0}$,

$$
\boxed{
r_o(t)=r_{o0}\left(1-\frac{t}{t_d}\right)^2,
\qquad
t_d=\frac{2\sqrt{r_{o0}}}{K_s}},
$$

and

$$
\boxed{
M_s(t)=M_{s0}\left(1-\frac{t}{t_d}\right)^4,
\qquad
r_t(t)=r_{t0}\left(1-\frac{t}{t_d}\right)^2}.
$$

In this ideal cusp, radius and remaining mass both reach zero at the finite time $t_d$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
