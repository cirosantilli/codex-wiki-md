<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Since $\mathbf e_\rho\times\mathbf e_\varphi=\mathbf e_z$, the [Poynting vector](../../../../../poynting-vector.md) is axial. The [magnetic permeability](../../../../../permeability-electromagnetism.md) cancels from $\mathbf E\times\mathbf B/\mu$ in each material layer:

$$
\boxed{\boldsymbol{\mathcal P}(\rho)=\begin{cases}
0,&\rho<a\ \text{or}\ \rho>b,\\[2pt]
\displaystyle\frac{VI\epsilon'}{2\pi\Delta\rho^2}\mathbf e_z,&a<\rho<c,\\[2pt]
\displaystyle\frac{VI\epsilon}{2\pi\Delta\rho^2}\mathbf e_z,&c<\rho<b.
\end{cases}}
$$

The signed [Poynting flux](../../../../../poynting-flux.md) through the plane with [unit normal](../../../../../unit-normal.md) $+\mathbf e_z$ is its [surface integral](../../../../../surface-integral.md) with area element $\rho\,d\rho\,d\varphi$:

$$
\begin{aligned}
P&=2\pi\int_a^b\mathcal P_z(\rho)\rho\,d\rho\\
&=\frac{VI}{\Delta}\left[\epsilon'\ln(c/a)+\epsilon\ln(b/c)\right].
\end{aligned}
$$

Thus

$$
\boxed{P=VI.}
$$

The transmitted [electromagnetic energy](../../../../../electromagnetic-energy.md) per unit time is the circuit's terminal power. For $VI>0$, the [Poynting flux](../../../../../poynting-flux.md) points in the direction of the inner [electric current](../../../../../electric-current.md). The [electromagnetic energy](../../../../../electromagnetic-energy.md) travels through the insulating gap and reaches a load at the end of the [coaxial cable](../../../../../coaxial-cable.md). The radii and material constants redistribute the [electromagnetic energy density](../../../../../electromagnetic-energy-density.md) and the local [Poynting vector](../../../../../poynting-vector.md), while their integrated [Poynting flux](../../../../../poynting-flux.md) depends only on the terminal [electric potential difference](../../../../../electric-potential-difference.md) and [electric current](../../../../../electric-current.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the electromagnetism course of the University of Oxford](../../../../split.md)
6. [Electromagnetism course of the University of Oxford](../../../../../electromagnetism-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
