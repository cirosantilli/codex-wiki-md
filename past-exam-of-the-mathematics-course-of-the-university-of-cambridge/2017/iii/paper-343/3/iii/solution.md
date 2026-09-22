<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a straight singly quantized [quantum vortex](../../../../../../quantum-vortex.md), use cylindrical distance $r$ from the line and write

$$
\psi=f(r)e^{i[\theta+\chi(r)]},\qquad f\geq0,\qquad k(r)=\chi'(r),\qquad \xi=\xi_R+i\xi_I.
$$

There is no dependence along the vortex line. Substitution into the normalized stationary equation gives, before separating real and imaginary parts,

$$
f''+\frac{f'}r-\frac f{r^2}-fk^2+i\left(2f'k+fk'+\frac{fk}r\right)+\xi(1-f^2)f=0.
$$

Consequently the [wave amplitude](../../../../../../wave-amplitude.md) and phase-gradient equations are

$$
\boxed{\begin{aligned}f''+\frac{f'}r-\left(\frac1{r^2}+k^2\right)f+\xi_R(1-f^2)f&=0,\\
k'+\left(\frac1r+2\frac{f'}f\right)k&=-\xi_I(1-f^2).\end{aligned}}
$$

The second equation can also be written $(r f^2 k)'=-\xi_I r f^2(1-f^2)$, which remains convenient at the core.

To specify what is meant by radial [velocity](../../../../../../velocity.md), use the [condensate number current](../../../../../../condensate-number-current.md). The time-dependent equation has kinetic operator $-\nabla^2$ and therefore number current $\mathbf j=2|\Psi|^2\nabla S$. Its hydrodynamic [superfluid velocity](../../../../../../superfluid-velocity.md) in these units is $\mathbf u=2\nabla S$, so $u_r=2k$ and $u_\theta=2/r$. In that convention the requested pair is

$$
\boxed{\begin{aligned}f''+\frac{f'}r-\frac f{r^2}-\frac{u_r^2}{4}f+\xi_R(1-f^2)f&=0,\\
u_r'+\left(\frac1r+2\frac{f'}f\right)u_r&=-2\xi_I(1-f^2).\end{aligned}}
$$

If instead [velocity](../../../../../../velocity.md) is defined as the [complex argument](../../../../../../argument-complex-analysis.md) [gradient](../../../../../../gradient.md) itself, the preceding $k$ pair is the corresponding convention; the distinction matters because the printed kinetic coefficient differs from that of the normalized conservative equation in Question 1.

Regularity of a unit-charge core gives $f(r)=ar+O(r^3)$ with $a>0$. Integrating the current equation from the origin, with no point source or singular radial flux, gives

$$
r f^2 u_r=-2\xi_I\int_0^r s f(s)^2(1-f(s)^2)\,ds.
$$

The [integral](../../../../../../integral.md) is $a^2r^4/4+O(r^6)$, so the [radial flow near a driven vortex core](../../../../../../radial-flow-near-a-driven-vortex-core.md) is

$$
\boxed{u_r(r)=-\frac{\xi_I}{2}r+O(r^3)=\frac\alpha2r+O(r^3),\qquad u_r'(0)=\frac\alpha2.}
$$

For the phase-gradient convention, $k'(0)=-\xi_I/4=\alpha/4$. Gain exceeds loss in the depleted core, hence this regular flow is outwards for $\alpha>0$. The real [wave amplitude](../../../../../../wave-amplitude.md) equation also gives $f=ar-\xi_R ar^3/8+O(r^5)$, independently consistent with the linear core behaviour. A nonzero integration constant in the radial-current identity would create a singular $u_r\sim r^{-3}$ and is excluded.

Finally, the literal boundary $\psi\to1$ from the preceding part cannot apply to a multiplicity-one vortex: its [complex argument](../../../../../../argument-complex-analysis.md) changes by $2\pi$ around a large circle. Even $f(r)e^{i\theta}$ with $f\to1$ has different limits along different rays. The usual intended vortex condition concerns the [wave amplitude](../../../../../../wave-amplitude.md) approaching its bulk value, with the winding [complex argument](../../../../../../argument-complex-analysis.md) retained; it is not a constant complex-field limit. The local equations and core slope derived here do not establish a global stationary vortex satisfying that literal boundary. In a driven system the far-field radial flow and oscillation frequency may also require selection, so no global zero-flow vortex is asserted.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
