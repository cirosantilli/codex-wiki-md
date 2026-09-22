<h1 id="17g/solution">Solution</h1>

↑ **Parent:** [17G](../17g.md)

Assume homogeneous space and time, isotropic space, inertial frames related linearly, the relativity principle and a common isotropic speed $c$ for light. Take coincident origins at zero and parallel axes, with $S'$ moving at $v$ along $x$. The primed origin requires $x'=A(x-vt)$. Write $t'=Bx+Dt$; mapping each light ray $x=\pm ct$ into $x'=\pm ct'$ gives $D=A$ and $B=-Av/c^2$. Rotational symmetry about the boost axis gives a common transverse scale $B(v)$; reversing the boost direction by spatial isotropy gives $B(v)=B(-v)$. Reciprocity then gives $B(v)^2=1$, and continuity and the common orientation select $B(v)=1$. Thus transverse directions are unchanged. Reciprocity requires the inverse to have the same scale $A$ with $v$ replaced by $-v$. Composing gives $A^2(1-v^2/c^2)=1$; continuity from $A=1$ at $v=0$ selects the positive root. Hence the [Lorentz transformation](../../../../../lorentz-transformation.md) is

$$
\boxed{x'=\gamma(x-vt),\quad t'=\gamma(t-vx/c^2),\quad y'=y,\quad z'=z,\qquad \gamma=(1-v^2/c^2)^{-1/2}.}
$$

The printed wavelength formula uses the angle of the line of sight from observer towards star, opposite to photon propagation. Choose the transverse axis so the ray lies in the $xy$ plane. With that directed-angle convention the photon [four-momentum](../../../../../four-momentum.md) is

$$
\boxed{p'^\mu=\frac{h\nu'}c(1,-\cos\theta',-\sin\theta',0),\qquad p^\mu=\frac{h\nu}c(1,-\cos\theta,-\sin\theta,0).}
$$

The inverse coordinate boost takes a rest-frame four-vector to $S$, giving $p^0=\gamma(p'^0+\beta p'^1)$ and $p^1=\gamma(p'^1+\beta p'^0)$, where $\beta=v/c$. Thus $\nu=\gamma\nu'(1-\beta\cos\theta')$, and the [aberration of light](../../../../../relativistic-aberration.md) relation is $\cos\theta=(\cos\theta'-\beta)/(1-\beta\cos\theta')$. More directly, the boost from $S$ to $S'$ gives $p'^0=\gamma(p^0-\beta p^1)$, hence $\nu'=\gamma\nu(1+\beta\cos\theta)$. Since wavelength is $c/\nu$, the [relativistic Doppler effect](../../../../../relativistic-doppler-effect.md) gives

$$
\boxed{\lambda=\lambda'\gamma(1+\beta\cos\theta).}
$$

If the angle were instead measured along the actual photon momentum, both cosine signs would reverse and the same physical relation would have a minus sign. Specifying this orientation avoids confusing the two versions.

For $\cos\theta=1$, $\lambda/\lambda'=\sqrt{(1+\beta)/(1-\beta)}$: a receding star is redshifted. For $\cos\theta=-1$, the ratio is $\sqrt{(1-\beta)/(1+\beta)}$: an approaching star is blueshifted. For $\cos\theta=0$, $\boxed{\lambda/\lambda'=\gamma}$: the transverse redshift is the time-dilation effect. This transverse condition refers to the observer's angle, not $\theta'=\pi/2$ in the source frame.

## ↑ Ancestors (10)

1. [17G](../17g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
