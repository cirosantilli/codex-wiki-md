<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\rho_s$ be the grain density and $g'=g/g_0$. Vertical force balance for the [poroelastic aquifer](../../../../../../poroelastic-aquifer.md) gives

$$
\frac{d\sigma_e}{dz}=\phi(\rho_s-\rho)g,
$$

with compression taken negative in $\sigma_e=E(\phi_0-\phi)/\phi_0$. Hence

$$
\frac{d\phi}{dz}=-\frac{g'}{\ell_c}\phi,
\qquad
\boxed{\ell_c=\frac{E}{\phi_0(\rho_s-\rho)g_0}.}
$$

The zero-effective-stress condition $\phi(h)=\phi_0$ then gives

$$
\boxed{\phi(z)=\phi_0\exp\left[\frac{g'(h-z)}{\ell_c}\right].}
$$

This identifies the [poroelastic compaction length](../../../../../../poroelastic-compaction-length.md).

The water volume per unit horizontal distance is

$$
V=\int_0^h(1-\phi)\,dz.
$$

For $h\ll\ell_c$, a [Taylor expansion](../../../../../../taylor-expansion.md) yields

$$
\boxed{V=(1-\phi_0)h-\frac{\phi_0g'h^2}{2\ell_c}+O(h^3/\ell_c^2).}
$$

Storage conservation is $V_t+q_x=R$. Integrating from river to divide and using $q(L,t)=0$ gives the river influx

$$
\boxed{Q_r(t)=-q(0,t)=RL-\frac d{dt}\int_0^L V(x,t)\,dx.}
$$

For $g'=1+\epsilon e^{i\omega t}$ and a groundwater profile that changes little during one tide, the direct storage oscillation has magnitude

$$
|\delta Q_r|\sim\frac{\epsilon\omega\phi_0}{2\ell_c}\int_0^Lh^2\,dx.
$$

With typical thickness $H$ and mean recharge discharge $\overline Q_r=RL$,

$$
\boxed{\frac{|\delta Q_r|}{\overline Q_r}
\sim\frac{\epsilon\omega\phi_0H^2}{2\ell_cR}.}
$$

Using the steady balance $R\sim KH^2/L^2$ gives the equivalent estimate $|\delta Q_r|/\overline Q_r\sim\epsilon\omega\phi_0L^2/(2\ell_cK)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
