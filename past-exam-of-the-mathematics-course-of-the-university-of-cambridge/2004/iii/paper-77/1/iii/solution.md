<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A freely swimming body has neither an imposed end couple nor an imposed end transverse [force](../../../../../../force.md). Its end [bending moment](../../../../../../bending-moment.md) is therefore zero, and the transverse force $S=G_x$ is also zero at both ends. These are the four [free-end bending boundary conditions](../../../../../../free-end-bending-boundary-conditions.md); they do not require the end displacement or slope to vanish.

Put $R=m_bh_{tt}+\mathcal D(m\mathcal Dh)$, using the physically consistent sign. Integrating $G_{xx}=R$ with the two leading-end conditions gives

$$
G_x(x,t)=\int_0^xR(s,t)\,ds,\qquad G(x,t)=\int_0^x(x-s)R(s,t)\,ds.
$$

The two trailing-end conditions consequently require

$$
\boxed{\int_0^L R\,dx=0,\qquad \int_0^L xR\,dx=0.}
$$

These [free-end compatibility for a swimming beam](../../../../../../free-end-compatibility-for-a-swimming-beam.md) conditions are total transverse [force](../../../../../../force.md) and [torque](../../../../../../torque.md) balances. They explain why an arbitrary plausible prescribed $h$ does not suffice: two integration constants can satisfy only two end conditions unless the forcing already satisfies both compatibility integrals.

The missing freedom is the [swimming recoil correction](../../../../../../recoil-correction-in-elongated-body-theory.md). An observed or prescribed deformation $h_d$ relative to the body must be supplemented by a lateral translation $Y(t)$ and a small yaw $\Theta(t)$:

$$
h(x,t)=h_d(x,t)+Y(t)+\Theta(t)(x-x_c),\qquad x_c=\frac{\int_0^Lxm_b\,dx}{\int_0^Lm_b\,dx}.
$$

To identify $Y$ with the actual [centre of mass](../../../../../../center-of-mass.md) displacement, first remove the body-mass-weighted mean from $h_d$. One may also remove its body-mass-weighted first moment about $x_c$ to define the yaw reference uniquely. This changes the decomposition of the observed motion, not the physical displacement.

For $\xi=x-x_c$, the recoil contribution to the forcing is

$$
R_{\rm rec}=(m_b+m)(Y''+\xi\Theta'')+2Um\Theta'+Um'Y'+Um'\xi\Theta'+U^2m'\Theta.
$$

Insert $R=R_d+R_{\rm rec}$ into the two compatibility integrals, using $1$ and $\xi$ as weights. This gives two coupled [ordinary differential equations](../../../../../../ordinary-differential-equation.md) for the two recoil motions. Their principal acceleration matrix is

$$
\begin{pmatrix}\int_0^L(m_b+m)dx&\int_0^L\xi(m_b+m)dx\\\int_0^L\xi(m_b+m)dx&\int_0^L\xi^2(m_b+m)dx\end{pmatrix}.
$$

For a nondegenerate positive mass distribution it is a [positive-definite matrix](../../../../../../positive-definite-matrix.md): its quadratic form at $(a,b)$ is $\int_0^L(m_b+m)(a+b\xi)^2dx>0$ unless $a=b=0$. Thus initial translation and yaw determine the recoil through these equations, and the corrected $h$ supplies the two compatibility conditions. **The four free-end conditions determine the bending moment together with two rigid recoil motions; they do not overdetermine a physically complete swimming motion.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
