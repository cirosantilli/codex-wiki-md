<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $C_{ikjl}=\sum_aT^a_{ik}T^a_{jl}$. Hermiticity converts its complex-conjugate factors into $T^b_{ki}T^b_{lj}$. Summing all external colors therefore gives

$$
\sum_{i,j,k,l}|C_{ikjl}|^2
=\sum_{a,b}\operatorname{Tr}(T^aT^b)\operatorname{Tr}(T^aT^b)
=\frac14\sum_{a,b}\delta^{ab}\delta^{ab}=\boxed{2},
$$

since SU(3) has eight generators. This is a sum, before averaging the nine equally populated incoming color states.

For the [spinor](../../../../spinor.md) current, use $\bar u=u^\dagger\gamma^0$, $(\gamma^0)^2=1$ and the stated gamma-matrix adjoint identity:

$$
\begin{aligned}
[\bar u_3\gamma^\mu u_1]^*
&=u_1^\dagger(\gamma^\mu)^\dagger\gamma^0u_3\\
&=u_1^\dagger\gamma^0\gamma^\mu\gamma^0\gamma^0u_3
=\bar u_1\gamma^\mu u_3.
\end{aligned}
$$

The [spin sum](../../../../spin-sum.md) completeness relation then closes each product of currents into a [trace](../../../../matrix-trace.md). Averaging two spins for each incoming [quark](../../../../quark.md), in addition to nine incoming colors, gives

$$
\overline{|\mathcal M|^2}=\frac{2}{9\times4}\frac{g_s^4}{t^2}
\operatorname{Tr}(\not{p}_3\gamma^\mu\not{p}_1\gamma^\nu)
\operatorname{Tr}(\not{p}_4\gamma_\mu\not{p}_2\gamma_\nu),\qquad t=q^2.
$$

The factor is $1/18$, rather than $2/9$: the latter omits the initial spin average.

To derive the four-[gamma matrix](../../../../gamma-matrices.md) [trace](../../../../matrix-trace.md), first anticommutation and cyclicity give $\operatorname{Tr}(\gamma^\alpha\gamma^\beta)=4g^{\alpha\beta}$, with $\operatorname{Tr}1=4$. If $T=\operatorname{Tr}(\gamma^\lambda\gamma^\mu\gamma^\sigma\gamma^\nu)$, move $\gamma^\lambda$ successively through the next three matrices. The last term is $-T$ by cyclicity, so

$$
2T=2g^{\lambda\mu}\operatorname{Tr}(\gamma^\sigma\gamma^\nu)
-2g^{\lambda\sigma}\operatorname{Tr}(\gamma^\mu\gamma^\nu)
+2g^{\lambda\nu}\operatorname{Tr}(\gamma^\mu\gamma^\sigma).
$$

Substitution yields

$$
\boxed{T=4(g^{\lambda\mu}g^{\sigma\nu}-g^{\lambda\sigma}g^{\mu\nu}+g^{\lambda\nu}g^{\mu\sigma}).}
$$

Consequently the first [momentum](../../../../momentum-split.md) [trace](../../../../matrix-trace.md) is $4(p_3^\mu p_1^\nu+p_3^\nu p_1^\mu-g^{\mu\nu}p_3\cdot p_1)$. Contracting both [traces](../../../../matrix-trace.md) gives

$$
32[(p_3\cdot p_4)(p_1\cdot p_2)+(p_3\cdot p_2)(p_1\cdot p_4)]
=8(s^2+u^2).
$$

Here $s=(p_1+p_2)^2$, $u=(p_1-p_4)^2$ and all external masses vanish. Thus the [distinct-flavor quark scattering color factor](../../../../distinct-flavor-quark-scattering-color-factor.md) gives

$$
\boxed{\overline{|\mathcal M|^2}=\frac49g_s^4\frac{s^2+u^2}{t^2}
=\frac{4g_s^4}{9}\frac{4+(1+\cos\theta^*)^2}{(1-\cos\theta^*)^2}.}
$$

We used $t=-s(1-\cos\theta^*)/2$ and $u=-s(1+\cos\theta^*)/2$. The forward divergence reflects massless $t$-channel exchange in this parton-level tree approximation; it is not an unrestricted prediction for an experimentally resolved jet [cross section](../../../../cross-section-physics.md).

Finally, completeness of the SU(3) generators gives the [fundamental-generator Fierz identity](../../../../fundamental-generator-fierz-identity.md)

$$
C_{ikjl}=\frac12\left(\delta_{il}\delta_{jk}-\frac13\delta_{ik}\delta_{jl}\right).
$$

For each distinct pair $i\ne j$, the allowed final colors are either $k=i,l=j$, with coefficient $-1/6$, or $k=j,l=i$, with coefficient $1/2$. If $i=j$, only $k=l=i$ is nonzero, with coefficient $1/3$. These are **15 ordered configurations**: six unchanged-color cases, six exchanged-color cases and three all-equal cases. Their squared coefficients sum to $6/36+6/4+3/9=2$, independently checking the first result. Flavor remains tied to each external line; exchanging colors does not exchange the up and down [quark](../../../../quark.md) species.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the gauge field theory course of the University of Cambridge](../../../split.md)
5. [Gauge Field Theory course of the University of Cambridge](../../../../gauge-field-theory-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
