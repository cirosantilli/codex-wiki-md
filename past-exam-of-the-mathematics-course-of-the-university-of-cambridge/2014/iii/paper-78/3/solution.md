<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The imposed [pressure gradient](../../../../../pressure-gradient.md) and [Darcy's law](../../../../../darcy-law.md) give a linear velocity profile. Use $U$ as the mean [pore velocity](../../../../../pore-velocity.md) in the contaminant [advection-diffusion equation](../../../../../advection-diffusion-equation.md); then

$$
u(y)=\frac{2Uy}{H},\qquad
c_t+u(y)c_x=D_Lc_{xx}+D_Tc_{yy},\qquad
c_y(0)=c_y(H)=0.
$$

The last conditions express zero transverse solute flux under the standard closed-layer interpretation. Transverse exchange through the layer boundaries would change this cell problem and requires additional boundary data. If the prescribed mean speed is a [Darcy velocity](../../../../../darcy-velocity.md), its corresponding [pore velocity](../../../../../pore-velocity.md) is that speed divided by [porosity](../../../../../porosity.md).

The given parameter is the ratio of transverse mixing time to travel time:

$$
\boxed{P=\frac{H^2/D_T}{L/U}\ll1.}
$$

Thus [transverse dispersion](../../../../../transverse-dispersion.md) mixes the contaminant across the layer many times during its passage along the long layer. Different fluid speeds still matter: repeated exchange between slow and fast portions produces [Taylor dispersion](../../../../../taylor-dispersion.md), rather than transport solely at each parcel's original speed. The averaged description applies after $t\gg H^2/D_T$ and on longitudinal scales large compared with the distance travelled during that mixing time.

Write $C=\overline c$ and, to leading correction order, $c=C+\chi(y)C_x+\cdots$, with $\overline\chi=0$. Taking $C_t\simeq-UC_x$ in the local equation gives the cell problem

$$
D_T\chi''=u-U,\qquad \chi'(0)=\chi'(H)=0.
$$

With $\eta=y/H$, its solution is

$$
\chi(y)=\frac{UH^2}{D_T}\left(\frac{\eta^3}{3}-\frac{\eta^2}{2}+\frac1{12}\right).
$$

Averaging the local [advection-diffusion equation](../../../../../advection-diffusion-equation.md) now yields $C_t+UC_x=[D_L-\overline{(u-U)\chi}]C_{xx}$. An [integration by parts](../../../../../integration-by-parts.md) in the cell problem gives $-\overline{(u-U)\chi}=D_T\overline{(\chi')^2}$. Since $\int_0^1(\eta^2-\eta)^2d\eta=1/30$, the effective equation is

$$
\boxed{C_t+UC_x=D_{\rm eff}C_{xx},\qquad
D_{\rm eff}=D_L+\frac{U^2H^2}{30D_T}.}
$$

This is [Taylor dispersion in a linear porous-layer velocity profile](../../../../../taylor-dispersion-in-a-linear-porous-layer-velocity-profile.md). For a localized pulse away from the inlet and outlet, its mean position advances at $U$ and its longitudinal variance grows as $2D_{\rm eff}t$.

For the inlet step, use the semi-infinite inlet approximation $x>0$, $C(0,t)=1$, $C(x,0)=0$ and $C\to0$ as $x\to\infty$ at fixed $t$. The resulting [constant-concentration inlet solution](../../../../../constant-concentration-inlet-solution.md) is

$$
\boxed{C(x,t)=\frac12\operatorname{erfc}\left(\frac{x-Ut}{2\sqrt{D_{\rm eff}t}}\right)
+\frac12e^{Ux/D_{\rm eff}}\operatorname{erfc}\left(\frac{x+Ut}{2\sqrt{D_{\rm eff}t}}\right).}
$$

One derivation is to [Laplace transform](../../../../../laplace-transform.md) in time: $\widetilde C(x,p)=p^{-1}\exp[(U-\sqrt{U^2+4D_{\rm eff}p})x/(2D_{\rm eff})]$. Inverting gives the two [complementary error functions](../../../../../complementary-error-function.md). Their sum is one at $x=0$; for fixed $x>0$ both terms vanish as $t\downarrow0$, and substitution verifies the averaged equation. Retaining only the first term gives the familiar moving error-function front far from the inlet when longitudinal [advection](../../../../../advection.md) dominates [diffusion](../../../../../diffusion.md), but does not satisfy the inlet condition exactly.

For a literal finite layer $0<x<L$, a downstream boundary condition is also needed once the outlet influences the solution. The PDF's step-inlet request specifies only the initially clean region $x>0$, so the formula above is the semi-infinite/long-layer solution, not a claim of a unique finite-interval solution with unspecified outlet data.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
