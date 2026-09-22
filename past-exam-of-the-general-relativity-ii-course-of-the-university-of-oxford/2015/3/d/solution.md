<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $a>0$, the assumed inequality and the [Friedmann acceleration equation](../../../../friedmann-acceleration-equation.md) imply $\ddot a\le0$. Thus $a$ is a [concave function](../../../../concave-function.md). Let $a_0=a(t_0)>0$ and $v_0=\dot a(t_0)>0$. At every earlier time in the same regular expanding interval, $\dot a(t)\ge v_0$. Integration gives the [concavity bound on past FLRW evolution](../../../../concavity-bound-on-past-flrw-evolution.md):

$$
a_0-a(t)=\int_t^{t_0}\dot a(s)\,ds\ge v_0(t_0-t),
\qquad
\boxed{a(t)\le a_0-v_0(t_0-t).}
$$

The right-hand side reaches zero at $t=t_0-a_0/v_0$. Hence an everywhere regular positive [scale factor](../../../../scale-factor-cosmology.md) cannot extend arbitrarily far into the past. With the usual implicit continuation assumption that the cosmological solution remains regular while $a>0$, it reaches $a(t_B)=0$ at a finite past boundary satisfying

$$
\boxed{0<t_0-t_B\le\frac{a_0}{v_0}=\frac1{H(t_0)}.}
$$

**Past expansion lasts at most the present inverse [Hubble parameter](../../../../hubble-parameter.md).** The inequality is the essential argument, and equality is attained by a linearly growing [scale factor](../../../../scale-factor-cosmology.md).

There is a literal qualification to the claim that $a$ must reach zero: the printed hypothesis alone does not exclude an earlier [curvature singularity](../../../../curvature-singularity.md) with positive limiting $a$. In arbitrary fixed units, take $k=0$ and $a(t)=1+\sqrt t$ for $t>0$, and define $\varrho,p$ using the two [Friedmann equations](../../../../friedmann-equations.md) and the [Friedmann acceleration equation](../../../../friedmann-acceleration-equation.md). Then $\dot a>0$, $\ddot a<0$, and $\varrho+3p=-3\ddot a/(4\pi Ga)>0$, but $a\to1$ while the [energy density](../../../../energy-density.md) and [pressure](../../../../pressure-split.md) diverge as $t\downarrow0$. Thus the rigorous unconditional conclusion is the finite bound on a regular past interval; reaching zero additionally requires the stated continuation assumption. Nor does a zero of $a$ alone prove a [curvature singularity](../../../../curvature-singularity.md), as the [Milne model](../../../../milne-model.md) illustrates.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the general relativity II course of the University of Oxford](../../../split.md)
5. [General relativity II course of the University of Oxford](../../../../general-relativity-ii-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
