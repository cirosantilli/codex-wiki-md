<h1 id="4/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take uncompensated [donor impurities](../../../../../donor-impurity.md) and initially approximate them as ionized. [Charge neutrality](../../../../../charge-neutrality.md) then gives $n-p=N_d$, while the [semiconductor mass-action law](../../../../../semiconductor-mass-action-law.md) gives $np=n_i^2$. Solving the quadratic without prematurely discarding minority carriers,

$$
n=\frac{N_d+\sqrt{N_d^2+4n_i^2}}2,\qquad
p=\frac{2n_i^2}{N_d+\sqrt{N_d^2+4n_i^2}}.
$$

Since $N_d\gg n_i$, the hole density is

$$
\boxed{p\simeq\frac{n_i^2}{N_d}
=4.5816\times10^{10}\,\mathrm{m^{-3}},\qquad
n\simeq1.0000\times10^{20}\,\mathrm{m^{-3}}.}
$$

Use the conduction population to locate the [chemical potential](../../../../../chemical-potential-split.md):

$$
\boxed{E_c-\mu=k_BT\ln\frac{N_c}{n}=0.269180\,\mathrm{eV},\qquad
\mu-E_v=0.840820\,\mathrm{eV}.}
$$

It moves toward the [conduction band](../../../../../conduction-band.md) but remains about $10.4k_BT$ below it, so the mobile electrons are nondegenerate. Despite the donor binding energy being comparable with $k_BT$, the large number of available conduction states makes ionization almost complete at this dilute doping. For a singly occupied two-spin donor, $N_d^+/N_d=[1+2e^{(\mu-E_D)/(k_BT)}]^{-1}$, with $E_D=E_c-0.02584\,\mathrm{eV}$. The inferred value is $0.99984$, confirming the approximation to much better than one percent. Including this small correction raises the hole density only to about $4.5824\times10^{10}\,\mathrm{m^{-3}}$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [4](../../../4.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the condensed matter physics course of the University of Oxford](../../../../split.md)
6. [Condensed matter physics course of the University of Oxford](../../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
7. [Year 3 of the physics course of the University of Oxford](../../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
