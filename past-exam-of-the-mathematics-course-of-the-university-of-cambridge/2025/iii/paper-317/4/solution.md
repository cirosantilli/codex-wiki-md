<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a circular binary with fixed total mass $M=M_1+M_2$, the orbital angular momentum is

$$
J=M_1M_2\sqrt{\frac{Ga}{M}}.
$$

[Conservative binary mass transfer](../../../../../conservative-binary-mass-transfer.md) keeps $J$ and $M$ fixed, so $a\propto(M_1M_2)^{-2}$. Since $M_1=Mq/(1+q)$ and $M_2=M/(1+q)$,

$$
\boxed{a\propto\frac{(1+q)^4}{q^2}}.
$$

Conservative transfer gives $d\log M_2/d\log M_1=-q$ and hence $d\log q/d\log M_1=1+q$. It follows that

$$
\frac{d\log a}{d\log M_1}=2(q-1),
$$

and, using $R_L\simeq0.4aq^{2/9}$,

$$
\boxed{\alpha=\frac{d\log R_L}{d\log M_1}
=2(q-1)+\frac29(1+q)
=\frac{20}{9}\left(q-\frac45\right)}.
$$

Let $f=\log(R_1/R_L)$. While the system is detached, $M_1$ is constant, so

$$
\boxed{\dot f=\tau_{\rm nuc}^{-1}}.
$$

During [Roche-lobe overflow](../../../../../roche-lobe-overflow.md), $\dot{\log M_1}=-f/\tau_{\rm dyn}$, while

$$
\dot{\log R_1}=\beta\dot{\log M_1}+\tau_{\rm nuc}^{-1},
\qquad
\dot{\log R_L}=\alpha\dot{\log M_1}.
$$

Therefore

$$
\boxed{\dot f+\frac{\beta-\alpha}{\tau_{\rm dyn}}f
=\frac1{\tau_{\rm nuc}}}.
$$

If $\beta>\alpha$, the stable fixed point is

$$
\boxed{f\longrightarrow
\frac1{\beta-\alpha}\frac{\tau_{\rm dyn}}{\tau_{\rm nuc}}}.
$$

The corresponding mass-transfer rate is

$$
-\dot{\log M_1}=\frac1{(\beta-\alpha)\tau_{\rm nuc}},
$$

so the donor overfills its Roche lobe by only a tiny amount while losing mass on the slow nuclear timescale.

If $\beta<\alpha$, overflow is unstable. Starting at contact time $t_0$ with $f(t_0)=0$,

$$
\boxed{f(t)=\frac{\tau_{\rm dyn}}{(\alpha-\beta)\tau_{\rm nuc}}
\left[e^{(\alpha-\beta)(t-t_0)/\tau_{\rm dyn}}-1\right]}.
$$

The overflow and mass-loss rate grow exponentially on a dynamical timescale, leading toward unstable mass transfer or a common-envelope phase.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 317](../../paper-317-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
