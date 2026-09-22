<h1 id="37b/solution">Solution</h1>

↑ **Parent:** [37B](../37b.md)

In [lubrication theory](../../../../../lubrication-theory.md), the gap scale $H$ is small compared with the axial scale $L$, so $\delta=H/L\ll1$ and wall slopes are small. [Incompressibility](../../../../../incompressible-flow.md) makes the transverse velocity scale $\delta U$. The reduced [Reynolds number](../../../../../reynolds-number.md) is $\rho UH^2/(\mu L)=\delta\operatorname{Re}_H$, and must be small to neglect convection; the transverse viscous diffusion time must also be short compared with the wall-motion time to neglect unsteady inertia. For a Newtonian incompressible fluid with no axial wall motion, the leading equations are $p_y=0$ and $\mu u_{yy}=p_x$.

No slip gives $u(0)=u(h)=0$. Integrating twice and then across the gap gives

$$
\boxed{u=\frac{p_x}{2\mu}y(y-h),\qquad q=\int_0^hu\,dy=-\frac{h^3}{12\mu}p_x.}
$$

Integrate $u_x+v_y=0$ and differentiate the moving-limit flux. The lower wall has $v(0)=0$, and the upper kinematic condition is $v(h)=h_t+u(h)h_x$. These terms cancel to give

$$
\boxed{h_t+q_x=0.}
$$

For a travelling gap $h(x-ct)$, this becomes $(q-ch)_x=0$, so $q=ch+Q$ with $Q$ independent of position. Zero mean pressure gradient gives

$$
0=\langle p_x\rangle=-12\mu\left[c\langle h^{-2}\rangle+Q\langle h^{-3}\rangle\right],
$$

therefore

$$
\boxed{\langle q\rangle=c\left[\langle h\rangle-\frac{\langle h^{-2}\rangle}{\langle h^{-3}\rangle}\right].}
$$

The positivity of $h$ is assumed so these averages exist. The wall pattern travels without an imposed mean pressure difference; the changing gap and its inverse-cubic hydraulic resistance produce the pumping.

## ↑ Ancestors (10)

1. [37B](../37b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
