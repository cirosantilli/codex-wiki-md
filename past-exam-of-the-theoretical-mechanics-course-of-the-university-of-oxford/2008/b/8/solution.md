<h1 id="b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Let the bed be $z=0$ and the free surface $z=h(x,t)$. In a long, shallow layer, vertical acceleration is smaller than gravity, so the vertical [Euler equation](../../../../euler-equations-for-an-inviscid-fluid-split.md) gives [hydrostatic pressure](../../../../hydrostatic-pressure.md) $p=p_{\rm atm}+\rho g(h-z)$. [Incompressibility](../../../../incompressible-flow.md) makes the vertical speed smaller than the horizontal speed by the [aspect ratio](../../../../aspect-ratio.md); [irrotationality](../../../../irrotational-flow.md) then makes the leading horizontal [velocity](../../../../velocity.md) depth-independent. The horizontal [Euler equation](../../../../euler-equations-for-an-inviscid-fluid-split.md) becomes

$$
\boxed{u_t+uu_x+gh_x=0.}
$$

Integrating $u_x+w_z=0$ across the depth, using bed impermeability $w(0)=0$ and the surface condition $w(h)=h_t+uh_x$, yields

$$
\boxed{h_t+(hu)_x=0.}
$$

Combining these gives the conservative momentum equation $(hu)_t+(hu^2+gh^2/2)_x=0$. Integral mass and [momentum balance](../../../../momentum-balance-for-a-material-fluid-element.md) across a stationary thin jump therefore require

$$
\boxed{[hu]_-^+=0,\qquad[hu^2+gh^2/2]_-^+=0.}
$$

These conservation laws still apply across a jump where the smooth hydrostatic/[irrotational](../../../../irrotational-vector-field.md) derivation does not resolve the internal turbulent structure.

Put $A=h_-$, $B=h_+$ and $q=Au_-=Bu_+>0$, orienting the flow from minus to plus. For a nontrivial jump the momentum condition gives $q^2=gAB(A+B)/2$. Its change in mechanical-[energy](../../../../energy-split.md) [flux](../../../../flux.md) is

$$
\begin{aligned}
[\rho hu(u^2/2+gh)]_-^+
&=\rho q\left[\frac{q^2}{2}\left(\frac1{B^2}-\frac1{A^2}\right)+g(B-A)\right]\\
&=-\frac{\rho gq(B-A)^3}{4AB}
=\boxed{\frac{\rho gu_-(h_--h_+)^3}{4h_+}}.
\end{aligned}
$$

A passive jump cannot create mechanical [energy](../../../../energy-split.md), so the change is nonpositive. Since $q>0$, $\boxed{h_+>h_-}$ for a genuine jump; equality describes no jump. The upstream flow is supercritical and the downstream flow subcritical, since $Fr_-^2=B(A+B)/(2A^2)>1$ and $Fr_+^2=A(A+B)/(2B^2)<1$.

The gas-dynamic analogue is a compressive [normal shock](../../../../normal-shock-wave.md): [density](../../../../density.md) and [pressure](../../../../pressure-split.md) increase and flow changes from [supersonic](../../../../supersonic-flow.md) to [subsonic](../../../../subsonic-flow.md). [Entropy](../../../../entropy-split.md) increases; directed mechanical [energy](../../../../energy-split.md) is irreversibly converted into [internal energy](../../../../internal-energy-split.md). Total gas [energy](../../../../energy-split.md), including [internal energy](../../../../internal-energy-split.md), is conserved across an [adiabatic](../../../../adiabatic-process.md) [shock](../../../../shock-wave.md). This distinguishes that total-[energy](../../../../energy-split.md) balance from the reduced shallow-water mechanical-[energy](../../../../energy-split.md) loss.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the theoretical mechanics course of the University of Oxford](../../../split.md)
5. [Theoretical mechanics course of the University of Oxford](../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
