<h1 id="a10/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $D$ be the equal constant [density of states](../../../../../../density-of-states.md) per unit volume and energy in each band. In the [nondegenerate semiconductor](../../../../../../nondegenerate-semiconductor.md) regime, the conduction-band occupation is

$$
f(E)\simeq e^{-(E-\mu)/(k_BT)}.
$$

For bands broad compared with $k_BT$, integrating above the conduction edge gives

$$
n=D\int_{E_c}^{\infty}e^{-(E-\mu)/(k_BT)}\,dE
=Dk_BT\,e^{-(E_c-\mu)/(k_BT)}.
$$

The valence-hole integral similarly gives $p=Dk_BT\,e^{-(\mu-E_v)/(k_BT)}$. Midgap $\mu$ therefore implies

$$
\boxed{n=p\simeq Dk_BT\,e^{-E_g/(2k_BT)}},\qquad E_g=E_c-E_v.
$$

Inserting the carrier densities into the transport expression yields

$$
\sigma\simeq\underbrace{eDk_BT(u_e+u_h)}_{\sigma_0(T)}
 e^{-E_g/(2k_BT)}.
$$

**On treating the algebraic and mobility prefactor as approximately constant, the requested leading activation law is**

$$
\boxed{\sigma\propto e^{-E_g/(2k_BT)}}.
$$

The factor $1/2$ is essential: an intrinsic excitation creates an electron–hole pair, and charge neutrality places the [chemical potential](../../../../../../chemical-potential-split.md) halfway across the symmetric gap. The conduction-electron population is governed by $E_c-\mu=E_g/2$, not by replacing this separation with the full gap.

There is a qualification to the proportionality as printed. A literal [constant-density-of-states intrinsic semiconductor](../../../../../../constant-density-of-states-intrinsic-semiconductor.md) with temperature-independent mobilities retains the additional factor $T$. Indeed, using the full [Fermi-Dirac distribution](../../../../../../fermi-dirac-distribution.md) gives

$$
n=p=Dk_BT\ln\left(1+e^{-E_g/(2k_BT)}\right),
$$

which reduces to the expression above when $E_g\gg k_BT$. Thus the pure exponential is an activation approximation, not an exact consequence of constant DOS alone. A mobility sum proportional to $T^{-1}$ would cancel the leading algebraic factor.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [A10](../../../a10.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the chemistry A course of the University of Cambridge](../../../../../split.md)
7. [Chemistry A course of the University of Cambridge](../../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
