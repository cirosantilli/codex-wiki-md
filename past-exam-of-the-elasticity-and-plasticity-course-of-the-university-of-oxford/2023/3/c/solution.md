<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

During increasing [pressure](../../../../pressure-split.md), the elastic solution reaches the [Tresca yield criterion](../../../../tresca-yield-criterion.md) with $t-q>0$. In the plastic shell of a material with [perfect plasticity](../../../../perfect-plasticity.md), this sign is retained and

$$
t-q=2\tau_Y.
$$

Radial [force balance](../../../../force-balance.md) becomes $q'-4\tau_Y/r=0$. Integrating from the cavity wall, where $q(a)=-P$, gives

$$
q=-P+4\tau_Y\log(r/a),\qquad t=q+2\tau_Y,
\qquad a<r<s.
$$

Outside the plastic shell, [radial elastic compatibility](../../../../radial-elastic-compatibility.md) and vanishing far-field [stress](../../../../stress.md) again give $q=-C/r^3$ and $t=C/(2r^3)$. At the advancing plastic front $r=s$, the [Tresca yield criterion](../../../../tresca-yield-criterion.md) gives $3C/(4s^3)=\tau_Y$, so $C=P_cs^3$. [Continuity](../../../../continuous-function.md) of radial [traction](../../../../traction.md) now gives

$$
-P+4\tau_Y\log(s/a)=-P_c.
$$

Thus

$$
\boxed{s=a\exp\left(\frac{P-P_c}{4\tau_Y}\right).}
$$

The complete [stress](../../../../stress.md) field of this [spherical elastoplastic cavity](../../../../spherical-elastoplastic-cavity.md) is

$$
\boxed{\tau_{rr}=
\begin{cases}
-P+4\tau_Y\log(r/a),&a\leq r\leq s,\\
-P_c(s/r)^3,&r\geq s,
\end{cases}
\qquad
\tau_{\theta\theta}=\tau_{\phi\phi}=
\begin{cases}
-P+4\tau_Y\log(r/a)+2\tau_Y,&a\leq r\leq s,\\
\tfrac12P_c(s/r)^3,&r\geq s.
\end{cases}}
$$

At $s$, the tangential [stress](../../../../stress.md) also matches because $-P_c+2\tau_Y=P_c/2$. Outside $s$, the function in the [Tresca yield criterion](../../../../tresca-yield-criterion.md) is $\tau_Y(s/r)^3<\tau_Y$, which verifies that the remaining material is elastic. As $P\downarrow P_c$, $s\downarrow a$ and the solution joins the entirely elastic regime. The radius $a$ is the fixed reference radius of the small-[strain](../../../../strain.md) model used by the paper.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
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
