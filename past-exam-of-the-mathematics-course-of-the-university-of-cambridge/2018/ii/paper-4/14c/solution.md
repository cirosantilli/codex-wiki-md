<h1 id="14c/solution">Solution</h1>

↑ **Parent:** [14C](../14c.md)

The $u^2/v$ term makes $u$ locally autocatalytic, while increasing $v$ suppresses this production. Thus **$u$ is the activator and $v$ is the inhibitor**.

At a positive [spatially homogeneous equilibrium](../../../../../spatially-homogeneous-equilibrium.md),

$$
\frac{u^2}{v}-2bu=0,
\qquad
u^2-v=0.
$$

Hence $u=2bv$ and $v=u^2$, giving

$$
\boxed{(u_*,v_*)=\left(\frac1{2b},\frac1{4b^2}\right).}
$$

The reaction [Jacobian matrix](../../../../../jacobian-matrix.md) there is

$$
J=
\begin{pmatrix}
2b&-4b^2\\
1/b&-1
\end{pmatrix},
\qquad
\operatorname{tr}J=2b-1,
\qquad
\det J=2b.
$$

Because $b>0$, the [trace-determinant stability criterion](../../../../../trace-determinant-stability-criterion.md) shows that the spatially uniform reaction kinetics are stable exactly when

$$
\boxed{0<b<\frac12.}
$$

For a perturbation proportional to $e^{\lambda t+ikx}$, put $q=k^2$. Its growth rates are the eigenvalues of

$$
J-q
\begin{pmatrix}d&0\\0&1\end{pmatrix}.
$$

The trace is $2b-1-(d+1)q<0$ in the reaction-stable regime, while the determinant is

$$
\Delta(q)=dq^2+(d-2b)q+2b.
$$

A [Turing instability](../../../../../turing-instability.md) occurs exactly when this upward-opening quadratic is negative for some $q>0$. By the [two-species diffusion-driven instability criterion](../../../../../two-species-diffusion-driven-instability-criterion.md), this requires

$$
d<2b,
\qquad
(2b-d)^2>8bd.
$$

Together these reduce to

$$
\boxed{0<b<\frac12,\qquad 0<d<(6-4\sqrt2)b.}
$$

Thus the unstable region in the $(b,d)$-plane lies below the straight line $d=(6-4\sqrt2)b$ and to the left of $b=1/2$.

Inside this region, the unstable squared-wavenumber band is

$$
\boxed{\frac{2b-d-\sqrt{(2b-d)^2-8bd}}{2d}
<k^2<
\frac{2b-d+\sqrt{(2b-d)^2-8bd}}{2d}.}
$$

At the bifurcation boundary the two roots coincide, so

$$
k_c^2=\frac{2b-d}{2d}.
$$

Substituting $d=(6-4\sqrt2)b$ yields

$$
\boxed{k_c=\sqrt{1+\sqrt2}.}
$$

## ↑ Ancestors (10)

1. [14C](../14c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
