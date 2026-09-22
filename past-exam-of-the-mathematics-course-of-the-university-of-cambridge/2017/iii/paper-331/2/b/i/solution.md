<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $y=\tanh z$ and $a=1-k$, so $dy/dz=1-y^2$ and $\widehat w=(1-y^2)^{k/2}y^a$. Away from $y=0$, the [logarithmic derivative](../../../../../../../logarithmic-derivative.md) gives

$$
\frac{\widehat w'}{\widehat w}=\frac ay-y,\qquad
\frac{\widehat w''}{\widehat w}=\frac{a(a-1)}{y^2}-a-1+2y^2.
$$

For $c=0$, $\overline U''/\overline U=-2(1-y^2)$ and $N^2/\overline U^2=J(1-y^2)/y^2$. The [Taylor–Goldstein equation](../../../../../../../taylor-goldstein-equation.md) residual divided by $\widehat w$ consequently simplifies to

$$
[J-k(1-k)]\left(\frac1{y^2}-1\right).
$$

Thus the [neutral mode of the equal-width Hazel model](../../../../../../../neutral-mode-of-the-equal-width-hazel-model.md) requires

$$
\boxed{J=k(1-k).}
$$

The qualifier “solution” needs care at the [critical level of an internal gravity wave](../../../../../../../critical-level-of-an-internal-gravity-wave.md) $z=0$. For $0<k<1$, $\widehat w\sim z^{1-k}$ and $\widehat w'\sim(1-k)z^{-k}$: it is a solution separately on either side, not a classical smooth [eigenfunction](../../../../../../../eigenfunction.md) across the [critical level of an internal gravity wave](../../../../../../../critical-level-of-an-internal-gravity-wave.md). A branch for negative $\tanh z$ is also needed. For example, a limit from $c_i>0$ assigns $(\tanh z)^{1-k}=|\tanh z|^{1-k}e^{-i\pi(1-k)}$ on $z<0$.

The [critical-layer regularity of a neutral Hazel mode](../../../../../../../critical-layer-regularity-of-a-neutral-hazel-mode.md) further gives local finite horizontal [kinetic energy](../../../../../../../kinetic-energy.md) only for $0<k<1/2$, since [incompressible flow](../../../../../../../incompressible-flow.md) gives $\widehat u=i\widehat w'/k$ and $\int_0^\epsilon z^{-2k}dz$ then converges. At $k=1$, $J=0$ and $\widehat w=\operatorname{sech}z$ is smooth after the removable $\overline U''/\overline U$ quotient is continued. At $k=0$, $J=0$ and the formal $\tanh z$ profile does not decay at infinity, so it fails the remote endpoint condition. These qualifications prevent interpreting the whole closed parameter interval as a family of classical decaying modes.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
