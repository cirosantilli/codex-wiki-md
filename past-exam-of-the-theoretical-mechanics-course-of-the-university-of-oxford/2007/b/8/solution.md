<h1 id="b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Work in the rest frame of the planar [shock](../../../../shock-wave.md), with nonzero [mass flux](../../../../mass-flux.md) $j=\rho u$. [Conservation of mass](../../../../mass-conservation.md) gives $[j]=0$; the tangential and normal components of [balance of linear momentum](../../../../balance-of-linear-momentum.md) give $[jv]=0$ and $[p+ju]=0$. Thus $[v]=0$. For an [ideal gas](../../../../ideal-gas-split.md), [specific internal energy](../../../../specific-internal-energy.md) is $e=c_vT=p/[(\gamma-1)\rho]$, and [specific enthalpy](../../../../specific-enthalpy.md) is $e+p/\rho=\gamma p/[(\gamma-1)\rho]$. Total energy flux is $j[(u^2+v^2)/2+e+p/\rho]$. Its continuity, with $v$ already continuous, gives

$$
\boxed{[\rho u]=[v]=[p+\rho u^2]=\left[\frac{u^2}2+\frac{\gamma p}{(\gamma-1)\rho}\right]=0.}
$$

Put $c^2=\gamma p/\rho$ and $M=u/c$. Since $p=ju/(\gamma M^2)$, the normal component of [balance of linear momentum](../../../../balance-of-linear-momentum.md) says $u[1+1/(\gamma M^2)]$ is constant. Hence

$$
\boxed{\frac{u_+}{u_-}=\frac{M_+^2(1+\gamma M_-^2)}{M_-^2(1+\gamma M_+^2)}.}
$$

The energy equation says $u^2[1/2+1/((\gamma-1)M^2)]$ is constant, giving

$$
\boxed{\left(\frac{u_+}{u_-}\right)^2=\frac{M_+^2[2+(\gamma-1)M_-^2]}{M_-^2[2+(\gamma-1)M_+^2]}.}
$$

Set $a=M_-^2$, $b=M_+^2$, square the first relation and equate to the second. After clearing positive denominators the equation factors as

$$
\boxed{(b-a)\{b[2\gamma a-(\gamma-1)]-[2+(\gamma-1)a]\}=0.}
$$

The first factor is the unchanged state. For a genuine [shock](../../../../shock-wave.md) the second factor vanishes, yielding

$$
\boxed{M_+^2=\frac{2+(\gamma-1)M_-^2}{2\gamma M_-^2-(\gamma-1)}.}
$$

The physical selection principle is [entropy](../../../../entropy-split.md) increase in the direction of flow. For $u_\pm>0$, the upstream side is $x<0$ and the downstream side is $x>0$. A compressive [entropy](../../../../entropy-split.md)-admissible [shock](../../../../shock-wave.md) has $\boxed{M_->1,\quad M_+<1}$; interpreting the printed “ahead” and “behind” spatial labels must respect these explicit side assignments. The expansion-[shock](../../../../shock-wave.md) branch would violate the second law.

Substitution gives the [velocity](../../../../velocity.md) ratio

$$
\boxed{\frac{u_+}{u_-}=\frac{2+(\gamma-1)M_-^2}{(\gamma+1)M_-^2}<1.}
$$

Since $v$ is unchanged while the normal component decreases, $|v|/u$ increases. Thus an oblique flow bends **towards the [shock](../../../../shock-wave.md) plane**, equivalently away from its normal. If $v=0$ there is no angular bending; the flow stays normal and simply slows. The tangential continuity, not a change in the tangential speed, causes the deflection.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the theoretical mechanics course of the University of Oxford](../../../split.md)
5. [Theoretical mechanics course of the University of Oxford](../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
