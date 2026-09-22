<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a steady flow, [mass conservation](../../../../../../mass-conservation.md) gives $\rho w=\text{constant}$ and $\rho'/\rho=-w'/w$. Define the [Alfvén velocity](../../../../../../alfven-velocity.md) $\mathbf v_a=\mathbf B/\sqrt{\mu_0\rho}$ and $C=w^2-v_{az}^2$. Combining the horizontal momentum and [MHD induction equations](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) without dividing by $C$ gives

$$
C B_x'=-wB_xw',\qquad
C B_y'=-wB_yw'+a(wB_x-B_zv_x).
$$

Dot these identities with $B_x/(\mu_0\rho)$ and $B_y/(\mu_0\rho)$, respectively:

$$
\frac{C}{\mu_0\rho}(B_xB_x'+B_yB_y')
=-w(v_{ax}^2+v_{ay}^2)w'
+a v_{ay}(wv_{ax}-v_{az}v_x).
$$

The vertical momentum equation and the [isothermal equation of state](../../../../../../globally-isothermal-equation-of-state.md) give

$$
\left(w-\frac{c_s^2}{w}\right)w'
=-g-\frac{B_xB_x'+B_yB_y'}{\mu_0\rho}.
$$

Multiply by $C$ and eliminate the magnetic derivative to obtain

$$
\boxed{\left[w^4-(c_s^2+v_a^2)w^2+c_s^2v_{az}^2\right]\frac{w'}w
=g(v_{az}^2-w^2)+a v_{ay}(v_xv_{az}-wv_{ax}).}
$$

No division by $w^2-v_{az}^2$ was needed in deriving this necessary relation.

The [magnetosonic critical speeds](../../../../../../magnetosonic-critical-speed.md) in the $z$ direction are

$$
c_{\mathrm f,\mathrm s}^2=
\frac12\left[c_s^2+v_a^2
\ \mathbin{\pm}\
\sqrt{(c_s^2+v_a^2)^2-4c_s^2v_{az}^2}\right].
$$

The plus sign gives the [fast magnetosonic wave](../../../../../../fast-magnetosonic-wave.md) speed and the minus sign the [slow magnetosonic wave](../../../../../../slow-magnetosonic-wave.md) speed. Thus the differential coefficient is $(w^2-c_{\mathrm f}^2)(w^2-c_{\mathrm s}^2)$. A smooth outflow proceeding from below both speeds to above both must normally pass through both [magnetosonic critical speeds](../../../../../../magnetosonic-critical-speed.md). At each crossing, **the right-hand side must also vanish**; this is the [regularity at a magnetosonic point](../../../../../../regularity-at-a-magnetosonic-point.md) condition. The derivative coefficient changes sign at each nondegenerate crossing. For $w>0$ and $w'>0$, the driving term must be positive below the slow point, negative between the points and positive above the fast point.

The [Alfvén speed](../../../../../../alfven-speed.md) component satisfies $c_{\mathrm s}^2\leq v_{az}^2\leq c_{\mathrm f}^2$. With downward gravity $g>0$, the gravitational term is consequently nonnegative at the slow point and nonpositive at the fast point. The [magnetohydrodynamic shear work](../../../../../../magnetohydrodynamic-shear-work.md) contribution must balance it at each point, and can provide the upward driving needed to pass the fast point. For $a=0$ and strictly positive $g$, generic separated slow and fast points cannot satisfy the required zero numerator; special vanishing-gravity or coincident-speed cases need separate treatment.

There is also [Alfvén-point compatibility in a plane-parallel sheared flow](../../../../../../alfven-point-compatibility-in-a-plane-parallel-sheared-flow.md). At $w^2=v_{az}^2$, the original transverse equations require

$$
wB_xw'=0,\qquad
wB_yw'=a(wB_x-B_zv_x).
$$

These restrictions are not generally visible as a zero of the scalar differential coefficient, which there equals $-v_{az}^2(v_{ax}^2+v_{ay}^2)$. In particular, a strictly accelerating regular solution must have $B_x=0$ at that point. The scalar relation is therefore a necessary wind equation, not a substitute for regularity of all the original [ideal magnetohydrodynamic equations](../../../../../../ideal-magnetohydrodynamic-equations.md). Degenerate cases such as a purely longitudinal [magnetic field](../../../../../../magnetic-field.md) can merge characteristic speeds and reduce the number of distinct critical conditions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
