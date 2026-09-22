<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let

$$
s_m=a\exp\left(\frac{P_m-P_c}{4\tau_Y}\right),\qquad
\Delta=P_m-P,\qquad0\leq\Delta\leq P_m.
$$

At maximum [pressure](../../../../pressure-split.md), the [stress](../../../../stress.md) is the field from part (c) with $P=P_m$ and $s=s_m$. Under the assumed [elastic unloading](../../../../elastic-unloading.md), previously accumulated plastic [strain](../../../../strain.md) is frozen. Therefore it is the [stress](../../../../stress.md) increment, rather than the total [stress](../../../../stress.md), that satisfies homogeneous [linear elasticity](../../../../linear-elasticity.md) and [radial elastic compatibility](../../../../radial-elastic-compatibility.md). Applying the [superposition principle](../../../../superposition-principle.md), a [pressure](../../../../pressure-split.md) change $-\Delta$ produces the elastic increments

$$
\delta q=\Delta\frac{a^3}{r^3},\qquad
\delta t=-\frac{\Delta}{2}\frac{a^3}{r^3}.
$$

They have zero far-field [stress](../../../../stress.md) and change the wall [traction](../../../../traction.md) from $-P_m$ to $-P$. These increments are the same in the formerly plastic and formerly elastic regions because their elastic [Lamé parameters](../../../../lame-parameter.md) agree. Adding them to the maximum-load field gives

$$
\boxed{q(r;P)=
\begin{cases}
-P_m+4\tau_Y\log(r/a)+\Delta(a/r)^3,&a\leq r\leq s_m,\\
-P_c(s_m/r)^3+\Delta(a/r)^3,&r\geq s_m,
\end{cases}}
$$

and

$$
\boxed{t(r;P)=\tau_{\phi\phi}(r;P)=
\begin{cases}
-P_m+4\tau_Y\log(r/a)+2\tau_Y-\tfrac12\Delta(a/r)^3,&a\leq r\leq s_m,\\
\tfrac12P_c(s_m/r)^3-\tfrac12\Delta(a/r)^3,&r\geq s_m.
\end{cases}}
$$

These formulae retain $s_m$: it records the plastic loading history and is not the instantaneous loading-front formula with $P$ substituted for $P_m$. If the entire return is elastic, setting $\Delta=P_m$ gives the [residual stress](../../../../residual-stress.md) after removal of the applied [pressure](../../../../pressure-split.md).

To check admissibility, examine the signed difference of the [principal stresses](../../../../principal-stress.md) in the formerly plastic shell:

$$
D(r)=q-t=-2\tau_Y+\frac{3\Delta}{2}\left(\frac ar\right)^3.
$$

It immediately moves into the interior of the [Tresca yield criterion](../../../../tresca-yield-criterion.md) when unloading starts. It can next reach the opposite limit $D=+2\tau_Y$. For fixed $\Delta>0$, $D$ is largest at $r=a$ and stays above $-2\tau_Y$. At the wall,

$$
-2\tau_Y+\frac32\Delta=2\tau_Y
\quad\Longleftrightarrow\quad
\Delta=\frac83\tau_Y=2P_c.
$$

There is no earlier violation in the outer region. Indeed,

$$
D(r)=D(s_m)\left(\frac{s_m}{r}\right)^3,\qquad r\geq s_m,
$$

so its magnitude is no larger than $|D(s_m)|$, which has already been controlled by the shell calculation. Hence the first [reverse yielding](../../../../reverse-yielding.md) occurs at the cavity wall, with

$$
\boxed{\Delta_{\mathrm{reverse}}=2P_c=\frac83\tau_Y,\qquad
P_{\mathrm{reverse}}=P_m-2P_c.}
$$

If $P_c<P_m<2P_c$, the [stress](../../../../stress.md) stays within the [yield surface](../../../../yield-surface.md) throughout unloading to zero. If $P_m=2P_c$, it reaches reverse yield exactly at $P=0$; further unloading would produce reverse plastic deformation. If $P_m>2P_c$, reverse plastic deformation starts while the applied [pressure](../../../../pressure-split.md) is still positive. Thus

$$
\boxed{\text{reverse yielding before zero pressure occurs iff }P_m>\frac83\tau_Y.}
$$

If “yield again while unloaded” includes first touching the [yield surface](../../../../yield-surface.md) at the final endpoint, the corresponding condition is $P_m\geq8\tau_Y/3$. The displayed [elastic unloading](../../../../elastic-unloading.md) fields are physically valid only for $0\leq\Delta\leq\min(P_m,2P_c)$; beyond that interval a new reverse-plastic region must be solved for. Continuing the elastic formula to $P=0$ when $P_m>2P_c$ would violate the given [Tresca yield criterion](../../../../tresca-yield-criterion.md).

## ↑ Ancestors (12)

1. [D](../d.md)
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
