<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [jump conditions](../../../../jump-condition.md) express a connected [elastic beam](../../../../elastic-beam.md) with no concentrated horizontal [force](../../../../force-split.md) or applied couple. [Continuity](../../../../continuous-function.md) of [tension](../../../../tension.md), $[T]=0$, follows from horizontal [force balance](../../../../force-balance.md). [Continuity](../../../../continuous-function.md) of the [displacement field](../../../../displacement-field-mechanics.md) and [slope](../../../../slope.md), $[w]=[w']=0$, excludes a break or a kink; a kink would also have unbounded bending [elastic energy](../../../../elastic-energy.md) in this model. [Continuity](../../../../continuous-function.md) of the [bending moment](../../../../bending-moment.md) in the absence of a point couple gives $[Bw'']=0$, or $[w'']=0$ for constant $B$.

The only allowed discontinuous section resultant is the [transverse shear force](../../../../transverse-shear-force.md). Integrating vertical [force balance](../../../../force-balance.md) through an upward [point force](../../../../point-force.md) $R_i$ gives $[N]=-R_i$. Since $N=-Bw'''$, this is precisely

$$
\boxed{[Bw''']=R_i.}
$$

The same sign follows by integrating $Bw''''-Tw''+p=R_i\delta(x-x_i)$, where $\delta$ is the [Dirac delta function](../../../../dirac-delta-function.md) and the regular terms have vanishing integrals over a shrinking interval. For nonadhesive [unilateral beam contact](../../../../unilateral-beam-contact.md), the required constraint is

$$
\boxed{R_i\geq0.}
$$

A negative [point force](../../../../point-force.md) would pull the [elastic beam](../../../../elastic-beam.md) towards the obstacle. At an endpoint where $R_i=0$, the third [derivative](../../../../derivative.md) is continuous as well.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
