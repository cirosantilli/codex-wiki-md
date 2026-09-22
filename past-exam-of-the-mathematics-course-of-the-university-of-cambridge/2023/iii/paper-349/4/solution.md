<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A star-forming galaxy contains short-lived, massive O and B stars whose hot photospheres dominate the ultraviolet and blue continuum and ionize surrounding gas. Once star formation ceases, these stars disappear quickly and an older, cooler stellar population produces a redder spectrum with stronger stellar absorption features and a prominent 4000-angstrom break.

In star-forming regions, direct stellar continuum is accompanied by nebular free-bound and free-free continuum, hydrogen and helium recombination lines, collisionally excited metal lines, and infrared emission from dust that absorbed shorter-wavelength photons. Supernova remnants and cosmic rays add synchrotron radio emission, while hot shocked gas can emit X-rays.

The [Strömgren sphere](../../../../../stromgren-sphere.md) model assumes a steady ionizing source in uniform, static, pure hydrogen of number density $n_H$, with a sharp [ionization front](../../../../../ionization-front.md) enclosing fully ionized gas. If $N_i=(4\pi/3)R^3n_H$ is the number of ions, photon conservation gives

$$
\frac{dN_i}{dt}=\dot N_{\rm ion}
-\frac{4\pi}{3}R^3\alpha n_H^2.
$$

The equilibrium [Strömgren radius](../../../../../stromgren-radius.md) and [recombination time](../../../../../recombination-time.md) are

$$
R_S^3=\frac{3\dot N_{\rm ion}}{4\pi\alpha n_H^2},
\qquad t_{\rm rec}=\frac1{\alpha n_H}.
$$

Consequently the radius obeys

$$
3R^2\frac{dR}{dt}
=\frac{R_S^3-R^3}{t_{\rm rec}}.
$$

Writing $x=(R/R_S)^3$ turns this into $dx/d(t/t_{\rm rec})=1-x$. For an initially neutral medium, $x(0)=0$, and the [Ionization-front growth of a Strömgren sphere](../../../../../ionization-front-growth-of-a-stromgren-sphere.md) is

$$
\boxed{R(t)=R_S\left(1-e^{-t/t_{\rm rec}}\right)^{1/3}.}
$$

The front initially expands rapidly because few ions are recombining and asymptotically approaches $R_S$ as recombinations balance ionizations. This photon-counting solution precedes any pressure-driven hydrodynamic expansion of the H II region.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 349](../../paper-349-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
